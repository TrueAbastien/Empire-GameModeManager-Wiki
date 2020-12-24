# Purge, die die die.

* Shooting your teammates have a chance to make you explode.
* Shooting unarmed people may get you to be cursed with an inconvenient status effect.
* Slow-throwing grenades will make them explode instantaneously.
* The MicroHID may shrink, grow or kill its victims depending of the item in hand.
* SCPs can be slightly boosted (if need be).
* SCP-207 damage can be mutliplied.
* Killed players may respawn after being killed as a human Class and only after a few seconds.
* In-game rituals can be achieved by respecting very specifics and expensive conditions (see **Rituals** section below).

## Patches

* **SpeakingSCP:** All SCPs can now speak using their secondary vocal keybind.

## Configuration

### Death

Name | Type | Value | Constraints | Description
:---: | :---: | :---: | :---: | :------
ZombieOn049Death | bool | false | - | Respawn as a Zombie on SCP049 death.
LethalLarryBodyCount | int | -1 | Under 0 (to disable), Above or equal to 0 (to enable) | Requiered victims for 106 to become lethal.
CocaDmgMultiplier | float | 0.0 | Above 0 | Multiplier for damage caused by SCP-207 effects.
AutoRespawn | bool | true | - | Allow for auto respawn or not.
RespawnLatency | float | 15.0 | Above ~0.5 | Time before you respawn once you die.

### Factor

Name | Type | Value | Constraints | Description
:---: | :---: | :---: | :---: | :------
ShrinkHIDFactor | float | 0.75 | Between 0 and 1 | Factor of shrinking on HID.
GrowthHIDFactor | float | 1.25 | Above 1 | Factor of growing on HID.
~~RagdollForce~~ | float | 1.0 | Above 0 | Velocity multiplier at which body are thrown.
UspDamageFactor | float | 1.0 | Above 0 | Damage multiplier for any USP shot.

### Grenade

Name | Type | Value | Constraints | Description
:---: | :---: | :---: | :---: | :------
ModifiedBall | bool | true | - | Verify is SCP-018 is modified or not.
BallAmount | int | 7 | Above or equal to 1 | Amount of SCP-018 to spawn on normal throw.
NukeAmount | int | 10 | Above or equal to 1 | Amount of Grenade to explode on a SCP-018 slow throw.
NukeRecursiveDelay | float | 0.1 | Above 0 | Delay between each Grenade explosion.
NukeDelay | float | 0.01 | Above 0 | Delay between each Grenade explosion.

### Limit

Name | Type | Value | Constraints | Description
:---: | :---: | :---: | :---: | :------
MaxScaleLimit | float | 3.0 | Above 1 | Limit of maximum scale factor.
MinScaleLimit | float | 0.5 | Between 0 and 1 | Limit of minimum scale factor.

### Luck

Name | Type | Value | Constraints | Description
:---: | :---: | :---: | :---: | :------
FriendlyExplosionLuck | double | 0 | Between 0 and 1 | Chances of exploding on friendly fire.
DefenselessStatusLuck | double | 0.1 | Between 0 and 1 | Chances of being cursed on defenseless kill.

### Magic

Name | Type | Value | Constraints | Description
:---: | :---: | :---: | :---: | :------
MagicUspLuck | float | 0.0 | Between 0 and 1 | Chances of custom bullet depending on your USP modding.
MagicUspTutorial | bool | false | - | Auto magic USP for Tutorials (depending on modding).
MagicUspMask | int | 2047 | Between 0 and 2047 | Integer mask code for the USP magic effects.

## Commands

Name | Alias | Arguments | Permission | Description
:---: | :---: | :---: | :---: | :------
check | - | - | Mod | Verify if a ritual can be triggered at the sender position.
~~curse~~ | gay | PlayerName | Mod | Give someone a random effect with infinite duration.
info | factor | ['all'] | Mod | Display the info of the current Size Modifier Items.
reroll | roll, random, rand, r | - | Admin | Roll the items set to Grow or Shrink the player on MicroHID damage.
ritual | rituals | 'true'/'false' | Admin | Change the state of rituals to enabled or disabled.
uspmod | usp, mod, mods, uspmods | ['c'.'h'.'s'.'f'] | Mod | Change the modding of the USP in hand.
_check_ | - | - | User | List every ritual achievable nearby (if any).

## Rituals

By placing items in a circle, respecting constrainsts and following a specific guideline (for activation), 'rituals' can be achieved to trigger special in-game events.

Name | Items | Constraints | Activation | Effect
:---: | :-----: | :-----: | :-----: | :------
Awakening | *Each keycard in the game* **(12)** | Player must only have an SCP-500 in Inventory | Using an SCP-500 | A Player becomes invicible, taller, faster...
BlackHole | Keycard05 (x2), Flashlight (x2), GrenadeFlash (x2) **(6)** | There must be an SCP-106 | Placing an SCP-106 portal | Every human players in range will teleport to the lobby room and slowly die.
LightSwap | Flashlight (x3), KeycardJanitor, KeycardScientist, KeycardScientistMajor, Radio **(7)** | - | Slow throwing a Flash Grenade | Every player in range will swap its traits with another.
NutChild | SCP-500 (x3), Medkit (x3) **(6)** | There must be an SCP-173 | SCP-173 must kill someone | Every human players (alive) will be transformed in smaller SCP-173.
PocketCall | Radio (x4), Coin (x2), Flashlight (x2) **(8)** | Must be done in the Pocket Dimension | Having someone being disarmed | Will teleport the disarmed player and make him invisible (for the round).

**PS:** activation event must be triggered at the center after what the items used in the rituals will be consumed.

---

*latest update on 24th of December 2020*
