## Type-9 Heavy Aerodynamics

Published: 23 Apr 2025 on Canonn (https://canonn.science/codex/research-notes/type-9-heavy-aerodynamics/)

Content: The Type-9 Heavy is a large ship manufactured by Lakon Spaceways. It is the largest dedicated trading ship and is often lovingly referred to as “The Cow”. While it lacks offensive and defensive capability, several “Battle Cow” builds exist. The Type-9 excels at trading and mining, as long as CMDRs can pilot it through the access corridors which can be challenging at times of high traffic. While the Type-7 Transporter is known as “The Brick” due to its flat front, the large frontal area of the Type-9 Heavy and low aspect ratio actually made for a more draggy ship. As one might expect, the Type-9 Heavy’s aerodynamics suffer in other ways. Diagrams of the Type-9 Heavy geometry and CG used in the analysis are provided. All gifs shown below can be found here: https://imgur.com/a/ATiNLYO 

| S\_ref (Reference Area) | 2158.6290 m^2 |
| --- | --- |
| b\_ref (Reference Span) | 115.2852 m |
| c\_ref (Reference Chord) | 117.4095 m |

Reference Values

| CG\_x | 53.6406 m from leading edge |
| --- | --- |
| CG\_y | Ship centerline |
| CG\_z | 20.6456 m from bottom-most surface |

![](https://canonn.science/wp-content/uploads/2025/04/image-18-808x1024.png)CG Approximation Diagram

![](https://canonn.science/wp-content/uploads/2025/04/image-19-1024x575.png)Isometric View

![](https://canonn.science/wp-content/uploads/2025/04/image-20-1024x368.png)Vehicle Diagram

## Lift and Drag

The shape of the Type-9 immediately leads us to believe it has poor aerodynamics performance. It’s frontal area alone is almost 3x the Type-7 and it has an incredibly poor aspect ratio, being almost as wide as it is long. In aerodynamics, there is something called the [Area Rule](https://en.wikipedia.org/wiki/Area_rule) which, in short, dictates the optimal area distribution for minimum drag in the transonic and supersonic regime. The Type-9 blows this clean out of the water and this is detailed in its performance. While at subsonic speeds it has less drag than the Type-9, in the transonic and faster regimes it has more drag then the “Brick”. With such poor performance, I am unsure how “the Cow” could ever jump over the moon. Well I guess there is no air in space, if you can make it out of the atmosphere. The heavily angled front pushes the min-drag point to larger angles of attack, which may actually be beneficial as the large pancake like shape of the Type-9 dictates it must flight at high angles of be aerodynamically effective, at least as effective as it can be. If you squint hard enough, the Type-9 does have a sort of airfoil shape which may explain its surprisingly good lift-to-drag ratio at subsonic speeds, but anything faster results in abysmal performance. 

![](https://canonn.science/wp-content/uploads/2025/04/image-1-1024x614.png)Lift, Drag, and Aerodynamic Efficiency Characteristics

![](https://canonn.science/wp-content/uploads/2025/04/Type9Heavy_MachSweep.gif)Type-9 Heavy Mach Sweep

## Pitch Stability

Like most ships analyzed so far, the Type-9 Heavy is unstable in pitch. For dedicates freights, good flight handling characteristics are a must with lesser stable craft used in a more nimble roll. It is again noted that the moments are directly dependent on the Center of Gravity location which is assumed for this and all analyses. As shown by the static margin, the Type-9 Heavy is close to neutrally stable, requiring the CG to shift 0.1 to 0.2 calibers (body lengths) forward to be purely stable. Like many craft with large angled upper sections on the front of the vehicle, the Type-9 has a almost always negative nose down pitching moment which is good at positive angles of attack, but less so at negative angles as it would just continue to diverge. This analysis was limited to 10° angle of attack but we do see the peak lift-to-drag likely is above 10° for everything above subsonic, and the pitching moment curves are trending upward. This could mean that the Type-9 could find a trim point near its maximum lift-to-drag which is ironically ideal. However it is still unstable and would require active control to keep it at this ideal glide condition through the atmosphere.  

![](https://canonn.science/wp-content/uploads/2025/04/image-2-1024x614.png)Pitch Stability Characteristics

- ![](https://canonn.science/wp-content/uploads/2025/04/Type9Heavy_Subsonic_AlphaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2025/04/Type9Heavy_Transonic_AlphaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2025/04/Type9Heavy_Supersonic_AlphaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2025/04/Type9Heavy_Hypersonic_AlphaSweep.gif)

## Yaw Stability

The Type-9 Heavy is neutrally stable in yaw, with a trend towards unstable. In reality, there is hardly any yawing moment, the same goes for the pitching moment. This indicates the CG is almost located on the Center of Pressure (CP) but is still slightly unstable meaning any perturbation to the pitch and yaw planes will cause the craft to continue spinning away from its original position. Advanced autopilots would be need to keep the craft stable, allowing the pilot to focus on flying while the computer keeps it in the air. The Type-9 Heavy lacks any kind of vertical stabilizer which would aid in restoring the perturbation from zero sideslip.

![](https://canonn.science/wp-content/uploads/2025/04/image-4-1024x614.png)Yaw Stability Characteristics

- ![](https://canonn.science/wp-content/uploads/2025/04/Type9Heavy_Subsonic_BetaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2025/04/Type9Heavy_Transonic_BetaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2025/04/Type9Heavy_Supersonic_BetaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2025/04/Type9Heavy_Hypersonic_BetaSweep.gif)

## Roll Stability

Unsurprisingly, due to its shape, the Type-9 Heavy has a larger rolling moment capability than it does yawing moment, at least at transonic speeds. Surprisingly, unlike many other vehicles studies thus far, the Type-9 Heavy is stable in roll, it naturally wants to fly flat as a pancake. This is likely due to the [dihedral](https://en.wikipedia.org/wiki/Dihedral_%28aeronautics%29) wing tips which increase roll stability in the subsonic and transonic regimes. Going into supersonic and hypersonic though, the shock shading removes this stabilizing affect and the ship becomes unstable in roll. The front view in the gif below for Hypersonic flow shows just how large the shock is around the blunt ship. Compare this to other more slender ships previously analyzed.

![](https://canonn.science/wp-content/uploads/2025/04/image-5.png)Roll Stability Characteristics

- ![](https://canonn.science/wp-content/uploads/2025/04/Type9Heavy_Subsonic_PhiSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2025/04/Type9Heavy_Transonic_PhiSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2025/04/Type9Heavy_Supersonic_PhiSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2025/04/Type9Heavy_Hypersonic_PhiSweep.gif)

## Conclusion

As shown above, the Type-9 Heavy is very unsteady in the subsonic and transonic regime, with large changes in flow behavior around the vehicle for small changes to angle. This could lead to buffeting behavior as it transitions from subsonic to supersonic flight, and visa versa. It also makes steady state solutions harder to obtain and may not fully capture the full risks of flying the Type-9 Heavy. The neutral to unstable nature of the ship in pitch and yaw is atypical for dedicated frights, which typically favor stability and comfort of flight over maneuverability. With little aerodynamic capability to recover, the Type-9 Heavy requires continuous active thruster control just to flight straight and level. It would not be recommended to fly the Type-9 Heavy for long durations in the atmosphere, it performs much better as an orbital hopper where air is no longer an issue.

Like the [Type-7 Transporter](https://canonn.science/codex/research-notes/type-7-transporter-aerodynamics/), which also has a forward located blunt windowed cockpit, the Type-9 Heavy has large high pressure zones right on the canopy glass. I won’t belabor the point again, see the other page for a more detailed analysis, but needless to say this is risky for the pilot.

![](https://canonn.science/wp-content/uploads/2025/04/Type9Heavy_Scalar-Pretty-Picture-2-1024x576.png)Type-9 Heavy in Flight