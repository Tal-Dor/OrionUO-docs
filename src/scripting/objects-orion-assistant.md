# Objects

### Command Format

**NameSpace**.**name**(_**requiredParameters**_, [_optionalParameters=defaultValue_]);
</br></br>
***
</br>
_void_ **Orion.Info**(['serial'=targetRequest]);

Display information about the object "serial" in a text box.

Request target to be aimed at the desired object, if parameters were not specified.
</br></br>
***
</br>
_void_ **Orion.InfoTile**(['lasttile'=targetRequest]);

Display information about 'lasttile' (tile, on which target was selected last time ) in the text box.

Request target to be aimed at the desired tile, if parameters were not specified.
</br></br>
***
</br>
_String_ **Orion.GetSerial**('serial');

Returns real value of the serial.

For instance: Orion.GetSerial(self) or Orion.GetSerial(lastcontainer) - will return the serial of the player 0x12345678
</br></br>
***
</br>
_String_ **Orion.GetGraphic**('graphic');

Return real value of "graphic".

For instance: Orion.GetGraphic('bm') - will return type of blood moss, stated in Lists/Types
</br></br>
***
</br>
_String_ **Orion.GetContainer**('serial');

Return serial of the object, in which an object with "serial" is located.

Orion.GetContainer(self) will return 0xFFFFFFFF (worlds serial) or Orion.GetContainer(backpack) - will return serial of the player 0x12345678, since backpack container is the player, who's owning it.
</br></br>
***
</br>
_void_ **Orion.Click**(['serial'=self]);

Request click for the object serial.
</br></br>
***
</br>
_void_ **Orion.UseObject**(['serial'=self]);

Request to use (doubleclick) the object serial.
</br></br>
***
</br>
_void_ **Orion.GetStatus**(['serial'=self]);

Request for the object serial status.
</br></br>
***
</br>
_void_ **Orion.Attack**('serial');

Request to attack the object serial.
</br></br>
***
</br>
_void_ **Orion.Hide**(['serial'=targetRequest]);

Hide the object serial.

Request target selection for the object indication, if parameters were not specified.
</br></br>
***
</br>
_void_ **Orion.RenameMount**('serial', 'new name');

Rename your mount "serial".
</br></br>
***
</br>
_void_ **Orion.Drop**(['serial'=targetRequest], [count=0(all)], [x=-1, y=-1, z=0]);

Drop the item 'serial' with amount 'count' into coordinates x, y, z ; Use target if parameters were not specified.
</br></br>
***
</br>
_void_ **Orion.DropHere**(['serial'=targetRequest], [count=0(all)]);

Drop the item 'serial' under the character with amount 'count'. Request target to be aimed at the desired object, if parameters were not specified.
</br></br>
***
</br>
_void_ **Orion.MoveItem**(['serial'=targetRequest], [count=0(all)], ['container'=backpack], [x=-1, y=-1], [z=0]);

Move the object 'serial' with amount 'count' to the container 'container' into coordinates x, y, z (z when throwing on the ground), use target if parameters were not specified.
</br></br>
***
</br>
_int_ **Orion.GetDistance**('serial');

Return distance to the object.
</br></br>
***
</br>
_int_ **Orion.GetDistance**(x, y);

Return distance to the coordinates.
</br></br>
***
</br>
_void_ **Orion.BandageSelf**();

Bandageself.
</br></br>
***
</br>
_String_ **ClientLastTarget**();

Get the state of the global client variable LastTarget.

Result: The _String_ with the serial.
</br></br>
***
</br>
_void_ **ClientLastTarget**(serial);

Set the state of the client global variable LastTarget to the serial.
</br></br>
***
</br>
_String_ **ClientLastAttack**();

Get the state of the global client variable LastAttack

Result: The _String_ with the serial.
</br></br>
***
</br>
_void_ **ClientLastAttack**(serial);

Set the state of the global client variable LastAttack to the serial.
</br></br>
***
</br>
_String_ **TargetSystemSerial**();

Get the state of the global client variable TargetSystemSerial (from new target system).

Result: The String with the serial.
</br></br>
***
</br>
_void_ **TargetSystemSerial**(serial);

Set the state of the global client variable TargetSystemSerial (from new target system) to the serial.
</br></br>
***
</br>
_void_ **Orion.GetFriendsStatus**();

Retrieves statuses of all friends in update range ( required to get updates about their hp etc. ).
</br></br>
***
</br>
_void_ **Orion.GetEnemiesStatus**();

Retrieves statuses of all enemies in update range ( required to get updates about their hp etc. ).
</br></br>
***
</br>
_PositionObject_ **Orion.GetLastTargetPosition**();

Retrieves latest coordinates of LastTarget, if object has disappeared - it will retrieve last known coordinates.

Returns: a PositionObject data type.
</br></br>
***
</br>
_PositionObject_ **Orion.GetLastAttackPosition**();

Retrieves latest coordinates of LastAttack, if object has disappeared - it will retrieve last known coordinates.

Returns: a PositionObject data type.
</br></br>
***
</br>
_bool_ **Orion.OpenContainer**('serial', ['delay'=600], ['errorTextPattern']);

Open container.

- `serial` - serial of the container we're opening.

- `delay` - Maximum delay for container opening action.

- `errorTextPattern` - Error text. Default: 'reach that|too away'.

Returns: true if container was opened successfully.
</br></br>
***
</br>
_bool_ **Orion.ObjectExists**('serial');

Returns: true if object with 'serial' is present in OA memory.
</br></br>
***
</br>
_String_ **Orion.RequestName**('serial', ['delay'=200]);

Requests objects name. If the name is already present, it will return immediately. Otherwise name will be requested from the server.

- `serial` - serial of the object we're requesting name from.

- `delay` - Max delay for name requesting.

Returns: Objects name or an empty _String_ if failed.
</br></br>
***
</br>
_bool_ **Orion.GetProfile**('serial', ['delay'=300], ['errorTextPattern']);

Retrieves characters profile.

- `serial` - characters serial.

- `delay` - maximum wait time for profile retrievement.

- `errorTextPattern` - error pattern, default: 'reach that|too away'.

Returns true if a profile was retrieved.
</br></br>
***
</br>
_void_ **Orion.ShowStatusbar**('serial', x, y, [minimized=true]);

Show/Move status bar gump in client screen.

- `serial` - character serial.

- `x` - screen X coordinate.

- `y` - screen Y coordinate.

- `minimized` - only for your character. true will show minimized status bar, false will show expanded one.
</br></br>
***
</br>
_void_ **Orion.CloseStatusbar**('serial');

Close status bar which belongs to serial.
