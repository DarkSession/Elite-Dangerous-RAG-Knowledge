## Type-7 Transporter Aerodynamics

Published: 18 Nov 2023 on Canonn (https://canonn.science/codex/research-notes/type-7-transporter-aerodynamics/)

Content: The Type-7 Transporter is a large ship manufactured by Lakon Spaceways. It was designed as a dedicated freighter and it’s iconic shape has led many to compare it to a brick. Due to this informal designation, it was not expected that the Type-7 Transporter would be in any way aerodynamic, even considering its laughably stubby wings. The following reference quantities were used when performing the analysis for the Type-7 Transporter. Additionally, diagrams of the Type-7 Transporter geometry and CG used in the analysis are provided. All gifs shown below can be found here: https://imgur.com/a/mLbIwgN

| S\_ref (Reference Area) | 789.5374 m^2 |
| --- | --- |
| b\_ref (Reference Span) | 56.1250 m |
| c\_ref (Reference Chord) | 81.5611 m |

Reference Values

| CG\_x | 42.3117m from leading edge |
| --- | --- |
| CG\_y | Ship centerline |
| CG\_z | 17.5088m from bottom-most surface |

![](https://canonn.science/wp-content/uploads/2023/11/Type7CG-1024x308.png)CG Approximation Diagram

![](https://canonn.science/wp-content/uploads/2023/11/image-1-1024x718.png)Isometric View

![](https://canonn.science/wp-content/uploads/2023/11/image-3-1024x684.png)Vehicle Diagram

## Lift and Drag

Based on the shape of the Type-7 Transporter, and its stubby “wings” it was expected that it would have poor lift performance in line with other “lifting body” type designs. Additionally, the boxy shape of the Type-7 Transporter has led many to lovingly refer to it as a flying brick. This alone is a good indication that it was expected the Type-7 Transporter would suffer with resect to drag too. Looking at the Type-7 Transporters “wings”, it was found that they have no camber and are effectively flat plates with semi-sharpened/shaped leading edges. This type of shape is typically seen on hypersonic vehicles to protect the leading edge from extensive heating, but at the cost of poor lift performance. Additionally, the body shape of the Type-7 Transporter includes a heavily angled “forehead” which causes the lift curve slope to shift the zero-lift point to roughly 2° at subsonic conditions and up to 7° for hypersonic conditions. To put it another way, this heavily angled surface causes a large amount of downforce on the vehicle until the angle of attack is large enough to either shield it or expose enough of the flat bottom surface to counter it. This shift is reflected in the drag curve as well. 

To compare the claims that the Type-7 Transporter is a brick, CFD was performed on a UK standard size brick. As shown, the UK standard brick had substantially lower lift-to-drag than the Type-7 Transporter, as well as significantly more drag. As such, it is the author’s opinion that referring to the ship as a brick is unfair to the ship, at least in terms of lift and drag aerodynamic performance.

![](https://canonn.science/wp-content/uploads/2023/11/image-7-1024x617.png)Lift, Drag, and Aerodynamic Efficiency Characteristics (Type-7 Transporter)

![](https://canonn.science/wp-content/uploads/2023/11/image-8-1024x618.png)Lift, Drag, and Aerodynamic Efficiency Characteristics (UK Standard Brick)

![](https://canonn.science/wp-content/uploads/2023/11/Type7Transporter_MachSweep.gif)Type-7 Transporter

![](https://canonn.science/wp-content/uploads/2023/11/Brick_MachSweep.gif)UK Standard Brick

## Pitch Stability

Right away it is observed that the Type-7 Transporter is unstable in pitch, a surprising characteristic for a dedicated freighter. Typically, the most stable types of airframe are those dedicated to passenger and cargo transport as they tend to trade maneuverability in exchange for cargo volume and safety. As indicated by the static margin, it is arguably neutrally stable in pitch which is what is usually seen on vehicles with higher maneuverability requirements (see the Alliance Chieftain) but still trends on the side of instability. This inherent instability comes from the highly angled forehead seen on the ship. As shown in the pitching moment curves, practically across the board the Type-7 Transporter has a nose down pitching moment, due to the loading on that angled forehead. Except at subsonic speeds, the vehicle is unable to aerodynamically trim and even at subsonic speeds it is at approximately 7° angle of attack. The thrusters on the Type-7 Transporter will have to compensate for this in atmospheric flight.

Interestingly, the UK standard brick is stable in pitch at subsonic and transonic speeds, but becomes unstable, to about the same degree as the Type-7 Transporter, at supersonic and hypersonic speeds. Granted the pitch stability only exists between -5° and 5° at subsonic speeds. So once again the comparison between the Type-7 Transporter and a brick is unfounded. At least in some cases the brick is stable. 

![](https://canonn.science/wp-content/uploads/2023/11/image-9-1024x615.png)Pitch Stability Characteristics (Type-7 Transporter)

![](https://canonn.science/wp-content/uploads/2023/11/image-11-1024x615.png)Pitch Stability Characteristics (UK Standard Brick)

- ![](https://canonn.science/wp-content/uploads/2023/11/Type7Transporter_Hypersonic_AlphaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2023/11/Type7Transporter_Subsonic_AlphaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2023/11/Type7Transporter_Supersonic_AlphaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2023/11/Type7Transporter_Transconic_AlphaSweep.gif)

## Yaw Stability

When looking at the Type-7 Transporter from the side, it was assumed it would be unstable in yaw due to lacking any vertical stabilizers and the data agreed with this assumption. In fact, the vehicle is just as unstable if not more so in yaw as it is in pitch. It is believed this is mostly due to the lack of vertical stabilizers as mentioned but also due to the relative central location of the CG. If the CG was further forward, the large flat side surfaces on the Type-7 Transporter might have been enough to keep the craft stable in atmospheric flight. Once again this is an odd choice for a dedicated freighter vessel. At least due to the asymmetry of the craft it is trimmed at 0° sideslip, but due to the instability the flight control system will have to constantly work the thrusters to keep it pointed in the right direction.

Due to the similar shape of the brick in the pitch plane and in the yaw plane, the characteristics observed in yaw stability are basically identical to what was seen in pitch stability. So once again, the brick is at least aerodynamically stable some of the time.

![](https://canonn.science/wp-content/uploads/2023/11/image-12-1024x615.png)Yaw Stability Characteristics (Type-7 Transporter)

![](https://canonn.science/wp-content/uploads/2023/11/image-13-1024x615.png)Yaw Stability Characteristics (UK Standard Brick)

- ![](https://canonn.science/wp-content/uploads/2023/11/Type7Transporter_Hypersonic_BetaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2023/11/Type7Transporter_Subsonic_BetaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2023/11/Type7Transporter_Supersonic_BetaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2023/11/Type7Transporter_Transconic_BetaSweep.gif)

## Roll Stability

Due in large part to the high CG location on the Type-7 Transporter, it was found to be unstable in roll across all flight conditions. The saving grace here, is unlike other ships that have been analyzed to date, the Type-7 Transporter is at least consistent in its instability. This would make it easier to design a proper flight control system. However, to put it simple, the brick was found to be stable.

![](https://canonn.science/wp-content/uploads/2023/11/image-14.png)Roll Stability Characteristics (Type-7 Transporter)

![](https://canonn.science/wp-content/uploads/2023/11/image-15.png)Roll Stability Characteristics (UK Standard Brick)

- ![](https://canonn.science/wp-content/uploads/2023/11/Type7Transporter_Hypersonic_PhiSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2023/11/Type7Transporter_Subsonic_PhiSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2023/11/Type7Transporter_Supersonic_PhiSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2023/11/Type7Transporter_Transconic_PhiSweep.gif)

## Conclusion

It was not expected that the Type-7 Transporter would be a particularly aerodynamic ship and the analysis performed indicated that the initial assumptions were correct. The large flat surfaces pointed directly into the flow result in a large drag coefficient. That said, the drag is not as high as one might think thanks in part that a large piece of the frontal area is angled back. This makes the Type-7 Transporter roughly 40% less draggy than a UK standard brick at the same flight conditions. It was also found that despite being a dedicated freighter, the Type-7 Transporter is unstable in pitch, yaw, and roll due in part to its assumed CG location but also due to its lack of horizontal or vertical stabilizer surfaces. As an example, the UK standard brick was found to be pitch and yaw stable at slow speed and small angles which is due solely to the CG being placed at the center of the brick compared to the Type-7 Transporter’s offset CG. This is shown once again with roll stability since the brick is stable in roll across the board while the Type-7 Transport is not, due in large part to its high CG but also its low “wing” placement. Typically dedicated freighter airframes will have high wings or, if they can not due to other design requirements, low wings with dihedral since these types of wings add to the roll stability of the airframe.

During the runs it was noticed that there was a large pressure load on the front of the canopy due to its location. Unlike other ships analyzed to-date, the canopy was either angled  (reducing the aerodynamic loading) or further aft to sit behind the main vehicle shock. In the case of the Type-7 Transporter, the canopy is the cause of the main vehicle shock and its vertical glass components take a substantial pressure load. As shown below, it was found the large central window covers 76.232 square feet and at Mach 5 the average pressure coefficient (Cp) on the window is 1.7132. Assuming that there is 1 atmosphere of pressure (~14.7 psi) on the inside of the ship, the table below shows the force acting on this single pane of glass. As shown, in typical space flat, the glass has to withstand 81 short-tons of pressure force pushing outward. However, at Mach 5 flight in a 0.01 atm pressure, this outward force is reduced to 56 and at a 0.1 atm pressure it has increased to over double (169 short-tons) the force pushing inward. It is highly recommended that Lakon continue to perform extensive quality control on their cockpit glass panels and double check their calculations along the attachments points. Glass does very well in compression and could easily withstand these loads. However, once mounted in a frame, the load transfers from the glass to the structure by putting the glass in tension, a state it is not very strong in. 

| Atmospheric Pressure<br>[atm] | Atmospheric Pressure<br>[psi] | Dynamic Pressure<br>[psi] | Outside Pressure<br>[psi] | Inside Pressure<br>[psi] | Force Inward<br>[short ton] |
| --- | --- | --- | --- | --- | --- |
| 0 | 0 | 0 | 0 | 14.6959 | -81 |
| 0.01 | 0.1470 | 2.5718 | 4.5530 | 14.6959 | -56 |
| 0.1 | 1.4696 | 25.7179 | 45.5295 | 14.6959 | 169 |
| 1 | 14.6959 | 257.1791 | 455.2952 | 14.6959 | 2418 |

Overall, the Type-7 Transporter is not a very good airframe and comparing it to a brick is unfair to the brick, at least in regards to stability, but it does have the advantage of being consistently unstable. This would allow for proper flight control systems to be written fairly easily allowing even inexperienced pilots fly this ship. That said, advanced training would still be highly recommended due to the airframe’s instability. While a proper flight control system could keep the pilot out of trouble most of the time, without the pilot understanding the potential risks the ship could be put into an unrecoverable situation very easily. Additionally, while the Type-7 might have significant drag, as long as its engines can overcome this force it becomes a non-issue except in the regard of in-atmosphere fuel economy, which should not really be considered here since the ship can effectively drop into the atmosphere right over its intended target and should not be performing long range freighter flights in-atmosphere.

![](https://canonn.science/wp-content/uploads/2023/11/Type7Transporter_Scalar-Pretty-Picture.png)Type-7 Transporter in Flight

![](https://canonn.science/wp-content/uploads/2023/11/Brick_Scalar_-_Pretty_Picture.png)UK Standard Brick in Flight