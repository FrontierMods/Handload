# Reference

## Formulae

- **bullet damage**: `sqrt(muzzle_energy)`, as per the base game, where

  - `muzzle_energy`: energy of the bullet immediately upon exiting the muzzle, in joules

- **sectional density** (if not provided): `weight / 7000 / diameter ^ 2`, where

  - `weight`: weight of bullet (in grains)
    - division by 7000 is a conversion factor to pounds (lbs); if bullet weight is given in lbs, use `weight` instead of `weight / 7000`
  - `diameter`: diameter of bullet (in inches)
    - for expansive bullets, the diameter of final expansion is used
      - if diameter of final expansion is not available, multiply bullet diameter by 1.8 for modern rounds (2010+) and by 1.45 for older rounds
  - _[source](https://bulletin.accurateshooter.com/2021/06/sectional-density-of-bullets-what-you-need-to-know/)_

- **armor penetration**: `sqrt(muzzle_velocity * sectional_density)`, where

  - `muzzle_velocity`: muzzle velocity of the bullet (i.e., velocity immediately upon the bullet leaving the barrel), in m/s
  - `sectional_density`: density multiplier (see above)
