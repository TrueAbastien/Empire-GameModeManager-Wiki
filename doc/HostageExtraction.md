# HostageExtraction, the usual mission: in and out.

#### <ins>Prefix:</ins> **Hostage**

* A single player is picked to be the hostage (Scientist), others are either Chaos or MTF.
* MTF have to free the Scientist while Chaos have to keep the hostage.
* The game end either by having all the Chaos terminated, all the MTF respawn killed or by killing the hostage or freeing him.
* The hostage cannot take damages in LCZ or HCZ if he doesn't have any weapon, disarmer, ball, hat or grenade.
* Cuffing the Scientist may have him ensnared (which can be undone).
* MTF respawn will be more important if more Chaos remain and usually are triggered on all MTF death (but can be called manually).

## Configuration

### General

Name | Type | Value | Constraints | Description
:---: | :---: | :---: | :---: | :------
ChaosRepartition | float | 0.5 | Between 0 and 1 | Chaos starting amount over MTF starting amount.
CuffedImmobility | bool | false | - | Become immobilized when cuffed.
HostageDamageFactor | float | 0.05 | Above or equal to 0 | Multiplier of damage delt to the Hostage.

### Respawn

Name | Type | Value | Constraints | Description
:---: | :---: | :---: | :---: | :------
RespawnAmount | int | 1 | Above or equal to 0 | Amount of custom NTF respawn allowed.
MinimumRespawnAmount | int | 4 | Above or equal to 0 | Minimum amount of custom NTF to respawn.
LieutenantChances | float | 0.3 | Between 0 and 1 | Chances of becoming a lieutenant on custom NTF spawn.

## Commands

Name | Alias | Arguments | Permission | Description
:---: | :---: | :---: | :---: | :------
respawn | r, next, new, respawnNTF | - | Admin | Force a new MTF respawn.

---

*latest update on 22nd of August 2020*