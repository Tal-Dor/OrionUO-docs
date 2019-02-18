# Map

### Command Format

NameSpace.name(requiredParameters, [optionalParameters=defaultValue]);

***

- void Orion.OpenOrionMap([x, y]);

Opens Orion map.

If x and y were defined, moves map window to given screen coordinates.

***

- void Orion.MoveOrionMap(x, y);

Moves map to given screen coordinates.

***

- void Orion.CloseOrionMap();

Close Orion map.

***

- void Orion.OpenEnhancedMap(['filePath']);

Opens Enchanced Map at 'filePath' (for example "D:\Games\UO\EnhancedMap.exe").

If 'filePath' wasn't defined, tries to open from a default location <UORoot>/Map/EnhancedMap.exe'
