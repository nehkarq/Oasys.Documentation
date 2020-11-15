# OASYS DOCUMENTATION



## LUA API

Examples can be found in the exmaple folder.

### Hero

Hero class

#### Functions

##### IsObject

Returns `Boolean`

XXX

Usage: `Hero:IsObject()`

##### IsTeam

Returns `Boolean`

XXX

Usage: `Hero:IsTeam()`

##### IsCombatType

Returns `Boolean`

Checks whether this unit has a given CombatType

Usage: `Hero:IsCombatType()`

#### Fields

##### EncryptedID

`Hero`

The encrypted object ID

##### Index

`Hero`

XXX

##### Team

`Hero`

XXX

##### TypeFlag

`Hero`

XXX

##### Name

`Hero`

XXX

##### NetworkID

`Hero`

XXX

##### Position

`Hero`

Actual in-game position - use this for calculation

##### W2S

`Hero`

World To Screen position - use this to set your mouse cursor etc

##### Distance

`Hero`

Distance to Local Player

##### IsVisible

`Hero`

XXX

##### Mana

`Hero`

XXX

##### MaxMana

`Hero`

XXX

##### Health

`Hero`

XXX

##### MaxHealth

`Hero`

XXX

##### AttackRange

`Hero`

Attack Range of this object in 100th teemos

##### UnitStats

`Hero`

Unit stats of this object

##### Gold

`Hero`

Current gold of this unit

##### BuffManager

`Hero`

Buff control manager of this unit

##### CombatType

`Hero`

CombatType of this unit

##### UnitComponentInfo

`Hero`

The unit info of this object

##### ModelName

`Hero`

NAme of this object's Model

### Debug

### Do

### Cursor

### Key

### Calc

### Info

### Spells

### Minions

### Heroes

#### Functions

##### GetAll

Returns `Hero[]`

Returns all currently registered heroes.

Usage: `Heroes:GetAll()`

##### GetEnemies

Returns `Hero[]`

Returns all currently registered enemy heroes.

Usage: `Heroes:GetEnemies()`

##### GetEnemiesInRange

Returns `Hero[]`

Returns all currently registered enemy heroes within a given range.

Usage: `Heroes:GetEnemiesInRange()`

##### GetAllies

Returns `Hero[]`

Returns all currently registered allied heroes.

Usage: `Heroes:GetAllies()`

##### TEMP_GetClosestToPlayer

Returns `Hero`

Returns the closest hero to the player.

Usage: `Heroes:TEMP_GetClosestToPlayer()`

#### Fields

##### Objects

`Heroes`

Contains all currently registered heroes.

### Dice

