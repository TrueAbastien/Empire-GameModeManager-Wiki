# ZombieInvasion, like the good old days.

* Every SCPs is either 049 or its zombies while others are Guards.
* While 049 is alive, every death will result in a new zombie which grows weaker after each death.
* 049 is affected with Bleeding and Burned effect and its size is slightly changed.
* Every zombie has a chance to open a door on interaction, 049 can open any door on first try.
* Killing zombies should grant the killer more ammos and regen its stamina.
* However, whenever a zombie dies, all guards receive a small amount of ammo.
* Whenever 049 dies, dying zombies will respawn as guards.

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
ZombieDoorLuck | float | 0.01 | Between 0 and 1 | Luck of opening a door as a Zombie.
ScpDoorSwitch | bool | true | - | SCPs can open doors.

---

*latest update on 21st of October 2020*
