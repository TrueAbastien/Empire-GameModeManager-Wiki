# TeamFight, a modular game of fighting the others.

#### <ins>Prefix:</ins> **Team**

* Each team is spawned somewhere, in a selected room in a selected zone.
* Before the game starts, every doors is locked.
* In the waiting phase, players may receive items and ammos and will be moved on room changed.
* Once the game starts, the doors open and players are free to kill the other team players.
* Gate will be opened but Lifts & 914 may not be opened.
* People do not respawn (usually) and will fight the other team to the death.
* The Round ends when only one team remains.
* The Gamemode and its rules may change depending on the current ruleset.

## Configuration

### Allow

Name | Type | Value | Constraints | Description
:---: | :---: | :---: | :---: | :------
AllowLift | bool | false | - | Allow for people to use lifts.
Allow914 | bool | false | - | Allow for people to use 914.
AllowItems | bool | false | - | Allow players to keep their items on spawn.

### Class
Name | Type | Value | Constraints | Description
:---: | :---: | :---: | :---: | :------
DefaultClassA | Enum.RoleType | RoleType.ClassD | Must be different from **DefaultClassB** | Default class for first team.
DefaultClassB | Enum.RoleType | RoleType.Scientist | Must be different from **DefaultClassA** | Default class for second team.

## Commands

Name | Alias | Arguments | Permission | Description
:---: | :---: | :---: | :---: | :------
room | spawn | 'A'/'B', 'Here'/RoomName | Admin | Change the spawn room in which to play.
zone | changezone, newzone | ZoneName | Admin | Change the Zone in which the match is played in.
give | item, add | ItemType/ItemID, [Amount] | Admin | Add an item (or ammo) to everyone.

---

*latest update on 21st of October 2020*