[[- User Manual Info -]]
#### 0.1-0.9:

Base Model
Added left hand sword, Shield, and seat
Limbs are now modular
#### 1.0:

HUD implementation
#### 1.1:

Set up indicator icons
#### 1.2:

User Join notifier
#### 1.3:

Current face display feed
#### 1.4:

Emote Wheel (happy, deadpan, brow)
#### 1.5:

Functional Emote Wheel
#### 1.6:

Functional sad face
Face display no longer breaks when not at 1 global scale
#### 1.7:
 
Exosuit animation and helmet
#### 1.8:

Sounds added to booting and suiting
#### 1.9:

Added high five visuals
Added removable sword arm
#### 1.10:

Added exosuit gauntlets
High five to activate exosuit mode
Exosuit Drone MMC submission
#### 1.11:

Added time display
Added controller battery display
Added steam menu loading face
Added talking lights dynvar
#### 1.12:

Bugfixes
Minor tweaks
Added gauntlet thrust indicators
Drone now turns green when suited on sloppy
Bitbot now has dynamic thrust
#### 1.13:

Exosuit can now be disengaged by the wearer or pilot by holding both radial buttons
Thruster mode now has an indicator for current output strength
#### 1.14:

Added legs
Arms now retract on power down
Fixed security loophole in modularity
Restructured boot sequence
Fixed thrust particle mesh facing direction
#### 1.15:

New hidden menu system
Bitbot DroneCamera
Proper Finger animation system (finally!)
New emotes (wink, wide-eyed, angry, blush)
Bitbot now has dynamic thrust
#### 1.16:

Expandable modular hand transformations
Enabled manual access to gauntlets
Switching between hand modes without going to normal in between no longer breaks the finger positions
Right arm is now also a removable weapon
#### 1.17:

Anchor Space no longer duplicates itself if one already exists
Suit equipping now works on the first try
Ending modular mode animates the parts back to place instead of teleporting
Leg mode now has a notification icon
Sword now makes sound when swinging
High five sound doesn't move with the Drone anymore
#### 1.17.5:

[UNSTABLE] First implementation of hand multitool (has devtip and logix, but only the devtip transformation)
Missing Bitbot
#### 1.18: 
  
Multitool now has both transformations
Label and press indicator for logixtip now displays on HUD
Logixtip now visually transforms
Re-added Bitbot (hopefully permanently)
Added scaling to finger tweens to prevent them sometimes getting stuck at zero
Sword hands now have a slice trail
#### 1.19:

All lights and particles are now driven by the UserDefaultColor cloud variable
New (probably temporary) bootup sound, destroyblock on hands, arms, and Bitbot
Bitbot now fires a laser for gizmo/wire clear
Adjusted arm points in suit mode
Lower spread and rate of thrust visuals while ascending
Buster can now be used by the person holding it while detached
Suit mode gauntlets can now be controlled autonomously by the Pilot
Hands now use finger posing from whoever is holding them rather than only the Pilot
Added crane mode arm snapper
Set Drones in an area to be on by default
Full throttle on both thrusters now activates a boost
Suiting onto someone now changes lights to their colors
New HUD icons for global/local UI and Drone power
User leaving pop-up now shows who left
#### 1.20:

New boot up sound courtesy of Engi!
Shields now have proper colliders (raycasts and projectiles won't detect a player on hit)
Fixed a bug where suit-up high fives wouldn't delete themselves
New pixel art emote icons to replace the old screen pictures
Changed gauntlet mode selection to double radial
Moved grab sphere in multitool mode
Dequipping multitool through the radial menu now properly reverts the fingers
New thruster boost effect animation
Boosting in reverse now fully cancels out momentum
Major overhaul to leg logix and walking animation, feet now lift off the ground while stepping, make small sounds, and use coordinates rather than slots as targets
New gravity change ability by touching right ear button and clicking a surface with left hand
Suiting onto a user without a default color now defaults to PilotColor
UserDefaultColor is now used for PilotColor when no cloud variable is detected
Bitbot now stays upright relative to global gravity
Prime Unit now Localizes context menus on boot
Changed hardlight material from specular to intersect
Simplified logix and fixed multiple bugs by completely reworking how hand modes are detected
Thruster is now the default gauntlet mode
Bitbot can now be toggled through the menu and has a bootup/shutdown animation
Bitbot multitools are now stored in Dataspace so they can be turned off while suiting
Idling multiple Bitbots will cause them to float in an arc overhead
#### 1.21:

New chest compartment feature, contains a Rusty Cola, Shock Rock, Talking lights cube, and Rusty Power Core
Hand transformations are now cleared on shutdown
Reorganized gauntlet logix
Added blaster mode (old blaster is now named repulsor)
Centralized snappers on the head (goggles, crane mode, etc)
Added hat snapper and christmas hat
#### 1.22:

Buster now has Beam option, click trigger to overdrive
Rusty Cola now opens
Text scrolling finally added to boot sequence!
Fixed eyes sometimes overlapping with text on boot
Fixed eyes not smoothing between sizes when entering and exiting loading animation
Power core now modularly connects to any drone
Power core can be opened and closed while disconnected
Reorganized bitbot swarm
Bitbot swarm is now also hidden when retracting the alpha
Radial Localizers are now replaced when entering a new drone
Bitbot now focuses TargetedUser in camera mode
Added Bitbot Christmas hat
Added Deployable platforms as a secondary option of the gravity setter tip
Added pulsing hex particles to buster beam mode
Added boost effect on beam overdrive
Fixed one eye being resized incorrectly in the loading animation
Changed how Bitbot Multitools get stored so they don't become nonpersistent
Vastly improved power core open/close animation
Power core can no longer be grabbed while open
Added new overlay for power level
Set up system for any item to provide a unique amount of power generation
Drone now shuts off completely if it reaches 0% power
Talking lights are now responsive to power level.
Bitbot can now retrieve the power core when it is removed
Shock Rock now provides 50% power when inserted
Added Doppler Perch
Fixed the Bitbot multitool receiver not deleting itself when emptied
Improvements to beam visuals
#### 1.23:

Power core now easily links to up to three connection points designated by dynamic slots
Power core is now open while in drone and retracts on grab
New hand transformation for Buster mode
Arms can now be retracted manually
Wren mask snapper
Legs now have a jump position
First implementation of Rocket Mode! Pitch and roll are controlled with head rotation, movement is sped up and slipperier
Hands become thrusters and lock to torso in rocket mode
Improved rocket mode thruster trails
Drone can now be ridden like a hoverboard while in rocket mode
Drone is no longer scalable
Legs icon no longer appears while in rocket mode
Added component clone and material tips to multitool, hold left grip while switching to access
Redid menu system and emote selection to use distance instead of raycasting, making them far more reliable
Menu buttons now visually signify hover and click
Bitbot now has screen tapping
Reconnecting sound no longer plays when toggling off modularity if arm/hand is already connected
Arms/hands aren't grabbable while retracted
Added character colliders to shields
Added menu button for belly compartment
Restructured arm retraction to clear up chest compartment
Neck now retracts on shutdown
Belly compartment now has double doors
Added new quick menu category for transformations: Modes
Added Bike Mode!
Added Bike Mode locomotion sensor
Added Bike Mode tread
Fixed hitbox while in Rocket and Bike Modes
Increased size of anchor hitbox in Rocket and Bike Modes
Added user targeting reticles
#### 1.24:

Cleaned up user targeting reticles
-Added ping counter
-Added FPS counter
Moved thrust direction calculation to head direction while in rocket mode
Added preliminary support for Ultra Cannon mode
Changed chest compartment to flip down rather than swing out
Changed screen material to specular from unlit
Added speedometer to HUD, appears while in rocket mode or moving faster than 12 m/s
Doubled thruster power
Thruster power now scales with user size
Gauntlet User variable is now driven instead of written
Quick menu is now inaccessible to individuals of access level 3 and below
Ultra cannon mode uses power core as a focus for a beam (temporary)
#### 1.25:

New Minigun stored in the lower torso!
Disabled grip to revert to normal hands in rocket and turret mode
Left trigger now controls both thrusters in rocket mode
Right trigger deploys the minigun, hold to spin up and fire
Right grip retracts the gun
Turret mode now attaches the minigun to the front of the power core
User targeting reticles are set to visible while the minigun is deployed
Added sound driver to minigun spinning
Turret mode now has shields
Fixed a bug where arm meshes wouldn't disable when retracting
Prevented minigun from being deployed in bike mode
Exosuit target visuals now only track users while the menu is open
Removed distance requirement for equipping exosuit
Improved leg logix to dynamically step based on furthest foot rather than all in order
Separated Bike Mode from Rocket Mode
Completely overhauled Bike Mode:
-Locomotion is a modified walk instead of fly
-Fixed back tread disappearing too early
-Added front tread
-Treads now raycast to the ground and rotate with velocity
Thrusters are now controlled with the joystick in Bike and Rocket mode
Hold left grip and tap secondary while looking at a user to anchor them
Added vocal waveform to suit mode HUD
Enabled speedometer while in suit mode
Added a running gait to leg logix that activates when moving fast enough
Added rudimentary leg deploy/retract animation
Legs now auto deploy in turret mode
Activating Turret Mode now forces the drone into walk mode
Added flashlight mode to left hand
Unified materials used on legs and feet
Fixed bike mode treads not rotating correctly
Arms can now be deployed by pressing both grips
Fixed thruster particle speed at abnormal user scale
Fixed shields being inconsistent in turret mode
Drone's head now stops tracking while neck is retracted
#### 1.26:

Added crude Compact Mode that folds the whole drone into its head
Front tread now extends in Compact Mode while grounded
Both grips now release arms from retraction
Treads now move in accordance to drone speed
Rusty context menu options are no longer available while holding a powered-down drone
Fixed forcing a user on/off vehicle anchor causing them to get stuck weirdly rotated
Added pen hand to multitool, touch left trackpad while switching tools
Improved Rusty Clearables deletion
Suit mode now uses the wearer's finger pose
Changed forcing a user to ride vehicle mode to hold left grip and look at them within 1 meter
Optimised and centralized finger meshes
Added proper ObjectRoot and Default scale
Added side panels in the head to hold future weaponry (likely missile pods)
Converted platform collider to convex hull
Blaster shots now destroy on impact
Compact mode can now convert to Bitbot with left trigger
Added sound when converting to Bitbot Mode
Replaced blaster bullets with laser pulse
Added material pallet to left hand in multitool Pen Mode
Eyes now become headlights in Bike Mode
#### 1.27:

REPLACED CHEST, HAND, FOOT, AND ABDOMEN MESHES WITH CUSTOM BLENDER VERSIONS. This removes five slice materials from the avatar
Fixed/updated away materials
Added panel openings to shoulders for future missile pods
Added manual control of missile pod flaps
Bitbot now stays deployed when power core is removed, even on shutdown
Fixed desktop camera Bitbot's nametag color
Removed outline and added talking glow to nametag
Fixed Rusty Cola using debug material instead of grey
Replaced minigun shell meshes with blender meshes
Fixed foot1 still using a slice material
Chest compartment is now uniformly scaled and has panels in the shoulder sockets
Replaced head with custom meshes
Replaced screen with custom meshes
Replaced head seams with custom meshes
Replaced mouth with custom meshes
Removed at least five more slice materials
Localized interior of face and screen
Added screen to modularity parts
Screen interior now disappears when held close to a user's face
Screen now contains voice output
Separated panels from shoulder connectors for arm retraction
Grabbability of screen is now properly driven
Continued optimizing avatar (removing deactivated components, converging identical meshes)
Added head guns, aimed with left controller and fired with left trigger
Head guns now change sound and fire slower while in Bitbot Mode
Fixed right head gun being grabbable
Fixed head gun oneshotaudios not deleting themselves
Added laser visual to head guns
Added hit effect to head guns
Modified knockback of all blaster type weapons to jostle the target rather than send them flying on the first hit
Prototyped a new type of swarm missile using wobblers
Fixed away materials
Fixed desktop camera Bitbot's antennas glowing
Fixed shoulder Bitbot's eye laser protruding
Added knockback to swords
Added prototype left missile pod
Replaced missing meshes and materials on the pod's arm's elbow
Replaced duplicate meshes in the rest of the pod's arm as well as the pod itself
Cleaned up the pod deploying animation
Added animation sounds
Made missile pods compatible with Rocket and Bike Mode
Added missile firing controls and sounds
Added missile targeting control and reticle
Attached missiles to barrel interior that shrink and grow when launched
Modified missile flight parameters
Added missile explosion
Added right missile pod
Hooked up right missile pod animations
Added right pod barrels to the list of missile firing slots
Fixed missiles exploding on launch when lagging
#### 1.28:

Converted eyes to UIX display
Screen is now scalable
Changed blush to slashes instead of hexes
Converted emote selection icons to UIX
Removed duplicate materials
Fixed head guns raydriver sometimes disabling itself
Replaced remaining hull seams with blender meshes
Added second set of emotes accessed by ending touch on left trigger while emote selection is open
Added dynamic variable for facecam feed
All particles now have alpha fade
Beam hit effect now fades to dark blue
Removed front face from screen mesh
Adjusted face UIX canvas to be flush with screen mesh
Added visual ping effect to screen tap
Added hidden screen menu toggle button
Set up screen menu keypad
Interior of screen now renders for pilot while removed
Fixed screen text being the wrong material
Updated boot up changelog
Added support for LocalGravity dynvar
Added keypad to screen menu
Added internal compartment to head mesh behind screen
Replaced screen menu button toggle with slidable antenna
Antenna now retracts when re equipping screen
Replaced screen remote keypad with d-pad
Added scrollable options to screen remote
Fixed socket internals de-rendering too early on screen callback
Rotated eye cameras 90 degrees
Added custom icons to screen menu keypad
Set up dynamic variables for screen menu modes
Added home menu to screen tablet
Added reparenting menu to tablet
Hooked up tablet buttons to selection dynvars
Prototyped dynamic cursor for reparenting menu
Tried to dynamically generate reparenting menu, needs work
Implemented first bit of functionality to tablet mode, drone settings menu. Currently allows he pilot to toggle LocalGravity adherence and Global UI
Added silent mode to setting menu, turns off join/leave notifier sound
Added HUD icon for head guns
Added HUD icon for missile pods
Added HUD icon for screen removal
Added HUD icon for minigun
Multitool fingers now shrink on arm retraction
Treads raycast distance now adjusts for scale
Added viseme drivers to antenna rotation
High five now applies knockback to users below .25 scale
Multitool now accepts grip strength in accordance to custom controller bindings
Join/Leave notifier is now centered on the user that triggers it
Added reticle to screen in turret mode that uses an eye manager
Modified turret reticle parameters
Added reticle and loading to emote wheel
Added small eyes icon to emote wheel
Face cam world variable is now internally driven to prevent dereferencing
Added prototype shield wall creation to left hand, hold trigger in shield mode to paint, release to bake the wall in place
Shield wall now paints from entire shield rather than only the center line
Shield walls can now be painted using either hand (but not both at once)
Shield walls can now block raycasts
Shield walls are now given character colliders on bake
Added joint visuals to finger segments
Modified all hand transformations to better accommodate the new joints
Removed away material from all parts
Drone now boots up as long as it is no more than 3 slots under the user root, rather than only while a direct child
Added emote icons for loading and reticle
Added distance display to user trackers
Added zoom vision activated by touching the left side of the screen
Eye cameras now telescope forward while zooming in
Moved zoom in viewport behind HUD
Fixed missiles sometimes coming from root
Most recently fired missile pod now reloads after a short time instead of waiting for the next one to fire
Added a hand root slot to prevent held items from shrinking wildly
Added Drone Power to tablet mode settings menu
Added ability to hotswap between rocket and bike mode (without kicking off any passenger)
Head guns can now be deployed in rocket mode by touching right secondary and pressing left trigger, and retracted with left grip
Modified sword knockback to ignore the hit user's scale
Drastically decreased power of sword knockback
Head guns raycaster now turns on/off properly
Added mouth opening/closing to Compact Mode transformation
Arms now properly fold into chest for Compact mode
Fixed head rapidly exploding while not piloted
Added inventory thumbnail icon
Fixed Bike/Rocket hotswap not working correctly
Focusing a different world now properly shuts the drone down
Added a snap plane to the screen
#### 1.29:

Fixed screen going dark if active user doesn't have a RustyTalkingLights dynvar
Fixed head guns firing a silent shot when deploying
Fixed all grabbable parts somehow becoming scalable
Fixed Bitbot somehow becoming scalable
Fixed entire drone somehow becoming scalable
Chest now rotates into compact mode properly
Head tread no longer vanishes when retracting
Converted screen cursor from mesh to UIX image
Changed paint mode material tip parts from default to wireframe
Rotated finger parts in devtip mode
Fixed anchor space clear leaving an item behind
Changed timing of tracking offset change in compact mode
Baked missile mesh
Shortened lifetime of laser blast effect
Added Turk face snapper
Head guns now hold their fire while left trackpad is touched, allowing for missile lock on while deployed
Bitbot antenna now wiggle while talking
Bitbot can now override hearing and speaking sources
Velocity cancel now keeps a tiny percentage of speed instead of fully zeroing out
Bitbot antenna now only wiggle while voice source is transferred
Beams are combinable into a single larger beam
Legs now extend while in an anchor that has valid foot positions
Added the ability to reparent to a users root slot by looking at them
Moved Attach option from Bitbot submenu to Misc.
Fixed self reparenting conflicting with suit mode
Added sloppy eye snappers
Improved combination beam visuals
Added head to modularity
Fixed torso staying behind when drone shuts down
Fixed torso staying behind when activating suit mode
Redid Bitbot enter/exit animation so they now enter/exit from a panel in the back of the drone's head
Moved thruster anchor on head to bottom chassis plate so it no longer clips when mouth opens
Added plasma tether left hand option
Fixed plasma tether building downwards momentum in the held user
Fixed plasma tether visuals activating when they shouldn't
Added plasma tether to the right hand
Releasing plasma tether now retains the targets velocity
Fixed the right plasma tether target selection raycast coming from the left hand
Fixed plasma tether lightning meshes using the incorrect transform spaces
Added electrical zapping sound to plasma tether
Added engine rumbling sound to bike mode
Fixed plasma tether sound continuing to play after releasing while targeting self
Modified pilot detection such that the avatar can be up to two slots below the user root on boot, fixing failed startups while in culling systems
Changed left hand menus to wireframes from outdated unlit holograms
Cleaned up logic for left hand back menu, removing fps and ping tracker and changing the trigger for setting TargetedUser
TrackingOffset is now calculated on feature activation rather than being a flat value
Replaced Bitbot seam with blender mesh
Added dynamic variables for railgun support: missile pod tween references, slot references, head gun slot references, and railgun anchor slot
Altered lightning mesh generation of tractor beam hands
Touchtips are now usable in compact mode
Face cameras now extend with left b button capacitive touch
Bitbot Multitool swarm organization is now more optimal
Fixed right shoulder Bitbot not becoming non-persistent in idle mode
Updated power core meshes, the sides are now inset so they can plug in to the chest cavity properly
Bitbot now retrieves power core in a reasonable amount of time if it is far away
Bitbot now returns in a reasonable amount of time when exiting dronecam mode
Removed the empty hand requirement for opening quick menu
Added more variables and new logix for railgun attachment
Improved minigun deploying animation
Centered Facecam camera BECAUSE APPARENTLY IT'S BEEN MISALIGNED THIS WHOLE TIME
Added cover panels to inside of head gun openings
Modified thruster particle meshes to be a reasonable size
#### 1.30:

Replaced Chest section of quick menu with Cloud
Removed chest storage slots
Added cloudspawning capability
Drone can now cloudspawn a Bitbot multitool
Drone can now cloudspawn a Bitbot blueprinter
Drone can now cloudspawn the Rusty Railgun
Modified railgun deploying and positioning animation
Fixed power core being permanently inactive after chest storage removal
Fixed power core struts being permanently inactive due to a misnamed variable driver
Updated the power core case mesh
Updated the power core screen mesh
Added top and bottom back panels to chest hull
Improved camera meshes
Added AWOOGA emote where cameras burst through and shatter face screen
Moved Sloppy eye snappers to camera lenses so they move with the camera's telescoping
Added variable control to Bibot's facing target and plasma tethers
Bitbot now grabs and moves railgun while deploying
Added a target slot DynVar for use in docking ports
Re-re-redid suit sizing variable and IT NOW WORKS PROPERLY
Fixed each button on left hand menu having its own font stored on it
Fixed user colors not reading properly due to leftover write node
Modified hand user variable to be more consistent
Added a “Match Scale” button to left hand menu
Added a monowire snapper to left hand.
Added a RustyZapPoint user variable to screen
Moved gizmo clear laser to face screen in Bitbot mode
Drone now prints images like a polaroid when taking finger photos
Committed blasphemy and converted eyes to skinned meshes
Redid emote system for blendshape control rather than shutters
Added heart eyes emote
Some emotes now have separate versions for Bitbot mode
Shoulder joint facing targets are now modular
Added a manual kill switch to reticles via the drone killing dynamic impulse
Added Rusty head snapper to bitbot
Added sound to leg deploying
Added panels on the bottom of the belly compartment for leg deploying
Added sound to rocket/bike mode transformation
Removed UIX button from face screen
Added physical touchbutton to face screen
Slowed down and impulse timeout’d the tap ping on face screen
Added sounds and adjusted timing of photo printing
Fixed missile pod arms spinning wildly
Added light cone to hand flashlight
Added a flashlight to Bitbot and gave that a light cone too
Lowered the brightness of Bitbot’s flashlight
Fixed screen sending signals to drone root instead of user root in tablet mode settings menu
Adjusted the MonoBrow emote
Added Grappling Hook hand transformations
Accidentally saved Sloppy's eyes in camera snappers
Suit mode now checks for talking lights before default color
Removed Sloppy’s eyes from snappers
Added Grapple finger animations for both hands
Added Cannon animation to left hand
#### 1.30:

Updated Changelog
Modified scale on hexagons on back of both hands to match literally every other hexagon produced by Rusty Manufacturing
Added Teleport button to targeting menu
Added right and left tether selection buttons to targeting menu
Removed teleport button from targeting menu
Added Match Scale button to targeting menu
Added Holohands (stretchy arms)
Holohands now only activate when both hand modes are 0
Holohands have grab spheres and touchtips
Optimized Holohand meshes and materials
Fingers now scale to 0.01 instead of 0 when arms retract so Holohand fingers can move
Holohands now project from screen in Bitbot mode
Finally finished railgun retraction animation
Changed Bitbot eye mesh to match main screen
Added ActiveEmote dynamic variable to avatar space
Fixed Bitbot's eye being de-referenced from materialset component for flashlight mode
Fixed Bitbot's eye being de-referenced from playoneshot while retrieving power core
Fixed Bitbot gizmo laser radius being zero while retrieving power core
Mirrored MonoBrow emote to match with the two eyed version
Removed Weiner
Added Dink
Added Torso Lookat to settings menu to toggle whether or not torso faces head forward or hand average point
Added HUD icon for Torso Lookat
Shrunk materialtip orbslots during animation to fit in new hex on back of hand
Added Heart Emote Icon
Fixed Positioning of grab sphere on right Holohand
Attaching to a user now copies their talking lights if available
Thruster is no longer active in helmet mode
Touchtips now move with Holohands in Bitbot Mode
Added broken screen mesh for awooga emote
Some logix now disables when not needed: headguns aiming and firing, minimum aiming and firing, missile pod aiming and firing, all legs logix, beam combining, railgun
More logix disables when not in use: swords, shields, tethers
Plasma tether lightning meshes no longer smooth to size
Added eye snappers with new standardized tag “RingThing”
Added chest tracker
Added exosuit harness positioners
Separated exosuit target tracking logix from equipping signal receiver logix
More logix disables when not in use
Virtual parent now completely de-refs, saving a whopping ten frames while not in use
Fixed railgun button spawning a Bitbot instead of the railgun
#### 1.31:

Added functionality to grapple hands, now they shoot out with trigger and have very elastic swinging
Changed grapple reeling from touchpad capacitive to trigger sensitivity
Changed grapple reeling from trigger sensitivity to joystick forward/backward
Spent a good 4-5 hours going over the math for force while swinging, grapples now behave in a roughly ideal manner using both velocity canceling and gravity force canceling
Added Hooke’s law to grapple cables, they can now be reeled in again.
Clamped grapple direction dot product output to prevent the cable from pushing
Made grapple hands compatible with user scaling
Reduced grapple cable spring constant
Made grapple hands compatible with standard controller
Cleaned up hand variables for active user and chirality
Integrated power state logix into Boot Sequence
HUD now toggles with IsBooted rather than IsOn
Bitbot thruster and main thruster now toggles with IsBooted instead of IsOn
Removed the IsOn variable
Adjusted arm roots and snapper position to be at the shoulders instead of partway down
Adjusted crane snapper on head to match new positioning
Disabled a bunch of buster logix when not in use
Saving a user’s suit size successfully now has an associated sound
Grapple hands no longer use virtual parents, instead the local transforms are calculated with logix, solving issues with hitting oddly scaled objects
Screen has been changed from UIX to a stencil material, leading to accurate talking lights bloom and more possibilities for animation
Modified screen meshes to have an internal volume inside the front bevel where things can be displayed
Shattered screen is now the same stencil material, allowing the eyes to be seen through the remaining shards from the right angle
Added a mesh to act as the beveled edges of the shattered screen
Added a flat mesh to act as a backdrop for the stenciled objects, preventing some rendering issues
Eyes are now physical objects in the screen’s volume
Blinker cursor is now a box mesh
Blush now correctly copies Pilot Color variable and is set slightly in front of the eyes, giving a neat 3d effect
The changelog that scrolls on boot is now a text renderer, leading to a simpler animation at the cost of 40k tris because text renders apparently have to use a separate quad for each character
Replaced eye meshes with 3d variants
Replaced screen backside mesh
Further inset screen stencil backplate mesh to allow for a larger stencil volume
Re-implemented screen tap visual with a 3d mesh that expands
Tap ping visual now instances itself, allowing multiple to occur at once
Removed the screen antenna slider
Removed the last of the tablet mode menu logix
Fixed the screen socket not rendering at the correct times
Fixed the drone being able to tap its own screen
Loading animation is now recessed into the head if the screen is attached
Reticle meshes are now 3d and at different depths
Added a cover mesh for the inner part of the reticle so it can have additional depth
Added an edge backplate mesh to screen to prevent some odd render queue issues
Sword blade particles are now hexagonal
Sword slash particles now fade out properly
Added mode switching for left cannon hand
Added visual to cannon charge shot
Improved charge shot visual
Added projectile to charge shot
Charge shot now pulses a boost hex when firing
Improved projectile visuals for left charge shot
Added sounds to left charge shot
Added knockback to left charge shot
Removed left energy sword
Added telescoping blade to left hand sword
Changed left hand sword sound effects to reflect new more mechanical visuals
Upgraded sword deploying sound
Fixed sword applying knockback on deploying
Modified sword knockback strength
Added hitting sounds to sword knockback
Upgraded right hand sword to match left
Modified sword finger positions to make a more convincing hilt (bye bye classic Rusty sword silhouette)
Flashlight cone now properly disables on both left and and Bitbot
Sword now has lit-up edges
Removed decoy bodynodes
Fixed rocket/bike mode being disengaged by only the right grip instead of both
Fixed bike mode not being hooked up to thrusterlogix correctly, causing it to only boost when the left hand is closer to the thrusters than the right
Changed internal Quick Menu functionality so it now sends dynamic impulses rather than setting a variable for a split second. This allows for more optimized feature activation logix as well as the disabling of receivers when not in use.
Added X-Eyes emote (finally hooked up that blendshape)
#### 1.32:

Changed font from Orbitron to Tomorrow across all Rusty Manufacturing products
Upgraded shield from arbitrary floating hexagons to a proper mechanical projector
Buster and Cannon internals are now toggled in the animation rather than driven based on casing rotation
Rotated hand shield and shield collider
Adjusted shield fingers
Added sounds to mechanical shield
Moved force hex to Dataspace
Rotated shield drawing to match new hand shield rotation
Fixed shield failing to close when the collider has been deleted
Adjusted position of shields in turret mode
Adjusted position of shields in railgun mode
Increased shield collider radius
Cannon hand now resets selected mode when closing
Added Part Recall button to Misc submenu
Toggling off modularity no longer recalls loose parts
Added child save blockers to some snappers: both antenna, both eyes, goggles
Added clearing functionality to remove strokes from the screen's snap plane

---
#### 2.0 (Neos to Resonite Migration):

Fixed boot sequence not working because the color cloud variable was looking for G-Neos instead of G-Resonite
Fixed rocket/bike mode transformation not working because locomotion switching needed to be an Async task
Fixed force hexes appearing at y=0 on root while shield painting
Changed eye/screen stencil ID so it won't interfere with the islands in the default cloud home
Fixed materials being the wrong color due to migration: Orange, Grey, Lasers, Shields
Laser color is now driven by the Pilot Color variable
Fixed Minigun disappearing too quickly during closing animation
Fixed parenting bullets not deleting correctly if the thing they hit disables itself
Reworked headguns to be hopefully more consistent and definitely more optimized
Removed many unneeded Start Async Task nodes
Added DroneVersion dynamic variable
Drone name is now driven by the version variable
Fixed hand thruster audio continuing to loop when retracting while active
Fixed Missiles not moving towards target
Added knockback to missiles
Cleaned up ALL migrated logix: 
-Removed redundant Start Async Task nodes
-Replaced auto generated Indirect Write nodes with Write nodes where applicable
-Converted slot drives from refID to direct
-Cleaned up layout of all circuits
-Tweaked some animations to work better with the new flow style
-Optimized some math
Fixed changelog sticking on boot
Added joint lights to knuckles
Modified finger positions for all hand transformations to incorporate new joint lights
Re-added active user port to left palm
Active user port can now be node-copied from for the GetActiveUserSelf node
Modified energy barrier material
Added a second layer to the force hexes used in shield painting so they can have both channel matrix and intersect materials
Recalling Bitbot from camera drone mode now returns him to his shoulder slot rather than leaving him floating in front of the user
Modified meshes: All screen and screen socket parts are taller as part of a minor redesign, all chassis seams are merged with the panel they are on for reduced slot count and draw calls (forgot hands)
Photo printing animation is now slightly lower so it doesn’t clip through the now-taller screen
Fixed a bug where parts being recalled would snap to the correct rotation instead of animating smoothly
Fixed the cursor blinker not appearing because it had the wrong stencil ID
Scaled up loading animation for new screen size
Scaled up reticle for new screen size
Adjusted blush for new screen size
Updated inventory thumbnail icon
Replaced hand hull meshes
Added button to devtip to activate all gizmo options at once
Fixed dead references caused by the removal of the Variable Reader Refs slot
Fixed fingerpose setting using the wrong handposer for the left hand
Fixed user trackers searching for G-Neos color variable instead of G-Resonite
Replaced Drone antenna meshes with a mechanical assembly
Replaced Bitbot antenna meshes with a mechanical assembly
Revamped antenna circuit for the new assembly and made them more expressive by modifying the angles for each viseme
Replaced chest and hand hex lights with beveled versions
Updated all emote icons to match new screen size and blendshapes and to fix asymmetry
Moved reticle emote to lower left
Added ClosedHappy emote
Added Closed emote
Fixed gauntlet finger positions
Fixed gauntlets resizing hand hexes incorrectly
Replaced new antennae with properly scaled versions
Updated all emote icons with new antennae
Re-added RingThing snappers to antennae
Added childsaveblocker to new RingThing snappers
Updated Bitbot Multitool
Fixed parts animating to root if dropped mid-recall
Removed outdated camera zoom circuit
Re-added camera zoom circuit because it was actually for the telescoping of the physical lenses and not the HUD display thing lol oops
Left hand touchtip can no longer activate the targeting menu
Lowered brightness of hand flashlight to compensate for proper scaling on the palm hex
Updated tread meshes
Changed ActiveEmote variable to User/ActiveEmotes
Changed texture on light cones
Removed the continuous relay from the target tracking circuit

---
## 3.0 (Major Modularity Overhaul):

Added dynamic variables and parent values to support fully modular hands and arms
INTEGRATED VERSION 1.0 OF THE HAND MODEL REWORK
Changed how the quick menu sends signals, each circuit now only needs an impulse receiver to be toggled
Hand now has on-board multitool
Compact mode is now compatible with modular tween target references
Rocket mode is now compatible with modular tween target references
Added external slot savers to some parts of the hand's multitool
Reactivated swords, shields, and left grapple in old hands
Added a fist override variable to modular hands for forcing the fingers closed during some transformations
Hand now has on-board flashlight that reacts to talking lights
Gripping now sends reset signals (Left, Right, and both) to remove the need for per-circuit grip detection
Made all hand modules compatible with new reset signals
Turret mode now reparents modular hands
Moved all Tractor Tether functionality to drone hands
Moved shield functionality to hands (lacking hexpainting) and cleaned up the animation and collider circuits
Moved sword functionality to hands
Fixed right shield being positioned wrong when in turret mode
Fixed some hand circuits trying to turn off while already off
Added extendo grip to replace holohands
Made high five compatible with modularity
Moved grapple to modular hand
Replaced grab lasers with custom Bitbot beams
Bitbot grab lasers now replace holohands in compact mode (without the stretching for now)
Extendo grip now properly parents grab spheres
Moved all buster flux to modular hand
Restructured hand modules to hopefully be more self-contained
Overhauled how buster mode is handled (haha get it?)
Regained thruster functionality
Regained Repulsor functionality
Regained blaster functionality
Updated thumb meshes to remove the need for extra pivot slots
Updated hand panels to make future opening animations nicer
Fixed turret mode trying to set GauntletState variables that no longer exist
Rocket/bike mode now accurately engages modular thrusters
Removed all arm LookAt components and replaced them with a proper IK Flux circuit (wrists no longer disconnect at all while moving!
Replaced segment meshes and AxisAligner component with telescoping forearm blendshape mesh
Hands are now snapped to the ends of the arms rather than directly on the drone
Grab lasers now activate for physical grab if no hand is attached
ADDED NEW MULTITOOL GRIPPER that folds out of the hand panels quite pleasingly
Added tool arm to new multitool
Drone arms now straighten when not attached, and smoothly swap to IK transforms while changing state
Animated new multitool tool head swapping
#### 3.1:

New multitool now has sounds
Made material orb storage prettier
Made the arms transition to being deployed look cooler
Arms now read a parent value to determine if they should be deployed
Removed old arm retraction animation
Retracting an arm now also activates that side’s fist override
Grab Spheres and Finger Dots are now more consistently in the right place
Added fluxtip tool head
All tool heads now react to trigger strength
Improved arm retraction animation
Arms now disable while both are fully retracted
Added sounds to multitool head switching animation
Turret mode now reparents and tweens the drone’s hand targets instead of the dynamic hand values
Rocket mode and bike mode now reparent and tween the drone’s hand targets instead of the dynamic hand values
Buster mode is no longer toggleable through the menu to prevent disabling when hotswapping rocket/bike mode
Sword mode now opens the hand’s front panels
Optimized rocket mode locomotion flux a bit
Added tractor tether mechanism animation to new hand
Changed how multitool visuals enable/disable
Updated chest hull, chest front panel, shoulder plate, shoulder panel, shoulder swivel, and wrist swivel meshes
Elbow tracking is now slightly smoothed courtesy of ShadowX
Added new rudimentary buster animation!
Added telescoping segments to fingers
Fist override now retracts the fingers slightly and folds the thumb up completely
Replaced middle hand panel mesh with properly offset hex
Improved buster animation
Multitool and buster circuits now disable when not in use
Regained (some) beam functionality
Rocket and turret mode now properly activate hand busters
Adjusted turret mode buster positions
Removed old left hand parts because apparently they were still there
Fixed multitool color pallet not deploying due to being turned off
Adjusted pen tip activation threshold and pressure smoothing for cleaner lines
Added grabbale joints to antennae
Yanking either antenna like a lever now causes the Drone's eyes to roll like a slot machine
Fixed power core energy connections
Changed power core energy connections from weird garbage circuit to ParentValueLink slots
Modularized power core
Made power core retrieval animation compatible with modular version
Turret mode now reparents the power core socket instead of the core itself
Hands and arms now respond to the Chirality ParentValue bool instead of being written to by nearest user hand
Updated part recall circuit to disable grabbable on a part while animating to prevent it from flying to origin
Re-added dynamic tween references to hands
Fixed antenna lever crank sound only coming from the right ear
Adjusted how the material orb storage slots retract
Dynamic hand reference is now cleared if that hand is attached to the opposite side, which fixes grab spheres and finger dots being stuck to the wrong hand (and maybe some world crashing behavior? We’ll see)
Shield animation circuit now uses async sequences instead of if node mazes
Adjusted shield animation to better fit new hand panels
Adjusted shield positions in turret mode
Minigun spinning no longer stops driving its audio, hopefully preventing it from being silent on the first deployment in a session (didn't)
Added new head panels to make compact mode animating smoother
Made compact mode animating smoother
Changed multitool tool head swapping sound
Reimplemented cloudspawning button with more consistent functionality
Cloudspawning now uses resrec URLs instead of resdb
Cloudspawning button now stores itself in Dataspace while not in use
Added new tether hook variables to Railgun
Updated Railgun materials
Reimplemented Railgun
Cloudspawning is now done via string cloud variables instead of direct URLs
Bitbot now holds himself upright relative to the drone
Cleaned up Railgun animation circuit a bit
Buster beam now emits a hex loop on overdrive again
Added sky twinkle effect to rocket mode
Fixed materials on new head panels
Fixed incorrect neck reparenting when disengaging suit mode
Turned an unnecessary division node into a multiplication because I'm an optimisation nut
Hand modules now have their own plasma materials
Grapple is now underhanded and has a basic hook mesh
Hand snappers no longer tilt awkwardly when retracting
#### 3.2:

Reworked arms retracting animation so shoulder panels fold instead of slide and the FistOverride and IsDeployed variables get set with proper timing
Added cloudspawning receiver circuit that teleports spawned items infront of the drone
Added cloudspawning signal senders to hand, arm, power core, Bitbot tool
Arm extending/retracting now has sound
Fixed cloudspawned items being teleported with the wrong coordinate space conversion
IsWaitingForObject variable is now reset after receiving an object
Foot claws are now a modular part that can attach to hand snappers
Replaced legs with arm snappers
Reworked leg deploying/retracting animation to work with new modular parts
Legs and feet are now modular
Legs and feet save with avatar for now (auto-populating cloudspawning on boot to come later)
Updated leg deploying/retracting animation to better accommodate new modular versions
Finally fixed buster beam sounds, visuals, and knockback effects
Finally added a tool head to the multitool’s pen mode
Adjusted thruster sounds so they can be heard from farther away for greater cinematic effect
Bitbot grab lasers are now lightning meshes
Modified cloudspawning system so a set of dynamic variables now populate with the most recent item URLs on boot rather than requesting the URL every time an item is spawned, saving significant time
Requesting item URL status is now shown on the HUD immediately following booting
Added variables for where or not individual arms are attached and a RustyOutfit snapper to the chest for Rusty Suit Jacked compatibility (thank you Amplified!)
Added RingThing snapper to Bitbot for his little bowtie
Added childsaveblocker to the new snappers and also the main hat snapper
Added the ability to spin hands about the wrist by touching the lower thumb button and not the upper thumb button. Trigger strength on the opposite hand then controls speed
Hand spinning sound changes to an alarm if flashlight mode is on
Added the User/LightsColor variable for colored lights that don't change while talking
Hand plasma color is now driven by User/LightsColor with User/RustyTalkingLights as a fallback
#### 3.3:

Tether raycast point reference no longer breaks when decoupled from the hand
Updated hand mesh with 1mm chamfered edges on the palm
Updated pen tool head mesh to have like 8 fewer polygons lol
Pilot color is now determined by primary cloud color with default user color as a backup
Decoupled anchor space initializer from the main boot sequence circuit
Decoupled head animation from the main boot sequence circuit
Decoupled radial localizer from the main boot sequence circuit
Decoupled pilot color setter from the main boot sequence circuit
Decoupled locomotion initializer from the main boot sequence circuit
Decoupled drone power establisher from the main boot sequence circuit
Chirality of detached hands now swap to the most recent grabber
Pilot color is now tweened on boot instead of instantly swapped
Fixed the range of boosting sound not actually being extended
Added support for cloudspawning Bitbot Blueprinters (after finally fixing those too, yay!)
Fixed some boot sequence flux
Chirality of detached arms now swap to the most recent grabber
Fixed the multitool being equipable via laser reeling-in the hand
The drone’s torso now rotates to face the average of the hand positions again, but in a way that makes sense this time
Torso rotation circuit now handles the spinning of the torso for rocket/bike mode
Torso rotation circuit now respects the IsBooted variable
Busters now change modes with a “Gunshift” system that works like a gear shift rather than spamming context menu
Updated some quick menu buttons: Modularity is now its own submenu with Toggle as the first option, Recall Parts is now in the Modularity submenu, Arms is now Retract Arms, removed both hands’ Cannon buttons in preparation for charge shot functionality in the main busters
Part Recall now sends a signal to each part so they can reparent and tween themselves
Only parts with the appropriate tag will sync to the modularity system when attached
Added tags to parts: RustyHand, RustyArm, RustyPowerCore
Hands now respect the TargetedUser variable when in suit mode
Rebuilt missile functionality from scratch to use a master async circuit rather than instancing a driving circuit per projectile
Missiles now visibly emit from within the barrel rather than a meter or two in front  
Missiles now fly straight for 10 meters before curving towards their target
Missile pods are no longer on smooth transforms
Adjusted some of the new missile parameters
Removed the childrensaveblocker on the legs as a bandaid fix until they auto-populate
Added a tie snapper
Moved more quick menu buttons around: swapped positions of the Modularity and Bitbot submenus
Modularity mode can now be toggled even while arms are retracted
Fixed the talking lights material on the power core connectors being wrong
Fixed power core tether point variables being wrong
Renamed an old “Logix” slot to “Circuitry” under the user tracker template. That should be the last one!
Organized Bitbot’s power state detection so he now properly shuts down when tabbed out of a world
Bitbot’s smooth transform value is now written to, preventing him from slipping out at high speeds
Organized the entire Rocket/Bike mode transformation circuit
The Rusty Hover locomotion module now controls the specifics of changing between rocket/bike and fly/walk, leading to faster and more consistent transforming
The Rusty Hover locomotion module now handles hot swapping between Rocket and Bike mode
Reworked how the torso facing direction is controlled to make animating it spinning and setting it to always forward easier
Torso spinning on boot up is now an intended feature
Torso no longer spins on shutdown
Fixed torso not spinning when hot swapping between Rocket and Bike modes
Added the RustyDrone/RustyUIVisibility variable
Gunshifts are now labeled
Gunshifts provide haptics when toggling between options
Re-selecting the current mode with the Gunshift no longer causes a redundant transformation
Gunshift now starts at the current mode
Fixed minigun sound not playing during first deployment
Holding jump while flying now causes vertical ascension
Fixed minigun not being aimable in rocket mode due to a broken reference
Turret mode now forces the torso to face forward for easier aiming
Minigun now flips out in a more interesting way during turret mode transformation (no clue what made that the case but I’ll keep it lol)
Left hand button now refreshes user trackers again
Fixed locomotion speed not being reset when hotswapping out of bike mode
#### 3.4:

Fixed force application mode in the locomotion not being set properly when hot swapping from bike to rocket
Modified user join/leave indicator to be a generic notification system
A notification now pops up when the pilot is reparented that displays the new parent space
Left hand multitool HUD elements now display below the right hand’s
Buster HUD elements now display below battery indicators
Fixed buster progress bar UI appearing outside of thruster mode
Moved hand back button from back hex to its own slot so only the hex is the button rather than the whole chassis
Legs no longer retract on shutdown if a pilot is still present
Moved some screen circuits from the main processor to the screen itself
Vertical force in flight mode is now applied based on head direction rather than up relative to the local space
Bitbot smooth transform is now relative to the local space while docked
Eye cameras now have a render transform override
Moved reticle control components from screen circuitry slot on the main processor to screen dataspace
Removed vestigial cursor slot from the emotes menu
Gunshift no longer appears in rocket/bike mode
Upgraded finger meshes (including thumb) to now have pads on the tips, better joints, and more obvious telescoping segments
Modified fist override to accommodate new finger meshes
Modified finger paint job
Hands now retract further into the arm to accommodate new fistoverride
Wrist rotation now behaves correctly when retracting arms
Reticles now show correct global distance regardless of the drone’s scale
Fixed thruster sound priority
Shortened new metacarpal struts
#### 3.5:

Cloudspawning button now instances itself so spawning multiple items can be done in parallel
Arms, hands, legs, and feet can now auto-populate
Added a Populate Parts button to the modularity submenu
Added childrensaveblockers to leg snappers
Cloudspawn button now queues entries and processes them every two calculation cycles, allowing mass part requesting
Fixed head gun laser material being incorrect
Adjusted resolution of facecam
Prepared drone for automatically attaching hand modules
Prepared hand functions for conversion to spawnable modules with debug functions
Converted Tractor Tether to a cloud spawnable module
Converted Sword to a cloud spawnable module
Converted Multitool to a cloud spawnable module
Converted Shield to a cloud spawnable module
Converted Grapple to a cloud spawnable module
Converted Flashlight to a cloud spawnable module
Converted Buster to a cloud spawnable module
All modules delete themselves when retracted
Modules can be stacked on the left hand
Fixed multitool animating incorrectly
Turret mode now requests busters and shields from the cloud
Rocket mode now requests busters from the cloud
Busters now react to the drone being in rocket/bike mode and turret mode
Extendo grip is no longer enabled during rocket/bike mode or turret mode
Wrist spinning is no longer enabled during rocket/bike mode or turret mode
Modified how the hand modules detect being attached
G.R.A.P.P.L.E. module now has unique visuals
G.R.A.P.P.L.E. module now has unique sounds
Added DRM (Duplicate Rusty Mitigation) to spawnable parts
Repopulating arms and hands no longer retracts an arm if it’s fully operational
Added new sound to beams
Shields now animate properly in railgun mode
M.I.S.S.I.L.E. System is now a spawnable module
Locking on to a user with the hologram menu while missile pods are deployed will redirect the missiles to that user’s hips
Added RustyDrone/PlasmaColor variable
Added RustyDrone/LaserColor variable
URL setting clipboard is now cloud spawnable (recursion)
#### 3.6:

Fixed tooltip unhider stealing tooltip holders (hopefully this prevents structural support Bitbots)
Boost visual is now twice as big in rocket mode
Adjusted boost sound to be heard slightly further away and added a new variant for extra long distances
Shoulder panels no longer animate if no arm is connected
Speedometer is now more accurate
Left visor button now displays additional information on the HUD
Added Local Space to HUD
Added Local Axis to HUD
Added distance and direction to local origin to HUD
Added Home Slot display to HUD
Adjusted positioning of notification display on HUD
Adjusted positioning of loading messages on HUD
Reorganized M.I.S.S.I.L.E.S. animation circuit
Upgraded targeting laser on M.I.S.S.I.L.E.S.
Upgraded targeting laser on G.R.A.P.P.L.E.
Upgraded targeting laser on Minigun
Reorganized dynamic variables
Adjusted G.R.A.P.P.L.E. beam sounds
Adjusted tread smoothing
Reworked tread rotation behavior
Upper arm now extends/retracts based on distance to arm point
Added a screen retraction/deploying animation
Added new text to boot sequence
Replaced changelog scrolling with proper boot sequence flavor text
Eyes now animate when booting
Reworked screen to be a modular part
Grab lasers, gizmo beam, and screen flashlight are now under a Utility Visuals slot in Dataspace
Reworked screen socket visibility
Reworked camera zooming
Reworked emote controller
Reworked variable handling for facecam render texture
Added LITE screen that only exists when the drone is spawned
LITE screen now gets seamlessly replaced when a proper screen is cloudspawned
Separated all 16 emotes into separate receiver circuits on board the screen
Moved modular screen to the second section of the part recall circuit
Screen is now included in the modular repopulation feature
Fixed whisper bubble being disconnected from voice mode
Fixed voice modes not working (broadcast, shout, etc)
Disabled grab laser lightning meshes when not in use
Fixed left brow raising slower than right due to automatic order offsets in the emote controller flux
Fixed screen reappearing too soon after shatter emote causing clipping with the cameras
Replaced user tracker system with new world data feed components for optimization and to allow the creation of trackers while culled
User trackers now use the cloud color of the targeted individual if possible
Added hinge and backplate model to screen socket
#### 3.7

Fixed whisper bubble being 500 times too big
Fixed voice modes not updating properly while the controlling component was disabled
Eyes now switch to a random emote each type they cycle by during the slot machine bit
Adjusted positioning of local axis indicator on HUD
Bitbot now copies torso rotation as well as position
Bitbot antenna movement is now controlled by dynamic variables
Began preliminary preparations for a Bitbot modularity pass
Thumb rotation now acts as the size adjustment knob for the multitool pen
Reworked Bitbot power state animation to be more reliable
Adjusted thruster particle circuit to lower random direction when ascending quickly
Main thruster particles now have ribbon trails when moving faster than 20m/s
Grab spheres no longer reparent to hand, instead hand interaction points can extend and spin silently to match the visuals
Interaction lasers and equipped tools can now spin and extend
Adjusted positioning of grab lasers and utility flashlight
Grab lasers and utility flashlight now emit from the chest if Bitbots are not visible
Removed user tracker cleanup circuit since the bug that caused it to be required was fixed
Added point light to G.R.A.P.P.L.E. hook
Modular parts can now be ejected
Recall now notifies all synced arms (including legs) which then recall their respective hands (including feet)
Fixed loading screen not being properly inset after screen modularity pass
Added point light to tractor tether
Fixed recall not affecting hands if its arm is attached
Recall eligibility checking is now handled entirely on the part
#### 3.8

Reticles now show days since registration
Replaced B.U.S.T.E.R. model with v3.0
Adjusted thumb plate position when fist override is engaged
Animated new B.U.S.T.E.R. and replaced sound effect
Modified rocket mode thruster positioning to account for new B.U.S.T.E.R. shape
Repositioned VFX to account for new B.U.S.T.E.R. shape
Modified beam mode (which is in bad need of a rework)
Added segment mesh struts to new B.U.S.T.E.R.
Animated new B.U.S.T.E.R. Struts
Localized face HUD display camera (remember later to delocalize it when in broadcast mode)
Anchor Release is now an integrated control activated by pressing both grips while jumping
Delocalized face HUD display while in broadcast mode
Hex loop in B.U.S.T.E.R. can now be emitted dynamically
Gunshifts behave a little worse now (oops)
Beam is now mode five
B.U.S.T.E.R. now has charge shot capability as mode four
Charge shot can be fired as pellets or held for up to five seconds to accumulate a large blast
G.R.A.P.P.L.E. now respects talking lights
Charge shot now respects talking lights
Hand flashlights now have sound and the palm hex extrudes out while active
Shoulder panels no longer have seams on the inside
Chest hull now has a separate lower panel