[[- User Manual Info -]]
# Snappers
The Rusty Drone utilizes multiple different snapper tags for its modularity functions. The following documentation serves as both a record of these systems and a guide on how to interface with them.

Unless otherwise specified, assume each part has its origin located roughly at the center of mass and is oriented such that its "forward" and "up" correspond to the positive Z-axis and positive Y-axis, respectively.
## RustyScreen
The "RustyScreen" tag is used for goggles and glasses, almost always covering the eyes.
## RustyHead
Detachable heads are a staple characteristic of Neolander interactions.
## RustyHat
A generic hat snapper tag. Origins should be on the surface of the head (generally the bottom of a hat or inside of a helmet).
## RustyPowerCore
In order to function correctly, power cores must have the "RustyPowerCore" dynamic variable space and the "RustyPowerCore/PowerSupply" dynamic variable of type float, where the value is any positive number (0 being no supply, 100 being full power, and greater than 100 being overcharged). 
#### Parent Values
RustyPowerCore Snappers can read the following parent values

| Tag              | Data Type | Function                                                                                         |
| ---------------- | --------- | ------------------------------------------------------------------------------------------------ |
| LeftConnection   | Slot      | If detected, a line of plasma will flicker on from the core's left port to the designated slot   |
| RightConnection  | Slot      | If detected, a line of plasma will flicker on from the core's right port to the designated slot  |
| CenterConnection | Slot      | If detected, a line of plasma will flicker on from the core's middle port to the designated slot |
## RustyArm
This tag is the most in-depth in terms of required systems to function. Slots with a RustyArm Snapper are to be oriented such that the positive Z-axis is facing away from what it is attached to and positioned such that the origin of the object is the attachment point.
#### Parent Values
RustyArm Snappers can read the following parent values

| Tag         | Data Type | Function                                                                                   |
| ----------- | --------- | ------------------------------------------------------------------------------------------ |
| Attached    | Bool      | Signals if the arm is in a valid SnapTarget                                                |
| Deployed    | Bool      | If the arm has a retraction state, this controls it                                        |
| Grabbable   | Bool      | Whether or not the part can be grabbed.                                                    |
| Chirality   | Bool      | Determines chirality of the attached hand (if applicable). True for right, False for left. |
| EndTarget   | Slot      | The slot the onboard IK will attempt to match the position of                              |
| JointTarget | Slot      | The slot the onboard IK will point the upper arm at                                        |
| PartType*   | String    | Indicates what type of SnapTarget the part is attached to                                  |
*\*PartType has support for "Eye", "Arm", "Leg", "Hand", "Foot", and "Neck"*
#### Inverse Kinematics
Two slots are necessary for the arm to move properly. Both should be parented under the avatar's hand proxy. For an arm, EndTarget is the slot whose position the wrist should pivot around (the tip of the blue arrow) while JointTarget is the slot whose position guides the upper arm (the purple ball at the tip of the green arrow).

![[Rusty IK Diagram.png]]
*Pictured: A functional RustyArm and RustyHand. the green arrow indicates the shoulder's target while the blue arrow indicates the elbow's target.*

Generally, the EndTarget is best positioned at the origin of an avatar's hand with the JointTarget moved along the negative Z-axis to a distance roughly the length of the user's forearm.
## RustyHand
If used, the RustyHand tag should be located on the end of a RustyArm oriented such that the fingers point along the positive Z-axis (this should result in the palm being at the "bottom). The origin of the hand should be positioned at the wrist's pivot point.
#### Parent Values
RustyHand Snappers can read the following parent values

| Tag       | Data Type | Function                                                              |
| --------- | --------- | --------------------------------------------------------------------- |
| Attached  | Bool      | Signals if the hand is in a valid SnapTarget                          |
| Deployed  | Bool      | If the arm has a retraction state, this controls it                   |
| Grabbable | Bool      | Whether or not the part can be grabbed.                               |
| Chirality | Bool      | Determines chirality (if applicable). True for right, False for left. |
| Elbow     | Slot      | Drives the LookAt in the wrist joint                                  |
| PartType* | String    | Indicates what type of SnapTarget the part is attached to             |
*\*PartType has support for "Eye", "Arm", "Leg", "Hand", "Foot", and "Neck"*