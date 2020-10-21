# Gamemode, classic GMod Murder.

* On Round Start, a player is selected as Murderer, amist ClassD, and a set amount of player as Detectives, being Scientists.
* Each player is given a random name from the Phonetic Alphabet.
* The Murderer is equiped with a Disarmer (his Knife), a Coin (like any Bystander), a Chaos Keycard and SCP-268.
* The Murderer is also able to see Player through walls and change its nickname by picking up a coin.
* On each kill, the Murderer may get bonus items such as Flash or Adrenaline.
* Each Detective is equiped with an USP which needs to be reloaded after each shot.
* If a Detective kills a Bystander, the USP is dropped and the Detective flashed for a few seconds.
* Any Bystander can pick up the USP and use it, the Murderer will explode if he tries.
* The Round ends if everyone is dead (as Murderer win) or is the Murderer dies (as Bystander win).

## Patches

* **KillCuffPatch:** The Murderer can kill any player by clicking him with a Disarmer.

## Configuration

### Role

Name | Type | Value | Constraints | Description
:---: | :---: | :---: | :---: | :------
BlindedDuration | float | 10.0 | Above 0 | Duration of blindness when a detective guess wrong.
DetectiveAmount | uint | 2 | Above 0 | Amount of detective to spawn on round start.
AutoRegister | bool | true | - | Determine if registration is automatic or not.

## Commands

Name | Alias | Arguments | Permission | Description
:---: | :---: | :---: | :---: | :------
register | - | Player(s) Steam ID(s) | Manager | Register new players as detectives and/or murderer.

---

*latest update on 21st of October 2020*