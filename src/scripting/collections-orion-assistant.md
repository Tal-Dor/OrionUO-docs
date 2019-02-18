# Collections

### Command Format

**NameSpace**.**name**(_**requiredParameters**_, [_optionalParameters=defaultValue_]);

***

- void Orion.AddType('typeName', ['typeValue'=targetRequest]);

Add type or select type (if typeValue isn't suggested).

***

- void Orion.RemoveType('typeName');

Delete type.

***

- void Orion.AddObject('objectName', ['objectValue'=targetRequest]);

Add object or select object (if objectValue isn't suggested)

***

- void Orion.RemoveObject('objectName');

Delete object.

***

- void Orion.AddFindList(['listName'=targetRequest], ['graphic', 'color'], ['comment']);

Add object properties or select to add object properties to Find list.

- - listName - list name. If not suggested - target selection appears to add properties to the currently selected element from the list(on the list tab), without auto-save.
- - graphic - object type.
- - color- object color.
- - comment - a comment, which will be displayed in the list.

***

- void Orion.ClearFindList('listName');

Delete search list with all it's content.

- - listName - list name.

***

- void Orion.AddIgnoreListObject(['listName'=targetRequest], ['serial'], ['comment']);

Add object to ignore list.

- - listName - list name.
- - serial - serial of the object..
- - comment - a comment, which will be displayed in the list.

***

- void Orion.AddIgnoreList(['listName'=targetRequest], ['graphic', 'color'], ['comment']);

Add object properties or target selection appears to add object properties to the ignore list.

- - listName - list name. If not suggested - target selection appears to add properties to the currently selected element from the list(on the list tab), without auto-save
- - graphic - Тип объекта.
- - color- object color.
- - comment - a comment, which will be displayed in the list.

***

- void Orion.ClearIgnoreList('listName');

Delete search list with all it's content.

- - listName - list name.

***

- StringList Orion.GetFriendList();

Return string list with friends id's.

***

- StringList Orion.GetEnemyList();

Return string list with enemies id's.

***

- void Orion.AddFriend('friendName', ['serial'=targetRequest]);

Add a friend or select one to add by a target if there's no 'serial' argument.

***

- void Orion.RemoveFriend('friendName');

Remove a friend from friends list.

***

- void Orion.ClearFriendList();

Clear friends list.
***

- void Orion.AddEnemy('enemyName', ['serial'=targetRequest]);

Add an enemy or select one to add by a target if there's no 'serial' argument.

***

- void Orion.RemoveEnemy('enemyName');

Remove an enemy from enemies list.

***

- void Orion.ClearEnemyList();

Clear enemies list.

***

- void Orion.SetGlobal(name, value);

Set a global variable. Value data type is always a string.

***

- String Orion.GetGlobal(name);

Retrieve value ( string data type ) of a global variable

Returns value of the variable or an empty string is no variable is found with such name.

***

- void Orion.ClearGlobals();

Clear global variables list.