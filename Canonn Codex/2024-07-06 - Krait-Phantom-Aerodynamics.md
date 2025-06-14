## Krait Phantom Aerodynamics

Published: 06 Jul 2024 on Canonn (https://canonn.science/codex/research-notes/krait-phantom-aerodynamics/)

Content: The Krait Phantom is a medium ship manufactured by Faulcon DeLacy. The Phantom is a variant of the Krait MkII which is more focused on multirole capability over being a fighter. It has found a niche as a great medium sized exploration vessel. The following reference quantities were used when performing the analysis for the Krait Phantom. Additionally, diagrams of the Krait Phantom’s geometry and presumed CG used in the analysis are provided. All gifs shown below can be found here:https://imgur.com/a/ndeWYjD

| S\_ref (Reference Area) | 698.5678 m^2 |
| --- | --- |
| b\_ref (Reference Span) | 72.0000 m |
| c\_ref (Reference Chord) | 73.2275 m |

Reference Values

| CG\_x | 39.1008 m from leading edge |
| --- | --- |
| CG\_y | Ship centerline |
| CG\_z | 9.5608 m from bottom-most surface |

![](https://canonn.science/wp-content/uploads/2024/07/image-840x1024.png)CG Approximation Diagram

![](https://canonn.science/wp-content/uploads/2024/07/image-1-1024x639.png)Isometric View

![](https://canonn.science/wp-content/uploads/2024/07/image-3-1024x318.png)Full View

## Lift and Drag

The Krait Phantom is a very interesting looking ship and one that doesn’t hint at strong aerodynamic performance. While it’s top profile is rather sleek much like a swept wing fighter of the 20th century, it’s front and side profile reveals a rather bulky frame. It has decent lift production in the subsonic and transonic regimes but the sharp drag rise in the transonic regime kills its lift-to-drag ratio. Accelerating into the supersonic and hypersonic regime, the Krait Phantom struggles to produce lift. Oddly enough, it would be better off flying upside down in this regime, it’s flat top would act as an ideal lifting surface at higher speeds, as shown by the lift curve. As expected, the forward pointing side antenna are exposed to strong flow fields and throw strong shocks of their own, as seen in the Mach sweep graphic below. These antenna structures need to be very strong to not only survive the brunt force of the aerodynamics, but also any aerodynamic heating that would be experienced on planetary entry as well as vibrational loads due to vortex sheading from their cylindrical form factor.

![](https://canonn.science/wp-content/uploads/2024/06/image-1-1024x616.png)Lift, Drag, and Aerodynamic Efficiency Characteristics

![](https://canonn.science/wp-content/uploads/2024/06/KraitPhantom_MachSweep.gif)

## Pitch Stability

For the selected CG, the Krait Phantom is unstable in pitch, especially in the subsonic and transonic regimes. The vehicles struggles in the transonic regime, as indicated by the difficulty in obtaining a converged solution. The blunt aft-end paired with the many interacting shock surfaces resulting in a complex flow environment that could lead to buffeting. All that said, in the transonic and subsonic regime, the Krait Phantom does trim at around 0°-1° angle of attack aerodynamically so with an active control system it shouldn’t be too challenging to control the trim of the vehicle in these flow regimes. However, at supersonic and hypersonic regimes, the sloped bottom surface result in positive pitching moments all the way to around -10° angle of attack. This could mean a Krait Phantom going through planetary entry at a high angle of attack, common for reentry, could suddenly flip out of control without an adequate control scheme. This could be mitigated by entering at a lower angle of attack, but then the negative lift would pull the vehicle deeper into the atmosphere more quickly, resulting in even more heating.

![](https://canonn.science/wp-content/uploads/2024/06/image-2-1024x616.png)Pitch Stability Characteristics

- ![](https://canonn.science/wp-content/uploads/2024/06/KraitPhantom_Subsonic_AlphaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2024/06/KraitPhantom_Transonic_AlphaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2024/06/KraitPhantom_Supersonic_AlphaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2024/06/KraitPhantom_Hypersonic_AlphaSweep.gif)

## Yaw Stability

Generally speaking the Krait Phantom is slightly unstable in yaw although it could be considered neutrally stable. This was likely helped by the bottom two strakes which do act as small vertical stabilizers, however their severe dihedral limits their effectiveness.  As expected from its flat shape, the yawing moment coefficient is around an order of magnitude smaller than the pitching moment. As such, any control system that can handle the pitch would likely be able to handle the yawing moment if properly placed. The Krait Phantom is a bank-to-turn airframe.

![](https://canonn.science/wp-content/uploads/2024/06/image-3-1024x616.png)Yaw Stability Characteristics

- ![](https://canonn.science/wp-content/uploads/2024/06/KraitPhantom_Subsonic_BetaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2024/06/KraitPhantom_Transonic_BetaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2024/06/KraitPhantom_Supersonic_BetaSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2024/06/KraitPhantom_Hypersonic_BetaSweep.gif)

## Roll Stability

The Krait Phantom is shown to be stable in roll, with the rolling moment having a similar magnitude as its yawing moment. In interesting feature here is the rolling moment is almost independent of Mach number up until the hypersonic regime where it loses effectiveness. More work would have to go into finding what surface are being shielded in this regime that is causing the difference. 

![](https://canonn.science/wp-content/uploads/2024/06/image-4.png)Roll Stability Characteristics

- ![](https://canonn.science/wp-content/uploads/2024/06/KraitPhantom_Subsonic_PhiSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2024/06/KraitPhantom_Transonic_PhiSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2024/06/KraitPhantom_Supersonic_PhiSweep.gif)
- ![](https://canonn.science/wp-content/uploads/2024/06/KraitPhantom_Hypersonic_PhiSweep.gif)

## Conclusion

The Krait Phantom, a utilitarian variant of the Krait MkII, shares many of the same fighter-like outer mold line (OML) traits but unfortunately these traits do not particularly make the vehicle a great utilitarian airframe. Being unstable in pitch and yaw would require an advanced control scheme to aid the pilot, especially at entry speeds. Like many other spacecraft studied in this series, the Krait Phantom features some potential shock-on-shock risks. In this case, its the forward arms that extend out past the cockpit. However, it was observed that at Mach 5, the shock angles from the arms were not interfacing with the cockpit shocks in such a way as to create deadly shock-on-shock interactions as seen on other vehicles. It should still be monitored carefully however since the whole cockpit/arm region is rife with complex flow environments that could show issues at higher Mach numbers not yet tested. The primary concern for the author would be the antenna/sensor pylons. They are very high fineness structures which inherently mean they are weaker in bending moment, at the tips are highly loaded aerodynamically due to being blunt cylinders. During entry they would experience very high heating and at slower speeds they would likely vibrate. Being a cylinder in cross flow they could shed vortices in such a way as to be a perfect example of a Kármán vortex street

![](https://canonn.science/wp-content/uploads/2024/07/KraitPhantom_Copy_Scalar-Pretty-Picture.png)Krait Phantom in Flight