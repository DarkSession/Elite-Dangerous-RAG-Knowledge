## Mamba Aerodynamics

Published: 07 Feb 2024 on Canonn (https://canonn.science/codex/research-notes/mamba-aerodynamics/)

Content: The Mamba is a medium ship manufactured by Zorgon Peterson. They took an unreleased racing prototype and fitting it for use in the Pilots Federation, adding hardpoints but keeping its high speed. Its design is so unique compared to other ships, sporting sleek curved lines like imperial ships while sporting two massive engine clusters on either side of a rather small central section. The following reference quantities were used when performing the analysis for the Mamba. Additionally, diagrams of the Mamba geometry and CG used in the analysis are provided. All gifs shown below can be found here: https://imgur.com/a/4l9XjGC

| S\_ref (Reference Area) | 354.5144 m^2 |
| --- | --- |
| b\_ref (Reference Span) | 51.5342 m |
| c\_ref (Reference Chord) | 79.2187 m |

Reference Values

| CG\_x | 46.0507 m from leading edge |
| --- | --- |
| CG\_y | Ship centerline |
| CG\_z | 5.7441 m from bottom-most surface |

![](https://canonn.science/wp-content/uploads/2024/02/image-1-1024x279.png)CG Approximation Diagram

![](https://canonn.science/wp-content/uploads/2024/02/image-2-1024x652.png)Isometric View

![](https://canonn.science/wp-content/uploads/2024/02/image-4-1024x599.png)Full View

## Lift and Drag

The unique look of the Mamba immediately leads the observer to believe it must have strong aerodynamic qualities. Even without advanced degrees, humans are remarkably perceptible about identifying “what can fly” and “what can’t fly” due to our observations of flight going back to our earliest history. The wide flat planform of the Mamba lends itself to having one of the largest lift-to-drag ratios of the ships available to the Pilots Federation. Of course, this is speaking for lifting bodies not winged vehicles which can boast double digit lift to drag ratios easily. The Mamba’s streamlined thin shape also leads to it having the lowest drag of any ship analyzed to date. While it does have top to bottom asymmetries, the drag bucket is almost symmetric about 0° angle of attack due to the vehicle’s thin nature limiting the dimensional differences. The streamline nature leads to having sleek, sweep back shocks instead of the bow shocks seen on many other ships. The engine nacelles extending forward of the leading edge of the body do lead to interesting shock patterns which will be discussed later.

![](https://canonn.science/wp-content/uploads/2024/02/image-7-1024x613.png)Lift, Drag, and Aerodynamic Efficiency Characteristics

![](https://canonn.science/wp-content/uploads/2024/02/Mamba_MachSweep.gif)

## Pitch Stability

While the Mamba’s planform lends itself to a low drag, high lift to drag ratio vehicle, it is unfortunately incredibly unstable. Based on the approximated CG, which is located in the center of the thruster cluster, the large nacelles which extend far forward of the CG lead to a large pitch up moment. These surfaces are semi-efficient lifting surfaces and their large moment arm to the CG is what causes this. While the pitching moment curves are very well behaved, this highly unstable nature means the Mamba would be impossible to fly without fast acting and strong thruster input. Despite this, the Mamba is also one of the few vehicles that have been analyzed that can actually trim aerodynamically with the Mamba trimming around 2° angle of attack at slower speeds and -4° angle of attack at higher speeds. The only way to make the Mamba stable would be to shift the CG over 8 meters forward. Even though the CG is approximated, this large shift seems unreasonable and the CG is likely not this far forward.

![](https://canonn.science/wp-content/uploads/2024/02/image-9-1024x615.png)Pitch Stability Characteristics

- ![](https://canonn.science/wp-content/uploads/2024/02/Mamba_Subsonic_AlphaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2024/02/Mamba_Transonic_AlphaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2024/02/Mamba_Supersonic_AlphaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2024/02/Mamba_Hypersonic_AlphaSweep.gif)

## Yaw Stability

Like its pitch characteristics, the Mamba is also unstable in yaw however due to how thin it is compared to how broad it is, the yawing moment is two orders of magnitude smaller than the pitching moment. This would lead to the Mamba being a bank-to-turn airframe compared to a skid-to-turn airframe. The Mamba does sport two vertical stabilizers but these are laughably small for the ship’s size and do nothing to stabilize the yaw. All that said, the yaw characteristics are at least similar through the Mach range meaning that it should be easy to implement active control logic to keep the ship aligned to its flight path. In yaw at least, pitch is a different monster as previously discussed.

![](https://canonn.science/wp-content/uploads/2024/02/image-10-1024x615.png)Yaw Stability Characteristics

- ![](https://canonn.science/wp-content/uploads/2024/02/Mamba_Subsonic_BetaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2024/02/Mamba_Transonic_BetaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2024/02/Mamba_Supersonic_BetaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2024/02/Mamba_Hypersonic_BetaSweep.gif)

## Roll Stability

Despite being unstable in both pitch and yaw, the Mamba is surprisingly stable in roll. It’s rolling moment is about on par with its yawing moment, being trivial compared to the pitching moment. With everything else working against the Mamba from a stability perspective, and the fact that most ships have been unstable in roll so far, the Mamba shines as an oddity with stable roll characteristics pair with wildly unstable pitch and yaw characteristics. At least the thrusters won’t have to work to keep it at 0° roll.

![](https://canonn.science/wp-content/uploads/2024/02/image-11.png)Roll Stability Characteristics

- ![](https://canonn.science/wp-content/uploads/2024/02/Mamba_Subsonic_PhiSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2024/02/Mamba_Transonic_PhiSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2024/02/Mamba_Supersonic_PhiSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2024/02/Mamba_Hypersonic_PhiSweep.gif)

## Conclusion

As one might have expected from the Mamba, it sports the lowest drag of any ship analyzed so far, pointing towards its speedy nature. It would not be surprising if the Mamba can hold speed records in both space and in an atmosphere. Additionally its large flat skipping stone like shape lends itself to an efficient lifting platform for its vehicle class (lifting body). Unfortunately that’s about where its aerodynamic benefits end as it sports incredibly unstable pitch and yaw characteristics. Its pitching moment is one of the largest seen so far, just pointing towards how much lift the forward sticking nacelles have. This could lead to the Mamba flipping end-over-end if not properly actively controlled. Another issue was found as the higher Mach numbers were analyzed. As seen before in the [Alliance Chieftain analysis](https://canonn.science/codex/research-notes/alliance-chieftain-aerodynamics/), the Mamba has similar shock-on-shock interaction issues. The blunt body generates a bow shock as seen in the image below but this bow shock is impinged upon by oblique shocks coming off of the forward nacelles. Depending on how the two shocks interact, which would require more complicated unsteady CFD analysis, a lance of superheated air could penetrate the forward shock and hit the vehicle surface directly, leading to a heat lance effect that could melt through the hull. In the case of the Alliance Chieftain, it was thought this effect could burn off the external engine struts but in the case of the Mamba, this could result in two superheated jets hitting the hull right in front of the canopy, directly endangering the pilot, potentially thermally reconfiguring (melting) them in their seat. It is such the recommendation from this researcher that the Pilots Federation suspend Mamba atmospheric activities until more extensive analysis and/or wind tunnel testing can be performed.

![](https://canonn.science/wp-content/uploads/2024/02/ShockOnShock.png)Shock-on-Shock interaction from the forward nacelle to the body bow shock

![](https://canonn.science/wp-content/uploads/2024/02/Mamba_Scalar-Pretty-Picture-1.png)Mamba in Flight