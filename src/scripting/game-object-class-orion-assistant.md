# Game Object

### Command Format

**NameSpace**.**name**(_**requiredParameters**_, [_optionalParameters=defaultValue_]);

***

- String obj.Serial();

Result: Serial number of an Object.

***

- String obj.Graphic();

Result: Type of an Object (Picture ID).

***

- String obj.Color();

Result: Color of an Object.

***

- int obj.X();

Result: X object coordinates in world.

***

- int obj.Y();

Result: Y object coordinates in world.

***

- int obj.Z();

Result: Z object coordinates in world.

***

- String obj.Container();

Result: Serial number of an Main(parent)-Object. 0xFFFFFFFF if object is located in world.

***

- int obj.Map();

Result: World map objects index.

***

- int obj.Count();

Result: Quantity

***

- int obj.Flags();

Result: Object flags.

***

- String obj.Name();

Result: Name of an Object (empty for items, until click on object).

***

- bool obj.Mobile();

Result: true is object is alive.

***

- bool obj.Ignored();

Result: true - if object is marked as ignored.

***

- bool obj.Frozen();

Result: true - if object is frozen.

***

- bool obj.Poisoned();

Result: true - if object is poisoned.

***

- bool obj.Flying();

Result: true - if object is flying (gargoyle).

***

- bool obj.YellowHits();

Result: true - if object has yellow health bar.

***

- bool obj.IgnoreCharacters();

Result: true - if object is ignoring players while moving.

***

- bool obj.Locked();

Result: true - if object cant be moved or marked (items).

***

- bool obj.WarMode();

Result: true - if object is in war mode.

***

- bool obj.Hidden();

Result: true - if object is invisible.

***

- bool obj.IsHuman();

Result: true - if object is attacking humanoid.

***

- bool obj.IsPlayer();

Result: true - if object is current player.

***

- bool obj.IsCorpse();

Result: true - if object is dead body.

***

- int obj.Layer();

Result: Number of Layer - object is located in.

***

- bool obj.IsMulti();

Result: true - if object is - Multi.

***

- int obj.EquipLayer();

Result: Number of Layer - object is supposed to locate in.

***

- int obj.Hits();

Result: Hit points amount of an Object.

***

- int obj.MaxHits();

Result: Maximum hit points amount of an Object.

***

- int obj.Mana();

Result: Mana amount of an Object.

***

- int obj.MaxMana();

Result: Maximum mana amount of an Object.

***

- int obj.Stam();

Result: Stamina amount of an Object.

***

- int obj.MaxStam();

Result: Maximum stamina amount of an Object.

***

- bool obj.Female();

Result: true - if object player is a female gender.

***

- int obj.Race();

Result: Race number of an Object.

***

- int obj.Direction();

Result: Direction of an Object.

***

- int obj.Notoriety();

Result: Wickedness of an Object.

***

- bool obj.CanChangeName();

Result: true - if object can be renamed.

***

- bool obj.Dead();

Result: true - if object is dead.

***

- bool obj.Exists();

Result: true - if object does not exist.
***

## Introduced in 2.0.8.2

- String obj.Properties();

Returns string with object properties ( if they were received by MegaCliloc packet from server )

***

## Introduced in 2.0.12.0

- bool obj.ProfileReceived();

Returns true if profile was received from server.

***

- String obj.Profile();

Returns profile contents.

***

- String obj.Title();

Returns characters title ( displayed in paperdoll ).