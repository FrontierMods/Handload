# Reference

## Ballistic Performance

### Range

Range for a cartridge is calculated as a distance at which the bullet it houses still retains around 260 ft·lbs (≈ 352.5 J) of energy, based on the bullet's mass, muzzle velocity, and ballistic coefficient (BC). This particular value was chosed based on [ammoman], because it provides a clean value to measure against.

Because _Cataclysm: Dark Days Ahead_ only models a "reality bubble" of around 60 in-game units of distance, we always clamp a larger value to 60.

The value from calculations based on desired energy is measured in meters, which does not cleanly correspond to game's internal units of distance. Barring a more-appropriate method, we consider the meter-based approach a good-enough approximation of a round's effective range in game terms.

Sources:

- [ammoman] https://www.ammoman.com/blog/9mm-effective-range/
