<p align="center">
  <img width="38%" src="./img/border/left.svg">
  <img width="20%" src="./img/logo.svg">
  <img width="38%" src="./img/border/right.svg">
</p>

# Empire - GameModeManager Wiki, EXILED 2.0 plugin

Here follows the description of every Gamemodes made for the Private plugin *GameModeManager* for the Empire, a french gaming server on **SCP: Secret Laboratory**.

## User manual

### Gamemodes

Here is a list of every Gamemodes currently available:

Name | Prefix | State
:---: | :---: | :---:
[BlindLooters](./doc/BlindLooters.md) | BlindL | **Ready**
[Breach](./doc/Breach.md) | - | *On Work*
[DarkSouls](./doc/DarkSouls.md) | - | **Ready**
[HideAndSeek](./doc/HideAndSeek.md) | - | **Ready**
[HostageExtraction](./doc/HostageExtraction.md) | Hostage | **Ready**
[Murder](./doc/Murder.md) | - | **Ready**
[Pillar](./doc/Pillar.md) | - | **Ready**
[Purge](./doc/Purge.md) | - | **Ready**
[Scp035](./doc/Scp035.md) | - | **Ready**
[TeamFight](./doc/TeamFight.md) | Team | **Ready**
[ZombieInvasion](./doc/ZombieInvasion.md) | - | **Ready**

#### Samples

If you want to test the commands, try using the following examples:
* [Bomberman](./doc/Bomberman.md)
* [GlassMade](./doc/GlassMade.md)
* [WorkHazard](./doc/WorkHazard.md)

### Commands

In order to compute and use Gamemodes successfully, take into account the following commands:

Name | Aliases | Arguments | Permission | Description
:---: | :---: | :---: | :---: | :------
gm.load | - | GamemodeName | SET | Load a new Gamemode.
gm.unload | gm.stop | - | DEL | Unload the current Gamemode. If any, the following Gamemode in Waitlist will automatically load.
gm.add | gm.queue | GamemodeName | PUT | Add a Gamemode to the back of the Waitlist. If no Gamemode is currently loaded, the added Gamemode will automatically load.
gm.clear | gm.clean, gm.cls | ('all') | DEL | Clean the Gamemode Waitlist. If 'all' argument is given, also unload the current Gamemode.
gm.set | gm.trigger | TriggerName | SET | Set the current trigger loading the next event. Before every round start, if conditions are met, if any, the next Gamemode in Waitlist will automatically load.
gm.info | gm.current | - | GET | Print out informations about the current state of Gamemode process.

Every specific Gamemode commands should be called as such: ```gm.<GamemodePrefix>.<CommandName> <arguments...>```

> :warning: **A GamemodePrefix is usually the GamemodeName**, however they can be redefined for longer name so be careful...

### Permissions

Every command may comes with a specific permission to add to the *permission.yml* file. Two kinds of permission exists for this plugin: **Action** and **Rank** permissions.

Here is a list of both of them:

#### Action

Those one are usually used for the Plugin Core system commands.

Name | Value | Description
:---: | :---: | :------
GET | gm.get | Limited to informative commands, like the one only printing out informations.
SET | gm.set | Allow to set value through commands, like loading Gamemodes or settings Triggers.
PUT | gm.put | Meant for command adding or changing a value content without reset, like adding Gamemodes to the Waitlist.
DEL | gm.del | Reserved for deleting actions through commands, like unloading Gamemodes or clearing the Waitlist.

#### Rank

These should be limited to in-Gamemode commands use.

Name | Value | Description
:---: | :---: | :------
Manager | gm.manager | Given to the **Event Manager**, reserved to dangerous commands.
Admin | gm.admin | Meant for any **Admin** staff, commands which shouldn't be spammed.
Mod | gm.mod | Attributed to any **Moderator** on duty, disallow a random player to use the command.
User | gm.user | Callable by any random **User**, usually meant for informative commands.

### Configs

Configurations are dynamically handled in this Plugin allowing you for each Gamemode to change its defined settings value in runtime. However, after every **reload** their value will go back to default.

Each proprety can be accessed or changed through the following commands:

Name | Aliases | Arguments | Permission | Description
:---: | :---: | :---: | :---: | :------
gm.config.get | - | GamemodeName, PropretyName | GET | Get a proprety value from dynamic config.
gm.config.set | - | GamemodeName, PropretyName, value | SET | Set a proprety value from dynamic config.

In short, the commands call themselves likewise:
* ```gm.config.get <GamemodePrefix> <PropertyName>```
* ```gm.config.set <GamemodePrefix> <PropertyName> <Value>```

### Features

Additional features have been implemented into the *GameModeManager* to ensure and complete further developments required.

#### Invisibility

* This fake invisibility register player to appear invisible every time they spawn.
* Invisibility render players almost impossible to shoot/hit with raycasts means of damage.
* Players affected may encounter various bugs with the Physic Engine and should be precautious around walls, stairs or any other obstacles.
* It will still trigger SCP-096 & SCP-173 properties when looking at them and will appear as a thin vertical line when seen by SCP-939's vision.
* Interaction of any sort (door, damage, shoots, etc...) will not remove the invisibility.
* Whenever their invisibility is removed, players will get back the scale they originally had before becoming invisible.

##### Commands

Name | Aliases | Arguments | Permission | Description
:---: | :---: | :---: | :---: | :------
gm.invisibility.add | gm.invis.add | PlayerID | Admin | Add a player to the Invisibility List.
gm.invisibility.remove | gm.invis.remove | PlayerID | Admin | Remove a player from the Invisibility List.

#### Map Seed

* Allows you to lock a specific Seed for the complete map generation.
* Doesn't affect item generation or role distribution.
* Can be locked/freed at any time but require a restart when set.

##### Commands

Name | Aliases | Arguments | Permission | Description
:---: | :---: | :---: | :---: | :------
gm.mapseed.free | - | - | Mod | Free the 'currentSeed' to be set randomly, as usual, for each round.
gm.mapseed.info | - | - | Mod | Display info related to the current state of Seed making.
gm.mapseed.lock | - | - | Admin | Lock the seed to be set on the 'currentSeed' (if different from -1).
gm.mapseed.set | - | seed (integer between -1e10 and 1e10) | Set the 'currentSeed' to the given value & lock the seed if need be.

##### Patches

**RandomSeedSync.Start:** to lock the map seed if required.
**ImageGenerator.GeneratorTask_SetRooms:** to print out informations on Debug mode.


## Developper manual

```No developper ressources has actually been written yet, this is still ongoing work...```

---

*latest update* **_on 24th of December 2020_**
