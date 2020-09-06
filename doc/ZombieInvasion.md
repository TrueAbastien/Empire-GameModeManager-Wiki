# ZombieInvasion, like the good old days.

* Every SCPs is either 049 or its zombies while others are Guards.
* While 049 is alive, every death will result in a new zombie which grows weaker after each death.
* Killing zombies should grant the killer more ammos.
* Whenever the bleeding 049 dies, only dying zombies will respawn as guards.

## Configuration

### Amount

Name | Type | Value | Constraints | Description
:---: | :---: | :---: | :---: | :------
AmmoGainAmount | uint | 35 | Above 0 | Amount of MP7 ammo gained on Zombie kill.
AllAmmoGainAmount | uint | 10 | Above 0 | Amount of MP7 ammo gained on Zombie kill for all Players.

### Delay

Name | Type | Value | Constraints | Description
:---: | :---: | :---: | :---: | :------
ZombieDelay | float | 10.0 | Above 0 | Delay before a Zombie respawns.

### Health

Name | Type | Value | Constraints | Description
:---: | :---: | :---: | :---: | :------
ZombieMinimalHealth | float | 50.0 | Above 0, Under 300 | Minimal health a zombie can get to.
ZombieHealthDecrease | float | 100.0 | Above 0, Under *300 - ZombieMinimalHealth* | Health decrease on zombie death.

### Misc

Name | Type | Value | Constraints | Description
:---: | :---: | :---: | :---: | :------
SizeMultiplier | float | 1.15 | Above 0 | Size multiplier for Scp049.

---

*latest update on 22nd of August 2020*