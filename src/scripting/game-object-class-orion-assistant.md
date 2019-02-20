# Game Object

### Command Format

**NameSpace**.**name**(_**requiredParameters**_, [_optionalParameters=defaultValue_]);
</br></br>
***
</br>
_String_ **obj.Serial**();

Result: Serial number of an Object.
</br></br>
***
</br>
_String_ **obj.Graphic**();

Result: Type of an Object (Picture ID).
</br></br>
***
</br>
_String_ **obj.Color**();

Result: Color of an Object.
</br></br>
***
</br>
_int_ **obj.X**();

Result: X object coordinates in world.
</br></br>
***
</br>
_int_ **obj.Y**();

Result: Y object coordinates in world.
</br></br>
***
</br>
_int_ **obj.Z**();

Result: Z object coordinates in world.
</br></br>
***
</br>
_String_ **obj.Container**();

Result: Serial number of an Main(parent)-Object. 0xFFFFFFFF if object is located in world.
</br></br>
***
</br>
_int_ **obj.Map**();

Result: World map objects index.
</br></br>
***
</br>
_int_ **obj.Count**();

Result: Quantity
</br></br>
***
</br>
_int_ **obj.Flags**();

Result: Object flags.
</br></br>
***
</br>
_String_ **obj.Name**();

Result: Name of an Object (empty for items, until click on object).
</br></br>
***
</br>
_bool_ **obj.Mobile**();

Result: true is object is alive.
</br></br>
***
</br>
_bool_ **obj.Ignored**();

Result: true - if object is marked as ignored.
</br></br>
***
</br>
_bool_ **obj.Frozen**();

Result: true - if object is frozen.
</br></br>
***
</br>
_bool_ **obj.Poisoned**();

Result: true - if object is poisoned.
</br></br>
***
</br>
_bool_ **obj.Flying**();

Result: true if obj.ct is flying (gargoyle).
</br></br>
***
</br>
_bool_ **obj.YellowHits**();

Result: true - if object has yellow health bar.
</br></br>
***
</br>
_bool_ **obj.IgnoreCharacters**();

Result: true - if object is ignoring players while moving.
</br></br>
***
</br>
_bool_ **obj.Locked**();

Result: true - if obj.ct cant be moved or marked (items).
</br></br>
***
</br>
_bool_ **obj.WarMode**();

Result: true - if object is in war mode.
</br></br>
***
</br>
_bool_ **obj.Hidden**();

Result: true - if object is invisible.
</br></br>
***
</br>
_bool_ **obj.IsHuman**();

Result: true - if object is attacking humanoid.
</br></br>
***
</br>
_bool_ **obj.IsPlayer**();

Result: true - if object is current player.
</br></br>
***
</br>
_bool_ **obj.IsCorpse**();

Result: true - if object is dead body.
</br></br>
***
</br>
_int_ **obj.Layer**();

Result: Number of Layer - object is located in.
</br></br>
***
</br>
_bool_ **obj.IsMulti**();

Result: true - if object is - Multi.
</br></br>
***
</br>
_int_ **obj.EquipLayer**();

Result: Number of Layer - object is supposed to locate in.
</br></br>
***
</br>
_int_ **obj.Hits**();

Result: Hit points amount of an Object.
</br></br>
***
</br>
_int_ **obj.MaxHits**();

Result: Maximum hit points amount of an Object.
</br></br>
***
</br>
_int_ **obj.Mana**();

Result: Mana amount of an Object.
</br></br>
***
</br>
_int_ **obj.MaxMana**();

Result: Maximum mana amount of an Object.
</br></br>
***
</br>
_int_ **obj.Stam**();

Result: Stamina amount of an Object.
</br></br>
***
</br>
_int_ **obj.MaxStam**();

Result: Maximum stamina amount of an Object.
</br></br>
***
</br>
_bool_ **obj.Female**();

Result: true - if object player is a female gender.
</br></br>
***
</br>
_int_ **obj.Race**();

Result: Race number of an Object.
</br></br>
***
</br>
_int_ **obj.Direction**();

Result: Direction of an Object.
</br></br>
***
</br>
_int_ **obj.Notoriety**();

Result: Wickedness of an Object.
</br></br>
***
</br>
_bool_ **obj.CanChangeName**();

Result: true - if object can be renamed.
</br></br>
***
</br>
_bool_ **obj.Dead**();

Result: true - if object is dead.
</br></br>
***
</br>
_bool_ **obj.Exists**();

Result: true - if object does not exist.</br></br>
***
</br>
_String_ **obj.Properties**();

Returns string with object properties ( if they were received by MegaCliloc packet from server )
</br></br>
***
</br>
_bool_ **obj.ProfileReceived**();

Returns true if profile was received from server.
</br></br>
***
</br>
_String_ **obj.Profile**();

Returns profile contents.
</br></br>
***
</br>
_String_ **obj.Title**();

Returns characters title ( displayed in paperdoll ).
