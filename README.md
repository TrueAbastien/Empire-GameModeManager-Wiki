<p align="center">
  <img width="40%" src"./img/border/left.svg">
  <img width="10%" src="./img/logo.svg">
  <img width="40%" src"./img/border/right.svg">
</p>

# Empire - GameModeManager Wiki, EXILED 2.0 plugin

Here follows the description of every Gamemodes made for the Private plugin *GameModeManager* for the Empire, a french gaming server on **SCP: Secret Laboratory**.

## User manual

### Gamemodes

Here is a list of every Gamemodes currently available:
* DarkSouls
* HideAndSeek
* Purge
* ZombieInvasion

The following plugins are currently being worked on:
* Murder

#### Samples

If you want to test the commands, try using the following examples:
* Bomberman
* GlassMade
* WorkHazard

### Commands

In order to compute and use Gamemodes successfully, take into account the following commands:

Name | Aliases | Arguments | Description
:---: | :---: | :---: | :------
gm.load | ~~none~~ | GamemodeName | Load a new Gamemode.
gm.unload | gm.stop | ~~none~~ | Unload the current Gamemode. If any, the following Gamemode in Waitlist will automatically load.
gm.add | gm.queue | GamemodeName | Add a Gamemode to the back of the Waitlist. If no Gamemode is currently loaded, the added Gamemode will automatically load.
gm.clear | gm.clean, gm.cls | ('all') | Clean the Gamemode Waitlist. If 'all' argument is given, also unload the current Gamemode.
gm.set | gm.trigger | TriggerName | Set the current trigger loading the next event. Before every round start, if conditions are met, if any, the next Gamemode in Waitlist will automatically load.
gm.info | gm.current | ~~none~~ | Print out informations about the current state of Gamemode process.

### Configs

Configurations are dynamically handled in this Plugin allowing you for each Gamemode to change its defined settings value in runtime. However, after every **reload** their value will go back to default.

Each proprety can be accessed or changed through the following commands:

Name | Aliases | Arguments | Description
:---: | :---: | :---: | :------
gm.config.get | ~~none~~ | GamemodeName, PropretyName | Get a proprety value from dynamic config.
gm.config.set | ~~none~~ | GamemodeName, PropretyName, value | Set a proprety value from dynamic config.


## Developper manual

```*No developper ressources has actually been written yet, this is still ongoing work...*```

---

*latest update* **_on 17th August of 2020_**
