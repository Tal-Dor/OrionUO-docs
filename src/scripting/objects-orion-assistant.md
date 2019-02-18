# Objects

### Command Format

**NameSpace**.**name**(_**requiredParameters**_, [_optionalParameters=defaultValue_]);

***

- void Orion.Info(['serial'=targetRequest]);

Display information about the object "serial" in a text box.

Request target to be aimed at the desired object, if parameters were not specified.

***

- void Orion.InfoTile(['lasttile'=targetRequest]);

Display information about 'lasttile' (tile, on which target was selected last time ) in the text box.

Request target to be aimed at the desired tile, if parameters were not specified.

***

- String Orion.GetSerial('serial');

Returns real value of the serial.

For instance: Orion.GetSerial(self) or Orion.GetSerial(lastcontainer) - will return the serial of the player 0x12345678

***

- String Orion.GetGraphic('graphic');

Return real value of "graphic".

For instance: Orion.GetGraphic('bm') - will return type of blood moss, stated in Lists/Types

***

- String Orion.GetContainer('serial');

Return serial of the object, in which an object with "serial" is located.

Orion.GetContainer(self) will return 0xFFFFFFFF (worlds serial) or Orion.GetContainer(backpack) - will return serial of the player 0x12345678, since backpack container is the player, who's owning it.

***

- void Orion.Click(['serial'=self]);

Request click for the object serial.

***

- void Orion.UseObject(['serial'=self]);

Request to use (doubleclick) the object serial.

***

- void Orion.GetStatus(['serial'=self]);

Request for the object serial status.

***

- void Orion.Attack('serial');

Request to attack the object serial.

***

- void Orion.Hide(['serial'=targetRequest]);

Hide the object serial.

Request target selection for the object indication, if parameters were not specified.

***

- void Orion.RenameMount('serial', 'new name');

Rename your mount "serial".

***

- void Orion.Drop(['serial'=targetRequest], [count=0(all)], [x=-1, y=-1, z=0]);

Drop the item 'serial' with amount 'count' into coordinates x, y, z ; Use target if parameters were not specified.

***

- void Orion.DropHere(['serial'=targetRequest], [count=0(all)]);

Drop the item 'serial' under the character with amount 'count'. Request target to be aimed at the desired object, if parameters were not specified.

***

- void Orion.MoveItem(['serial'=targetRequest], [count=0(all)], ['container'=backpack], [x=-1, y=-1], [z=0]);

Move the object 'serial' with amount 'count' to the container 'container' into coordinates x, y, z (z when throwing on the ground), use target if parameters were not specified.

***

- int Orion.GetDistance('serial');

Return distance to the object.

***

- int Orion.GetDistance(x, y);

Return distance to the coordinates.

***

- void Orion.BandageSelf();

Bandageself.

***

- String ClientLastTarget();

Get the state of the global client variable LastTarget.

Result: The string with the serial.

***

- void ClientLastTarget(serial);

Set the state of the client global variable LastTarget to the serial.

***

- String ClientLastAttack();

Get the state of the global client variable LastAttack

Result: The string with the serial.

***

- void ClientLastAttack(serial);

Set the state of the global client variable LastAttack to the serial.

***

- String TargetSystemSerial();

Get the state of the global client variable TargetSystemSerial (from new target system).

Result: The string with the serial.

***

- void TargetSystemSerial(serial);

Set the state of the global client variable TargetSystemSerial (from new target system) to the serial.

***

- void Orion.GetFriendsStatus();

Retrieves statuses of all friends in update range ( required to get updates about their hp etc. ).

***

- void Orion.GetEnemiesStatus();

Retrieves statuses of all enemies in update range ( required to get updates about their hp etc. ).

***

## Introduced in 2.0.7.0

- PositionObject Orion.GetLastTargetPosition();

Retrieves latest coordinates of LastTarget, if object has disappeared - it will retrieve last known coordinates.

Returns: a PositionObject data type.

***

- PositionObject Orion.GetLastAttackPosition();

Retrieves latest coordinates of LastAttack, if object has disappeared - it will retrieve last known coordinates.

Returns: a PositionObject data type.

***

## Introduced in 2.0.8.0

- bool Orion.OpenContainer('serial', ['delay'=600], ['errorTextPattern']);

Open container.

- serial - serial of the container we're opening.

- delay - Maximum delay for container opening action.

- errorTextPattern - Error text. Default: 'reach that|too away'.

Returns: true if container was opened successfully.

***

- bool Orion.ObjectExists('serial');

Returns: true if object with 'serial' is present in OA memory.

***

- String Orion.RequestName('serial', ['delay'=200]);

Requests objects name. If the name is already present, it will return immediately. Otherwise name will be requested from the server.

- serial - serial of the object we're requesting name from.

- delay - Max delay for name requesting.

Returns: Objects name or an empty string if failed.
***

## Introduced in 2.0.12.0

- bool Orion.GetProfile('serial', ['delay'=300], ['errorTextPattern']);

Retrieves characters profile.

- serial - characters serial.

- delay - maximum wait time for profile retrievement.

- errorTextPattern - error pattern, default: 'reach that|too away'.

Returns true if a profile was retrieved.
***

## Introduced in 2.0.13.0

- void Orion.ShowStatusbar('serial', x, y, [minimized=true]);

Show/Move status bar gump in client screen.

serial - character serial.

x - screen X coordinate.

y - screen Y coordinate.

minimized - only for your character. true will show minimized status bar, false will show expanded one.

***

- void Orion.CloseStatusbar('serial');

Close status bar which belongs to serial.


