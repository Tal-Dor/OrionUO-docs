# Collections

### Command Format

**NameSpace**.**name**(_**requiredParameters**_, [_optionalParameters=defaultValue_]);
</br></br>
***
</br>
_void_ **Orion.AddType**('typeName', ['typeValue'=targetRequest]);

Add type or select type (if typeValue isn't suggested).
</br></br>
***
</br>
_void_ **Orion.RemoveType**('typeName');

Delete type.
</br></br>
***
</br>
_void_ **Orion.AddObject**('objectName', ['objectValue'=targetRequest]);

Add object or select object (if objectValue isn't suggested)
</br></br>
***
</br>
_void_ **Orion.RemoveObject**('objectName');

Delete object.
</br></br>
***
</br>
_void_ **Orion.AddFindList**(['listName'=targetRequest], ['graphic', 'color'], ['comment']);

Add object properties or select to add object properties to Find list.

- `listName` - list name. If not suggested - target selection appears to add properties to the currently selected element from the list(on the list tab), without auto-save.
- `graphic` - object type.
- `color` - object color.
- `comment` - a comment, which will be displayed in the list.
</br></br>
***
</br>
_void_ **Orion.ClearFindList**('listName');

Delete search list with all it's content.

- **listName** - list name.
</br></br>
***
</br>
_void_ **Orion.AddIgnoreListObject**(['listName'=targetRequest], ['serial'], ['comment']);

Add object to ignore list.

- `listName` - list name.
- `serial` - serial of the object..
- `comment` - a comment, which will be displayed in the list.
</br></br>
***
</br>
_void_ **Orion.AddIgnoreList**(['listName'=targetRequest], ['graphic', 'color'], ['comment']);

Add object properties or target selection appears to add object properties to the ignore list.

- `listName` - list name. If not suggested - target selection appears to add properties to the currently selected element from the list(on the list tab), without auto-save
- `graphic` - Тип объекта.
- `color`- object color.
- `comment` - a comment, which will be displayed in the list.
</br></br>
***
</br>
_void_ **Orion.ClearIgnoreList**('listName');

Delete search list with all it's content.

- `listName` - list name.
</br></br>
***
</br>
_StringList_ **Orion.GetFriendList**();

Return string list with friends id's.
</br></br>
***
</br>
_StringList_ **Orion.GetEnemyList**();

Return string list with enemies id's.
</br></br>
***
</br>
_void_ **Orion.AddFriend**('friendName', ['serial'=targetRequest]);

Add a friend or select one to add by a target if there's no 'serial' argument.
</br></br>
***
</br>
_void_ **Orion.RemoveFriend**('friendName');

Remove a friend from friends list.
</br></br>
***
</br>
_void_ **Orion.ClearFriendList**();

Clear friends list.
</br></br>
***
</br>
_void_ **Orion.AddEnemy**('enemyName', ['serial'=targetRequest]);

Add an enemy or select one to add by a target if there's no 'serial' argument.
</br></br>
***
</br>
_void_ **Orion.RemoveEnemy**('enemyName');

Remove an enemy from enemies list.
</br></br>
***
</br>
_void_ **Orion.ClearEnemyList**();

Clear enemies list.
</br></br>
***
</br>
_void_ **Orion.SetGlobal**(name, value);

Set a global variable. Value data type is always a string.
</br></br>
***
</br>
_String_ **Orion.GetGlobal**(name);

Retrieve value ( string data type ) of a global variable

Returns value of the variable or an empty string is no variable is found with such name.
</br></br>
***
</br>
_void_ **Orion.ClearGlobals**();

Clear global variables list.
