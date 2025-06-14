# Stellar Forge
Cobra logo
 		 	 

The **Stellar Forge** is the system used to generate the roughly 400 billion star systems which are present in the 1:1 scale Milky Way galaxy in *Elite Dangerous*.^[1]^^[2]^

The Stellar Forge is part of the cutting-edge Cobra development platform. Frontier Developments has made its own state-of-the-art in-house proprietary engine technology and development tools since 1988. All Frontier’s games are developed using their proprietary Cobra cross-platform technology.^[3]^

The lead physicist in the creation of the galaxy using the Stellar Forge was Dr. Kay Ross. She was tributed with nebula Dr. Kay's Soul.

## 

Contents

- 1 Newsletter #36
- 2 Integration with real-life data
- 3 Quirks
- 4 Videos
- 5 References

## Newsletter #36

The Elite Dangerous Newsletter #36 has an in-depth explanation:^[4]^

> 
> 
> In Elite Dangerous, when we are generating a system procedurally, each planetary system is formed from first principles. Bodies are gradually aggregated over a very long simulated time from available matter, taking into account its chemical composition. Depending on the angular momentum, this might begin to form into a single central body, or into multiple co-orbiting bodies.
> 
> 
> As the gases collapse together under the force of gravity, matter tends to orbit these bodies in protoplanetary discs, which in turn further coalesces into smaller bodies within those discs. Tidal forces, orbital resonances and gradual accretion of mass gradually change their orbits, causing collisions, collapse and close encounters – which in turn means bodies might capture each other or fling each other into new orbits or out of the system altogether.
> 
> 
> At some point the stars in the system ignite one by one, and the resultant stellar winds gradually drive off the lighter non-gravitationally bound gases.
> 
> 
> Over its lifetime (different for different systems) close and not so close encounters with other stellar systems may remove outer planets and capture others, and the outer halo of comets and other bodies may pass through the other system, not just causing destruction, but also depositing lighter elements and compounds (like ice/water) on the bodies in the inner system that may have been lost during the heat of their formative years, making water-based life there possible.
> 
> 
> The above processes are all modeled from first principles for almost all of our 400 billion star systems by an Elite: Dangerous system called Stellar Forge.
> 
> 
> There are some interesting outcomes from Stellar Forge that are ‘backed up’ by astronomical observations – for example binary planets. During the process of the system forming, both catastrophic collisions (as in the case of Earth) and very close encounters can result in bodies in very similar orbits capturing each other into a wonderful co-orbiting waltz.
> 
> 
> We see the early stage of this in the Solar system with the moons of Saturn, Epimetheus and Janus which share an orbit – swapping positions whenever they have a close encounter – but this is not stable in the very long term, particularly not in a gaseous disc where the gases are continually absorbing energy. In such a gaseous disc while planets are still forming and the corresponding slowing of the orbits, this is likely to end up with the bodies eventually co-orbiting each other in an ever less elongated orbit.
> 
> 
> Pluto and Charon are another example of an asymmetric binary planet (or dwarf planet as I think we should say these days), likely arising as a result of a close encounter or collision of an unknown body with Neptune, but then the pair eventually ending up orbiting each other, picking up other debris from the collision over time.
> 
> 
> We have seen pairs of gas giants in Stellar Forge, co-orbiting each other, each with its own stable moons. When standing on one of those moons you will see both gas giants looming large in the sky.
> 
> 
> Even pairs of earth-like planets are possible. In fact if one had life, then it is most likely both would, as meteorite impacts on one would tend to catapult debris to the other and spread the life across.
> 
> 
> Bodies can orbit each other very closely indeed. They can even touch – forming a strange dual body with a ‘figure of eight’ or hourglass shape – something predicted by a mathematician called Roche. We see this with stars too – an example of this is the contact binary i Boötis BC – already seen in the Elite: Dangerous Premium Beta.
> 
> 

## Integration with real-life data

Stellar Forge is intended to fill in the blanks of early 21th-century observation (cutoff date 2013), which generally only maps bright-enough stars and planets big enough to cause a dip in the light curve. The story of Trappist-1 is a good window into how SF works: without prior knowledge of the newly-observed star system, SF deduced from existing data that a pocket of mass sufficient to form a small star should appear close to the real-life location of Trappist-1. As a result, it generated a brown star system named Core Sys Sector XU-P a5-0.^[5]^

It is not uncommon for similar small stars to not be present in the Stellar Forge model. For example, Gliese 229, an interesting binary system with a red dwarf and a brown dwarf (plus two planets), is not found in the ED universe. Teide 1, the other prototypical brown star, also misses out. (The real-life distance data for Teide 1 is very poor, though the same cannot be said of Gliese 229.) Large gravitational models are after all chaotic, so getting the mass and element distribution close to real is all one should expect from any simulation.

The observed (non-procedual) part likely does not take into account the galactic rotation (see: Stellar kinematics). Given that only ~1300 years have passed, the changes in terms of galactic coordinates are not expected to be large. Polaris may no longer point to Earth north, but this is more due to the movement of the Earth and the Solar system.

## Quirks

Stellar Forge suppresses the generation of unusual star types (neutron stars, white dwarfs, black holes, blue stars, Wolf-Rayet Stars, and 10+ Solar Radii stars) close to the x, y, and z axes of the galaxy. The pattern results in a 100–300 ly gap visible on star-type maps generated by EDAstro.^[6]^ Apparently this was intended to only affect the bubble, but a typo crept in.^[7]^