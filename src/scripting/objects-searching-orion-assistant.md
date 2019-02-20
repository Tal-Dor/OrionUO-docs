# Objects Searching

### Command Format

**NameSpace**.**name**(_**requiredParameters**_, [_optionalParameters=defaultValue_]);
</br></br>
***
</br>
**flags** - search filters:

- `fast` - the search stops on the first found object;

- `near` - search for the nearest object to the character;

- `mobile` - search only for alive creatures;

- `item` - search only inanimate objects;

- `human` - search only for humanoid creatures, types: 0x0190-0x0193, 0x03DB, 0x03DF and 0x03E2;

- `live` - search only for living creatures;

- `dead` - search only for dead creatures, types: 0x0192 and 0x0193.

- `injured` - Searching for a friend with lowest HP (works only for FindFriend/FindEnemy).

- `next` - Searching for next object (works only for FindFriend/FindEnemy).

- `ignorefriends` - ignores friends(Introduced in OA 2.0.8.0).

- `ignoreenemies` - ignores enemies (Introduced in OA 2.0.8.0).

_When using human, live or dead - mobile flag is set automatically._

_When using next - fast flag is set automatically._
</br></br>
***
</br>
**notoriety** - Wickedness of the desired character.

- innocent/blue

- friendly/green

- gray

- criminal

- enemy/orange

- murderer/red

- invulnerable/yellow
</br></br>
***
</br>
**distance** - The search distance.

In addition to numerical values, it can take string constants: finddistance, usedistance, opencorpsedistance.
</br></br>
***
</br>
_void_ **Orion.UseType**('graphic', ['color'=0xFFFF], ['container'=self], [recurse=true]);

Search for an object by type and color in the container.

 - `graphic` - Type or list of types. 0xFFFF is ignored.

 - `color` - The color or list of colors. 0xFFFF is ignored.

 - `container` - The container in which the search is performed.

 - `recurse` - Recursive search for sub-containers.
</br></br>
***
</br>
_void_ **Orion.UseFromGround**('graphic', ['color'=0xFFFF], ['distance'=useObjectsDistance], ['flags']);

Search for an object by type and color on the ground.

 - `graphic` - Type or list of types. 0xFFFF is ignored.

 - `color` - The color or list of colors. 0xFFFF is ignored.

 - `distance` - The search distance.

 - `flags` - Search filter flags.
</br></br>
***
</br>
_bool_ **Orion.UseTypeList**('listName', ['container'=self], [recurse=true]);

Search for an object from the find list in the container.

 - `listName` - The name of the find list.

 - `container` - The container in which the search is performed.

 - `recurse` - Recursive search for sub-containers.

Result: true if the object was found and used.
</br></br>
***
</br>
_bool_ **Orion.UseFromGroundList**('listName', ['distance'=useObjectsDistance], ['flags']);

Search for an object on the find list on the ground.

 - `listName` - The name of the find list.

 - `distance` - The search distance.

 - `flags` - Search filter flags.

Result: true if the object was found and used.
</br></br>
***
</br>
_StringList_ **Orion.FindType**('graphic', ['color'=0xFFFF], ['container'=backpack], ['flags'], ['distance'=searchObjectsDistance], ['notoriety'], [recurse=true]);

Search for an object by type and color.

- `graphic` - Type or list of types. 0xFFFF is ignored.

- `color` - The color or list of colors. 0xFFFF is ignored.

- `container` - The container in which the search is performed.

- `flags` - Search filter flags.

- `distance` - The search distance.

- `notoriety` - Wickedness of the desired character.

- `recurse` - Recursive search for sub-containers.

Result: List of found serials.
</br></br>
***
</br>
_void_ **Orion.Ignore**('serial', [state=true]);

Set / remove the ignore flag on the serial object.
</br></br>
***
</br>
_void_ **Orion.IgnoreReset**();

Remove the ignore flag from all objects.
</br></br>
***
</br>
_GameObject_ **Orion.FindObject**('serial');

Result: an object of type _GameObject_ or null.
</br></br>
***
</br>
_int_ **Orion.Count**('graphic', ['color'=0xFFFF], ['container'=self], ['distance'=searchObjectsDistance], [recurse]);

Returns the total number of items (the number of items, not the number of objects found).

- `graphic` - Type or list of types. 0xFFFF is ignored.

- `color` - The color or list of colors. 0xFFFF is ignored.

- `container` - The container in which the search is performed.

- `distance` - The search distance.

- `recurse` - Recursive search for sub-containers.

Result: the amount of items.
</br></br>
***
</br>
_void_ **Orion.ResetIgnoreList**();

Reset the use of the ignore list.
</br></br>
***
</br>
_void_ **Orion.UseIgnoreList**('listName');

Use ignore list listName.
</br></br>
***
</br>
_StringList_ **Orion.FindList**('listName', ['container'=backpack], ['flags'], ['distance'=searchObjectsDistance], ['notoriety'], [recurse=true]);

Search for an object in the find list.

- `listName` - The name of the find list.

- `container` - The container in which the search is performed.

- `flags` - Search filter flags.

- `distance` - The search distance.

- `notoriety` - Wickedness of the desired character.

- `recurse` - Recursive search for sub-containers.
</br></br>
***
</br>
_GameObject_ **Orion.ObjAtLayer**('layerName', ['serial'=self]);

Result: an object of type _GameObject_ in the specified layer of the object 'serial' or null.
</br></br>
***
</br>
_String_ **Orion.FindFriend**(['flags'=fast], ['distance'=searchObjectsDistance]);

Searching for a friend serial from friends list.

- `flags` - Searching filter flags.

- `distance` - Searching distance.
</br></br>
***
</br>
_String_ **Orion.FindEnemy**(['flags'=fast], ['distance'=searchObjectsDistance]);

Searching for an enemy serial from enemies list.

- `flags` - Searching filter flags.

- `distance` - Searching distance.
