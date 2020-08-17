# DarkSouls, sadistic staff usually have a tendency for explosion.

Interacting doors, throwing grenades, shooting SCPs (or just shooting) can trigger an explosion. Being handcuff allow for invulnerability in exchance for possible immobility.

This Gamemode is highly configurable.

## Configuration

### General

Name | Type | Value | Constraints | Description
:---: | :---: | :---: | :---: | :------
SCPGrenadeResistance | bool | true | ~~none~~ | SCPs no longer take damage from grenade.
SCPTeslaResistance | bool | true | ~~none~~ | SCPs no longer take damage from tesla gates.
SelfExplosion | bool | true | ~~none~~ | Explosion doesn't damage other players.
CuffedResistanceFactor | float | 0.1 | Above or equal to 0 | Multiplier of any resistance for any cuffed personnel.
CuffedImmobility | bool | true | ~~none~~ | Force player to stay at the place they were cuffed.
ExplodingZombie | bool | true | *ExplodingSCP* must be **false** | Zombies creates an explosion whenever they take damage.
ExplodingSCP | bool | false | ~~none~~ | SCPs creates an explosion whenever they take damage.

### Luck

Name | Type | Value | Constraints | Description
:---: | :---: | :---: | :---: | :------
DoorExplosionChances | float | 0.1 | Between 0 and 1 | Chances of exploding on door interaction.
ShootingExplosionChances | float | 0.05 | Between 0 and 1 | Chances of exploding when shooting.
GrenadeExplosionChances | float | 0.5 | Between 0 and 1 | Chances of exploding on long grenade throw.

### Size

Name | Type | Value | Constraints | Description
:---: | :---: | :---: | :---: | :------
MinWidthScale | float | 0.6 | Above 0, Under *MaxWidthScale* | Minimal width a player can spawn to (as a multiplier).
MaxWidthScale | float | 1.2 | Above *MinWidthScale* | Maximal width a player can spawn to (as a multiplier).
MinHeightScale | float | 0.7 | Above 0, Under *MaxHeightScale* | Minimal height a player can spawn to (as a multiplier).
MaxHeightScale | float | 1.2 | Above *MinHeightScale* | Maximal height a player can spawn to (as a multiplier).
MinDepthScale | float | 0.5 | Above 0, Under *MaxDepthScale* | Minimal depth a player can spawn to (as a multiplier).
MaxDepthScale | float | 1.2 | Above *MinDepthScale* | Maximal depth a player can spawn to (as a multiplier).

---

*latest update on 17th of August 2020*
