# Pillar, dodging the snapping.

* Most player are spawned as ClassD while a given amount of player are spawned as Scp-173.
* They all are teleported in one closed room where Scp-173 have to kill all the ClassD.
* When only one ClassD remains, he gets to choose where to play the next round in.
* The previous winner will always be a Scp-173 for the next round.

## Configuration

### General

Name | Type | Value | Constraints | Description
:---: | :---: | :---: | :---: | :------
PeanutAmount | int | 3 | Above 0 | Amount of 173 per round.
SpawnOffset | float | 2.0 | ~~none~~ | Height offset on round start spawn-teleportation.
AutoPeanut | bool | false | ~~none~~ | Automatically teleports 173 after 'PeanutDelay'.

### Delay

Name | Type | Value | Constraints | Description
:---: | :---: | :---: | :---: | :------
PeanutDelay | float | 3.0 | Above 0 | Delay before 173 spawn.
SpawnDelay | float | 5.0 | Above 0 | Delay before next round when a room is picked.

## Commands

Name | Alias | Arguments | Permission | Description
:---: | :---: | :---: | :---: | :------
pick | room, next, pickroom | 'here'/RoomName | Mod | Pick the next room to play the round in.

---

*latest update on 22nd of August 2020*