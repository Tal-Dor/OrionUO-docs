# Player Character

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

Result: X object coordinates in the world.

***

- int obj.Y();

Result: Y object coordinates in the world.

***

- int obj.Z();

Result: Z object coordinates in the world.

***

- String obj.Container();

Result: Serial number of an Main(parent)-Object. 0xFFFFFFFF if object is located in world.

***

- int obj.Map();

Result: World map objects index.

***

- int obj.Count();

Result: Quantity.

***

- int obj.Flags();

Result: Object flags.

***

- String obj.Name();

Result: Name of an Objext (empty for items, until click on object).

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

- bool obj.Paralyzed();

Result:true - if object is paralyzed.

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

Result: true - if object is in war mode

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

- int obj.Str();

Result: Str value of an Object.

***

- int obj.Int();

Result: Int value of an Object.

***

- int obj.Dex();

Result: Dex value of an Object.

***

- int obj.LockStrState();

Result: The value perspective gaining Str of an Object.

***

- int obj.LockIntState();

Result: The value perspective gaining Int of an Object.

***

- int obj.LockDexState();

Result: The value perspective gaining Dex of an Object.

***

- int obj.Weight();

Result: Weight value of an object.

***

- int obj.MaxWeight();

Result: Maximum weight value of an object.

***

- int obj.Armor();

Result: Armor value of an Object.

***

- int obj.Gold();

Result: Gold value of an Object.

***

- int obj.StatsCap();

Result: Maximum Statcap value (str+int+dex) of an Object.

***

- int obj.Followers();

Result: Creature quantity tamed to an Object.

***

- int obj.MaxFollowers();

Result: Maximum creature quantity that can be dependent to an Object.

***

- int obj.FireResistance();

Result: Fire defence value of an Object.

***

- int obj.ColdResistance();

Result: Cold defence value of an Object.

***

- int obj.PoisonResistance();

Result: Poison defence value of an Object.

***

- int obj.EnergyResistance();

Result: Energy defence value of an Object.

***

- int obj.Luck();

Result: Luck value of an Object.

***

- int obj.MinDamage();

Result: Minimal damage value of an Object.

***

- int obj.MaxDamage();

Result: Maximum damage value of an Object.

***

- int obj.TithingPoints();

Result: Skill point value of an Object.

***

- int obj.StealthSteps();

Result: Number of steps in Stealth of an Object.

***

## Introduced in 2.0.10.0

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
