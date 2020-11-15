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

`Int32`

The encrypted object ID

##### Index

`UInt16`

XXX

##### Team

`TeamFlag`

XXX

##### TypeFlag

`UInt16`

XXX

##### Name

`String`

XXX

##### NetworkID

`UInt16`

XXX

##### Position

`Vector3`

Actual in-game position - use this for calculation

##### W2S

`Vector2`

World To Screen position - use this to set your mouse cursor etc

##### Distance

`Single`

Distance to Local Player

##### IsVisible

`Boolean`

XXX

##### Mana

`Single`

XXX

##### MaxMana

`Single`

XXX

##### Health

`Single`

XXX

##### MaxHealth

`Single`

XXX

##### AttackRange

`Single`

Attack Range of this object in 100th teemos

##### UnitStats

`UnitStats`

Unit stats of this object

##### Gold

`Single`

Current gold of this unit

##### BuffManager

`BuffManager`

Buff control manager of this unit

##### CombatType

`CombatTypes`

CombatType of this unit

##### UnitComponentInfo

`UnitComponentInfo`

The unit info of this object

##### ModelName

`String`

NAme of this object's Model

### Debug

Debug

#### Fields

##### Time

`Single`

The Debug-Time used with Start/StopTimer()

### Do

In-Game Actions Base Class

#### Functions

##### Move

Returns `Void`

Dispatches a move-command via mouse-click to given world position.

Usage: `Do:Move()`

##### Attack

Returns `Void`

Dispatches an attack-command via mouse-click to target hero.

Usage: `Do:Attack()`

##### Attack

Returns `Void`

Dispatches an attack-command via mouse-click to given world position.

Usage: `Do:Attack()`

##### RightClick

Returns `Void`

Sends a right click.

Usage: `Do:RightClick()`

##### LeftClick

Returns `Void`

Sends a left click.

Usage: `Do:LeftClick()`

##### MoveCursor

Returns `Void`

Moves cursor to given world position.

Usage: `Do:MoveCursor()`

##### Spell

Returns `Void`

Casts a spell via key-press event on given target hero.

Usage: `Do:Spell()`

##### Spell

Returns `Void`

Casts a spell via key-press event on given world position.

Usage: `Do:Spell()`

##### Item

Returns `Void`

Uses an item via key-press event on given target hero.

Usage: `Do:Item()`

##### Item

Returns `Void`

Uses an item via key-press event on given world position.

Usage: `Do:Item()`

##### Sleep

Returns `Void`

Sets this module to sleep for a provided number of milliseconds.

Usage: `Do:Sleep()`

### Cursor

### Key

#### Functions

##### Down

Returns `Boolean`

Usage: `Key:Down()`

### Calc

### Info

### Spells

### Minions

#### Functions

##### GetMinionsInRange

Returns `Minion[]`

Usage: `Minions:GetMinionsInRange()`

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

`Hero[]`

Contains all currently registered heroes.

### Dice

#### Fields

##### Random

`Single`

Returns a random number at call.

