# BlindLooters, cooperative suffering speedrun.

#### <ins>Prefix:</ins> **BlindL**

* Players are sperated by being either ClassD or Scientist.
* The two teams have to help each other by looking for each player *Reward Item*.
* Each *Reward Item* brings points to the party and is mendatory to escape.
* Once a player has its item, he can escape the foundation and become a Zombie to help others.
* However, at a given interval, each team gets 'flashed' turn by turn (either Scientists or ClassDs).
* Whenever people die, they will respawn with their previous role at a random spawn point in LCZ.
* After a given time, the game ends and the Warhead explodes (finishing the round).
* The quicker a player escapes, the more points he'll bring to this round.
* Every escapee should drop their items to a randomly selected room on the map.

## Patches

* **SpeakingSCP:** All SCPs can now speak using their secondary vocal keybind.

## Configuration

### Time

Name | Type | Value | Constraints | Description
:---: | :---: | :---: | :---: | :------
StartDelay | float | 10.0 | Above 0 | Delay in seconds before LCZ doors gets unlocked.
FlashDuration | float | 120.0 | Above 0 | Duration of the flash effect on any personnel.
RoundDuration | float | 595.0 | Above 0, Slightly under **x** \* 'FlashDuration' | Duration of the round before Warhead explodes.
WarheadDuration | float | 90.0 | Above 0, Well under 'RoundDuration' | Time the warhead takes to explode.
EndDuration | float | 10.0 | Above 0 | Duration after which players explode at the end.
DisplayItemDuration | ushort | 15 | Above 0 | Duration after which the rewarding item of a player disappear.

## Commands

Name | Alias | Arguments | Permission | Description
:---: | :---: | :---: | :---: | :------
_item_ | info, reward | - | User | Display the name of your current reward item.
room | spawn, drop, drops | all | Admin | Display the informations regarding the room in which items are dropped.

---

*latest update on 21st of October 2020*