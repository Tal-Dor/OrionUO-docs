# Map

### Command Format

**NameSpace**.**name**(_**requiredParameters**_, [_optionalParameters=defaultValue_]);
</br></br>
***
</br>
_void_ **Orion.OpenOrionMap**([x, y]);

Opens Orion map.

If x and y were defined, moves map window to given screen coordinates.
</br></br>
***
</br>
_void_ **Orion.MoveOrionMap**(x, y);

Moves map to given screen coordinates.
</br></br>
***
</br>
_void_ **Orion.CloseOrionMap**();

Close Orion map.
</br></br>
***
</br>
_void_ **Orion.OpenEnhancedMap**(['filePath']);

Opens Enchanced Map at 'filePath' (for example "D:\Games\UO\EnhancedMap.exe").

If 'filePath' wasn't defined, tries to open from a default location <UORoot>/Map/EnhancedMap.exe'
