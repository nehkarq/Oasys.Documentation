## OASYS DOCUMENTATION



# LUA API

Examples can be found in the exmaple folder.

## Hero

Hero class

### Functions

#### Hero:IsObject(oTF)

Returns `Boolean`

XXX





#### Hero:IsTeam(tFlag)

Returns `Boolean`

XXX





#### Hero:IsCombatType(CType)

Returns `Boolean`

Checks whether this unit has a given CombatType





#### Fields

#### EncryptedID

`Int32`

The encrypted object ID

#### Index

`UInt16`

XXX

#### Team

`TeamFlag`

XXX

#### TypeFlag

`UInt16`

XXX

#### Name

`String`

XXX

#### NetworkID

`UInt16`

XXX

#### Position

`Vector3`

Actual in-game position - use this for calculation

#### W2S

`Vector2`

World To Screen position - use this to set your mouse cursor etc

#### Distance

`Single`

Distance to Local Player

#### IsVisible

`Boolean`

XXX

#### Mana

`Single`

XXX

#### MaxMana

`Single`

XXX

#### Health

`Single`

XXX

#### MaxHealth

`Single`

XXX

#### AttackRange

`Single`

Attack Range of this object in 100th teemos

#### UnitStats

`UnitStats`

Unit stats of this object

#### Gold

`Single`

Current gold of this unit

#### BuffManager

`BuffManager`

Buff control manager of this unit

#### CombatType

`CombatTypes`

CombatType of this unit

#### UnitComponentInfo

`UnitComponentInfo`

The unit info of this object

#### ModelName

`String`

NAme of this object's Model

## Debug

Debug

### Functions

#### Debug:Write(any)

Returns `Void`

Writes given parameter into console output.





#### Debug:Object(any)

Returns `Void`

Renders an object, JSON formatted, into the console output.





#### Debug:Read()

Returns `String`

Returns inputted user text.





#### Debug:StartTimer()

Returns `Void`

Starts the Debug-Timer





#### Debug:StopTimer()

Returns `Single`

Stops the Debug-Timer





#### Fields

#### Time

`Single`

The Debug-Time used with Start/StopTimer()

## Do

In-Game Actions Base Class

### Functions

#### Do:Move(x, y)

Returns `Void`

Dispatches a move-command via mouse-click to given world position.





#### Do:Attack(target)

Returns `Void`

Dispatches an attack-command via mouse-click to target hero.





#### Do:Attack(x, y)

Returns `Void`

Dispatches an attack-command via mouse-click to given world position.





#### Do:RightClick()

Returns `Void`

Sends a right click.





#### Do:LeftClick()

Returns `Void`

Sends a left click.





#### Do:MoveCursor(x, y)

Returns `Void`

Moves cursor to given world position.





#### Do:Spell(slot, target)

Returns `Void`

Casts a spell via key-press event on given target hero.





#### Do:Spell(slot, x, y)

Returns `Void`

Casts a spell via key-press event on given world position.





#### Do:Item(slot, target)

Returns `Void`

Uses an item via key-press event on given target hero.





#### Do:Item(slot, x, y)

Returns `Void`

Uses an item via key-press event on given world position.





#### Do:Sleep(ms)

Returns `Void`

Sets this module to sleep for a provided number of milliseconds.





## Cursor

## Key

### Functions

#### Key:Down(code)

Returns `Boolean`





## Calc

## Info

## Spells

## Minions

### Functions

#### Minions:GetMinionsInRange(range)

Returns `Minion[]`





## Heroes

### Functions

#### Heroes:GetAll()

Returns `Hero[]`

Returns all currently registered heroes.





#### Heroes:GetEnemies()

Returns `Hero[]`

Returns all currently registered enemy heroes.





#### Heroes:GetEnemiesInRange(range)

Returns `Hero[]`

Returns all currently registered enemy heroes within a given range.





#### Heroes:GetAllies()

Returns `Hero[]`

Returns all currently registered allied heroes.





#### Heroes:TEMP_GetClosestToPlayer()

Returns `Hero`

Returns the closest hero to the player.





#### Fields

#### Objects

`Hero[]`

Contains all currently registered heroes.

## Dice

### Functions

#### Dice:Roll(chance)

Returns `Boolean`

Rolls % chance and returns true if chance was met.





#### Dice:Range(min, max)

Returns `Single`

Returns a random value between min and max (max exclusive).





#### Dice:Range(min, max)

Returns `Int32`

Returns a random value between min and max (max exclusive).





#### Dice:Choose(options)

Returns `T`

Chooses one of the given parameters as random and returns it.





#### Dice:ExpoRoll(min, max, power, defx)

Returns `Single`

This is complicated to explain.





#### Dice:BrewString(length, set)

Returns `String`

Returns a random alphanumeric string of given length.





#### Fields

#### Random

`Single`

Returns a random number at call.

