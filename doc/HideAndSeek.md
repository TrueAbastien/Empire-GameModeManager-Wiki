# HideAndSeek, some hide while other seek but most will die.

A pack of 939 (seekers) is liberated in LCZ after a given time to ClassD (hiders) to hide themselves in the zone.
After a given amount of hiders are killed, each level open up little by little.
Whene the LCZ checkpoints open, a countdown to decontamination triggers: decontamination will kill Hiders and teleport Seekers in HCZ.
If a hider escapes, a final showdown will take place on the surface.
Seekers will be stunned for a few seconds whenever they take damages (if activated).

## Configuration

### Amount

Name | Type | Value | Constraints | Description
:---: | :---: | :---: | :---: | :------
FirstStageAmount | int | 10 | Above 0, Above *SecondStageAmount* | Amount of people remaining to open LCZ Checkpoints.
SecondStageAmount | int | 6 | Above 0, Above *ThirdStageAmount*, Under *FirstStageAmount* | Amount of people remaining to open HCZ Checkpoint.
ThirdStageAmount | int | 2 | Above 0, Under *SecondStageAmount* | Amount of people remaining to open EZ Gates.
SeekerLimit | int | 3 | Above 0 | Limit of seekers to spawn on round start.

### Delay

Name | Type | Value | Constraints | Description
:---: | :---: | :---: | :---: | :------
SeekerDelay | float | 90.0 | Above 0 | Delay before Seekers spawn in LCZ.
StageDelay | float | 5.0 | Above 0 | Delay before advancing to next stage.
DecontaminationDelay | float | 120.0 | Above 0 | Delay before decontamination.
WarheadDelay | float | 30.0 | Above 0 | Delay before warhead activation on ClassD escape.

### Status

Name | Type | Value | Constraints | Description
:---: | :---: | :---: | :---: | :------
EnsnaredSwitch | bool | true | ~~none~~ | Activation of ensnared effect on damages took.
EnsnaredMultiplier | float | 0.1 | Above 0 | Multiplier from damages to immobility duration.
MaxEnsnaredDuration | float | 5.0 | Above 0 | Maximum duration applied on damage in seconds.

---

*latest update on 17th of August 2020*
