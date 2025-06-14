# HUD/Center
The centre area shows important tactical information.

## 

Contents

- 1 HUD Mode
    - 1.1 Combat Mode
    - 1.2 Analysis Mode
- 2 Target Information
- 3 Target Hologram
- 4 Compass
- 5 Heat Indicator
- 6 Scanner
- 7 Speed Indicator
- 8 Ship Hologram
    - 8.1 Ship Status Indicators
- 9 Power Distribution
    - 9.1 Systems
    - 9.2 Engines
    - 9.3 Weapons
- 10 Signature
- 11 Fuel
- 12 Misc Indicators
- 13 Comms
- 14 Info
- 15 Proximity Indicators

## HUD Mode

Chapter Four (3.3) of *Elite Dangerous: Beyond* separated combat and certain scanner functions into two modes that the player can toggle between. Each mode has a specific set of functions.

### Combat Mode

Combat Mode is the default HUD Mode for a ship. It is signified by curved orange brackets on either side of the HUD. Combat Mode must be active in order to deploy and fire weapon hardpoints.

### Analysis Mode

Analysis Mode allows use of the Discovery Scanner, Full Spectrum System Scanner, Detailed Surface Scanner, Pulse Wave Analyser, Data Link Scanner, and Short Range Composition Scanner. It is signified by straight blue brackets on either side of the HUD. When active, in addition to allowing scanners to be used, it highlights planets and moons with a holographic grid.

## Target Information

Displays textual information on the current target, such as their name, ship type, and currently targeted subsystem. If no target is selected then information on the system is displayed.

## Target Hologram

Shows a holographic image of the current target.

The following information is provided by the hologram:

- Orientation relative to ship
- Shield strength
    - Displayed as three blue circles for full shields and reduces to three red for downed shields
- Hull health
    - Displayed underneath the target ship model
- Position of incoming damage
    - Displayed as flashes of light on the hologram

## Compass

The white circle marker indicates the position of the target relative to the ship's current heading. If the marker is a solid white then the target is in front of the ship and if the marker is an outline then the target is behind. The Compass turns blue when the ship is lined up for a hyperspace jump to another system.

The compass will point towards any of the following:

- Targeted Hyperspace destination
- Targeted celestial
- Allotted Docking Bay pad
    - For stations this only works once the ship is inside the docking ring
- An escape vector

## Heat Indicator

Displays the current temperature of the ship (as a percentage). Once the ship reaches 100% heat it will begin to take damage. Normally heat is radiated away from the ship through vents, however there are still a few ways that a ship can overheat - flying too close to a star, Silent Running mode which will stop the ship from emitting heat will cause the heat to build up inside the ship, or using too many heat inducing modules too quickly (such as continual boosting followed by FSD activation). Under normal conditions, the heat vents of a ship will be able to keep a ship's heat manageable - though, in some situations the pilot may want to use a (previously equipped) Heatsink Launcher to cool the ship. Upgrading the ship's Power Plant can also help keep the ship cooler when in heat intensive situations.

## Scanner

Scanner Icons
| Type | Meaning |
| --- | --- |
| Red | Hostile |
| Orange | Neutral |
| Green | Friendly |
| Grey | Cargo or FSD Wake<br> |
| Blue | Wingmate |
| Purple | Ship hostile towards Wingmate |
| Flashing White | Firing weapons at Player |
| Square | Hard-points Retracted |
| Triangle | Hard-points Deployed |
| Solid Icon | NPC |
| Outlined Icon | Player |
| Flickering Yellow | Unresolved Contact |
| White Triangle | Deployed Mine/Missile |
| Red Circle | Thargoid Interceptor |

Displays contacts and signals in the surrounding area. Objects are displayed depending on their position to the player's ship. Contacts are shown in various colours and shapes, indicating information about each contact. All signals are resolved once their signature strength exceeds a certain sensor threshold. Signature strength is determined based on distance to the signal and its emitted heat. The scanner can be switched between linear and logarithmic mode, in logarithmic mode the area nearest to the ship is magnified to provide more resolution on the relative positions of object nearby.

The yellow marker in the gauge directly underneath the edge of the scanner circle shows the current scanning range. The scanner range is smaller if the marker is towards the left-hand side and at its maximum when set to the far right. By default the scanner range can be changed by pressing `Page Up` to decrease range and `Page Down` to increase range.

The lines connecting the ship markers to the flat plane of the scanner show whether a detected object is above or below the current plane of your ship. If the line is drawn upwards towards a marker then the object is above the player's ship, and conversely if it is drawn downwards then the object is below the player's ship. If the ship is in Supercruise then the planet or star icons will be shown. Some objects may appear in supercruise. 

## Speed Indicator

The speed indicator displays many things and can be one of the most important gauges when manoeuvring. 

- The current speed is displayed at the top as a number (normal speed measured in m/s; faster in FSD)
- The horizontal bars indicate how fast the ship is moving relative to its normal maximum speed (note that it is possible to temporarily go faster than the normal maximum by boosting)
- The moving horizontal line represents the current throttle
- The blue section indicates the optimal turning speed - try to keep the throttle within this zone to make tight manoeuvres

## Ship Hologram

Shows a holographic image of your ship.

The following information is provided by the hologram: 

- Orientation relative to ship
- Shield strength
    - Displayed as three blue circles for full shields and reduces to three red for downed shields
- Hull health
    - Displayed underneath the target ship model
- Position of incoming damage
    - Displayed as flashes of light on the hologram

### Ship Status Indicators

 	 	 	 		 			 		 		 		 			
Ship status indicators
 		 	 

When the player's ship, or the ship that the player has currently targeted, takes certain types of damage (whether from a modified or standard weapon) the ship HUD will indicate this via the display of weapon effect icons shown below the relevant schematic for the affected ship.

| Icon | Description | Effect | Sources |
| --- | --- | --- | --- |
|  | Corrosion | The Hull is reduced by 20 points and incoming damage is increased by a quarter. | Corrosive Shell |
|  | Engine Disruption | Speed is reduced: changing ENG pips has no effect on the ship's max speed nor boost speed. | Drag Munitions |
|  | Engine Reboot | Temporarily disables thruster | Ion Disruptor, Thargoid Caustic Generator explosion |
|  | FSD Reboot | Temporarily disables FSD | FSD Interrupt, Containment Missile Powerplay weapon, Shift-Lock Canister |
|  | Hull Breach | Significant damage is directly dealt to modules | High-Yield Shell |
|  | Impulse Attack | Physically pushes the affected ship out of its previous trajectory. A Cannon with Force Shell can push the ship further with physical force. | Railgun, Force Shell |
|  | Increased Emissions | Increases the affected ship signature which makes the ship much easier to detect and generates heat faster | Emissive Munitions |
|  | Internal Damage | The ship can experience internal module damage | Overheating, Missile Racks (both dumbfire and seeker), strike on internal modules |
|  | Malfunction | A module will malfunction, regardless of the module's health.
<br>YELLOW ICON: a low chance that a malfunction will occur. <br><br><br>RED ICON: a malfunction becomes active. The Red icon is visible while receiving continuous weapon fire.<br> | Scramble Spectrum, Pulse Disruptor |
|  | Mass Locked | Increases FSD charge time from the default 5 seconds to over 1 minute. This does not affect the Hyperdrive | Mass Lock Munition |
|  | Regeneration | Without frequent hull damage, the Shield Generator will recharge at a rate of 1000+ | Concordant Sequence, Regeneration Sequence (two weapons only apply to teammates) |
|  | Sensor Disruption | The ship may experience reduced Sensor range and weapon target lock interference with decreased reliability. | Dazzle Shell, Seismic Charge explosion |
|  | Shield Breach | The Hull is directly damaged, regardless of shield power | Phasing Sequence, Thargoid Scout weapons |
|  | Shield Cell Cascade | Shield Cell Bank is damaged, and the shield restoration rate is reduced | Feedback Cascade |
|  | Shield Generator Attack | Directly damage the shield | Station Defence Turret, Reverberating Cascade |
|  | Shield Reboot | Temporarily disable the shield | Unknown |
|  | Target Interference | Target lock is lost | Target Lock Breaker |
|  | Targeting Overload | Turreted and gimballed weapons are scrambled. It reduces the target tracking efficiency | Dispersal Field, Thargoid Titan Field |
|  | Thermal Attack | The ship will experience a rise in heat | Plasma Accelerator, Thermal Cascade, Thermal Shock |

There is also an external ship status called "Hazardous Substance Detected" which often occurr as a replacement of "Internal Damage". This status effect only occurr which chances. It have a red grade-five material icon.  

## Power Distribution

Displays the current power distribution between the ship's three capacitors - Systems (SYS), Engines (ENG), and Weapons (WEP). Energy in each capacitor is filled based upon how many pips are allocated to that capacitor.

There are 6 pips ^(12 halves)^ that can be distributed at any time between the three capacitors by pressing the `Left Arrow` for Systems, `Up Arrow` for Engines, `Right Arrow` for Weapons, or `Down Arrow` to reset the pips to 2/2/2 ^(4/4/4 halves)^. Each capacitor can be allocated a maximum of 4 pips ^(8 halves)^ which will cause them to regenerate at maximum speed and a minimum of 0 pips which will cause them to not regenerate at all.

Each capacitor can store a maximum amount of energy determined by the ship's Power Distributor. When power is expended (either by shooting, regenerating shields, boosting, etc.) it then begins to regenerate back to maximum capacity at a rate determined by how many pips are allocated to its capacitor.

Players can view what capacitor each module draws from in the ship's right control panel under the Module section.

### Systems

### Engines

Boosting draws energy from this capacitor. A boost can only be activated if there is a sufficient amount of energy stored. Pips in this capacitor will influence the ship's maximum speed, optimum manoeuvrability range, and top boost speed.

### Weapons

Weapons and some scanners draw energy from this capacitor. Pips in this capacitor will allow weapons to cool faster thus reducing overheating problems.

## Signature

The waveform in the heat signature display indicates how much heat the ship is emitting to space. A flatter waveform means less heat is being emitted, therefore it will be more difficult for the sensors of other ships to detect the ship's signature. When Silent Running is switched on the waveform will be replaced with blue "Silent Running" text.

## Fuel

The ship's fuel information is displayed here as a number, a thin line, and a segmented bar.

The number displays how much fuel (in tons) the ship is currently using per hour - so 0.22/h means that the ship will consume 0.22 Tons of fuel every hour at the current rate. Note that the number changes based upon how fast the ship is moving and if it is in supercruise or in normal space.

The thin line displays the current running fuel that the ship has - consumed when in supercruise or normal space. The segmented bar (although for ships with fuel capacity of 16 tons or more it is displayed as a solid line as well) displays how much fuel is in the ship's main fuel tank and is predominantly consumed when performing Hyperspace jumps.

## Misc Indicators

There are three sections here : Mass Locked, Landing Gear, and Cargo Scoop. When the state is active the box will light up, and when inactive (default state) it will be your UI's default colour. The "FSD Cooldown" indicator is also displayed there for a short time after exiting supercruise.  

- Mass Locked - Lights up when the ship is too close to a large object that is disrupting its ability to use the FSD.
- Landing Gear - Lights up when the landing gear is deployed. Must be deployed when landing at a station or a planet in order to complete the docking/landing procedure. Top speed will be limited while the landing gear is deployed.
- Cargo Scoop - Lights up when the cargo scoop is deployed. Top speed will be limited while the cargo scoop is deployed.

## Comms

Comms are where the player can communicate with other players and where messages from NPCs will be displayed.

## Info

The Info section displays notifications about the status of your ship, other nearby ships, and bounty related activity. Icons for proximity and impact warnings will show up here, as well as indicators for the ship's headlights.

## Proximity Indicators

The two elongated panels (with red lights in them) flash red or yellow as proximity and impact prediction alerts. These panels may be in a different location or have a different shape depending on the ship's type.