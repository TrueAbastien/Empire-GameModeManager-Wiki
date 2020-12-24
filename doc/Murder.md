# Gamemode, classic GMod Murder.

* On Round Start, players are selected as Murderers, amist ClassD, and a set amount of player as Detectives, being Scientists.
* Each player is given a random name from the Phonetic Alphabet.
* The Murderers are equiped with a Disarmer (his Knife), a Coin (like any Bystander), a Chaos Keycard and SCP-268.
* The Murderers are also able to see Players through walls and change theirs nickname by picking up a coin.
* On each kill, the Murderers may get bonus items (such as Flash or Adrenaline).
* Each Detective is equiped with an USP which needs to be reloaded after each shot.
* If a Detective kills a Bystander, the USP is dropped and the Detective flashed for a few seconds.
* Any Bystander can pick up the USP and use it, a Murderer will explode if he tries.
* The Round ends if everyone is dead (as Murderer win) or if the Murderers die (as Bystander win).
* If the round last too long, the murderers name will be broacast (at decontamination).
* No one takes damage on decontamination and doors cannot be closed.

## Patches

* **KillCuffPatch:** The Murderer can kill any player by clicking him with a Disarmer.

## Configuration

### Murder

Name | Type | Value | Constraints | Description
:---: | :---: | :---: | :---: | :------
MurderDistance | float | 1.5 | Above 0, Not too high | Distance for a Murderer to make a kill.
DisarmerCooldown | float | 30.0 | Above 0 | Cooldown for Murder to get his 'knife'.
KillVisibility | bool | false | - | Disable invisibility (SCP-268) after a kill.
GrenadeMurder | bool | false | - | If a Murderer takes grenade damage or not.

### Role

Name | Type | Value | Constraints | Description
:---: | :---: | :---: | :---: | :------
BlindedDuration | float | 10.0 | Above 0 | Duration of blindness when a detective guess wrong.
PlayerPerDetective | uint | 10 | Above 2 | Amount of players required to get a new detective.
PlayerPerMurderer | uint | 20 | Above 2 | Amount of players required to get a new murderer.
CoinNameLuck | float | 0.5 | Above or equal to 0 | Luck of changing name on Coin Pickup.

## Commands

Name | Alias | Arguments | Permission | Description
:---: | :---: | :---: | :---: | :------
info | i, infos | - | Admin | Display confidential infos about the game state.
_info_ | - | - | User | Display important infos concerning the round depending on your role.

---

*latest update on 24th of December 2020*