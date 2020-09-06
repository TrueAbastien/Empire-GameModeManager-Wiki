# Purge, die die die.

* While friendly fire is active, this Gamemode punishes useless murder.
* Shooting your teammates or unarmed people may get you killed faster than expected.
* Slow-throwing grenades may result in your death or you victory.
* The MicroHID will have 'unexpected' results for victims with the right items in hand.
* SCPs can be slightly boosted (if need be).

## Configuration

### Death

Name | Type | Value | Constraints | Description
:---: | :---: | :---: | :---: | :------
ZombieOn049Death | bool | false | - | Respawn as a Zombie on SCP049 death.
LethalLarryBodyCount | int | -1 | Under 0 (to disable), Above or equal to 0 (to enable) | Requiered victims for 106 to become lethal.

### Factor

Name | Type | Value | Constraints | Description
:---: | :---: | :---: | :---: | :------
ShrinkHIDFactor | float | 0.75 | Between 0 and 1 | Factor of shrinking on HID.
GrowthHIDFactor | float | 1.25 | Above 1 | Factor of growing on HID.

### Limit

Name | Type | Value | Constraints | Description
:---: | :---: | :---: | :---: | :------
MaxScaleLimit | float | 3.0 | Above 1 | Limit of maximum scale factor.
MinScaleLimit | float | 0.5 | Between 0 and 1 | Limit of minimum scale factor.

### Luck

Name | Type | Value | Constraints | Description
:---: | :---: | :---: | :---: | :------
FriendlyExplosionLuck | double | 0.05 | Between 0 and 1 | Chances of exploding on friendly fire.
DefenselessStatusLuck | double | 0.1 | Between 0 and 1 | Chances of being cursed on defenseless kill.

## Commands

Name | Alias | Arguments | Permission | Description
:---: | :---: | :---: | :---: | :------
curse | gay | PlayerNickname | Mod | Give someone a random effect with infinite duration.
info | factor | ('all') | Mod | Display the info of the current Size Modifier Items.
reroll | roll, random, rand, r | - | Admin | Roll the items set to Grow or Shrink the player on MicroHID damage.

---

*latest update on 22nd of August 2020*
