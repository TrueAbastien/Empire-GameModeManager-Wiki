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
[BlindLooters](./doc/BlindLooters.md) | BlindL | *Untested*
[DarkSouls](./doc/DarkSouls.md) | - | *On Rework*
[HideAndSeek](./doc/HideAndSeek.md) | - | **Ready**
[HostageExtraction](./doc/HostageExtraction.md) | Hostage | **Ready**
[Murder](./doc/Murder.md) | - | *On Work*
[Pillar](./doc/Pillar.md) | - | *Untested*
[Purge](./doc/Purge.md) | - | **Ready**
[Scp035](./doc/Scp035.md) | - | *Untested*
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


## Developper manual

```No developper ressources has actually been written yet, this is still ongoing work...```

---

*latest update* **_on 6th of September 2020_**
