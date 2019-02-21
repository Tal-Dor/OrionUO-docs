# Targeting

### Command Format

**NameSpace**.**name**(_**requiredParameters**_, [_optionalParameters=defaultValue_]);
</br></br>
***
</br>
**graphicOrFlags** - searching filter:

- `mine` - searching for cave tiles;

- `tree` - searching for trees;

- `water` - searching for water tiles;

- `land` - searching for only land tiles;

- `any` - searching of any type of tile (static tiles have higher priority over landscape).
</br></br>
***
</br>
_bool_ **Orion.HaveTarget**();

Have a target.

Resul: true if target is on.
</br></br>
***
</br>
_void_ **Orion.WaitTargetObject**('serial');

Set the target trap for object(s) serial.
</br></br>
***
</br>
_void_ **Orion.WaitTargetType**('graphic', ['color'=0xFFFF], ['container'=self], ['flags'], [recurse=true]);

Set the target trap for object, found by searching container.

- `graphic` - Type or type list for search. 0xFFFF ignored.

- `color` - Colour or Colour list for search. 0xFFFF ignored.

- `container` - Searched Container.

- `flags` - Flag Search Filters.

- `recurse` - Recursive Search in subcontainers.
</br></br>
***
</br>
_void_ **Orion.WaitTargetGround**('graphic', ['color'=0xFFFF], ['distance'=searchObjectsDistance], ['flags']);

Set the target trap for object found by search on the ground.

- `graphic` - Type or type list for search. 0xFFFF ignored.

- `color` - Colour or Colour list for search. 0xFFFF ignored.

- `distance` - Search Distance.

- `flags` - Flag Search Filters.
</br></br>
***
</br>
_void_ **Orion.WaitTargetTypeList**('findListName', ['container'=self], ['flags'], [recurse=true]);

Set the target trap for object, found by searching container.

- `findListName` - Search list name.

- `container` - Container being searched.

- `flags` - Flag Search Filters.

- `recurse` - Recursive Search in subcontainers.
</br></br>
***
</br>
_void_ **Orion.WaitTargetGroundList**('findListName', ['distance'=searchObjectsDistance], ['flags']);

Set the target trap for object found by searching the ground.

- `findListName` - Search list name.

- `distance` - Search Distance.

- `flags` - Flag Search Filters.
</br></br>
***
</br>
_void_ **Orion.WaitTargetTile**('graphic', [x, y, z]);

Set the target trap on the ground.

- `graphic` - type of the tile, might be lasttile

- `x` - World X coordinate

- `y` - World Y coordinate

- `z` - World Z coordinate
</br></br>
***
</br>
_void_ **Orion.WaitTargetTileRelative**('graphic', [x, y, z]);

Set the target trap on the ground, against Character.

- `graphic` - type of the tile, might be lasttile

- `x` - X coordinate bias in the world

- `y` - Y coordinate bias in the world

- `z` - Z coordinate bias in the world
</br></br>
***
</br>
_void_ **Orion.CancelWaitTarget**();

Cancel of the current wait of the target.
</br></br>
***
</br>
_void_ **Orion.TargetObject**('serial');

Point the target on a serial object.
</br></br>
***
</br>
_void_ **Orion.TargetType**('graphic', ['color'=0xFFFF], ['container'=self], ['flags'], [recurse=true]);

Point the target on the object found by searching container.

- `graphic` - Type or type list for search. 0xFFFF ignored.

- `color` - Colour or Colour list for search. 0xFFFF ignored.

- `container` - Searched Container.

- `flags` - Flag Search Filters.

- `recurse` - Recursive Search in subcontainers.
</br></br>
***
</br>
_void_ **Orion.TargetGround**('graphic', ['color'=0xFFFF], ['distance'=searchObjectsDistance], ['flags']);

Point the target on the object found by searching the ground.

- `graphic` - Type or type list for search. 0xFFFF ignored.

- `color` - Colour or Colour list for search. 0xFFFF ignored.

- `distance` - Search Distance.

- `flags` - Flag Search Filters.
</br></br>
***
</br>
_void_ **Orion.TargetTypeList**('findListName', ['container'=self], ['flags'], [recurse=true]);

Point the target on the object found by serching container.

- `findListName` - Search list name.

- `container` - Container being searched.

- `flags` - Flag Search Filters.

- `recurse` - Recursive Search in subcontainers.
</br></br>
***
</br>
_void_ **Orion.TargetGroundList**('findListName', ['distance'=searchObjectsDistance], ['flags']);

Point the target on the object found by searching the ground.

- `findListName` - Search list name.

- `distance` - Search Distance.

- `flags` - Flag Search Filters.
</br></br>
***
</br>
_void_ **Orion.TargetTile**('graphic', [x, y, z]);

Point target on a ground.

- `graphic` - type of the tile, might be lasttile

- `x` - World X coordinate

- `y` - World Y coordinate

- `z` - World Z coordinate
</br></br>
***
</br>
_void_ **Orion.TargetTileRelative**('graphic', [x, y, z]);

Point target on a ground against Character.

- `graphic` - type of the tile, might be lasttile

- `x` - X coordinate bias in the world

- `y` - Y coordinate bias in the world

- `z` - Z coordinate bias in the world
</br></br>
***
</br>
_bool_ **Orion.ValidateTargetTile**('graphicOrFlags', x, y);

This function checks if targeted tile is valid for targeting.

- `graphicOrFlags` - tile type by graphic id or flags.

- `x` - X coordinate on the map.

- `y` - Y coordinate on the map.

Returns true if tile is valid for targeting.
</br></br>
***
</br>
_bool_ **Orion.ValidateTargetTileRelative**('graphicOrFlags', x, y);

This function checks if targeted tile( relative to character position on the map ) is valid for targeting.

- `graphicOrFlags` - tile type by graphic id or flags.

- `x` - X offset on the map.

- `y` - Y offset on the map.

Returns true if tile is valid for targeting.
</br></br>
***
</br>
_void_ **Orion.CancalTarget**();

Cancels current target ( if present in client ).
</br></br>
***
</br>
_bool_ **Orion.WaitForTarget**([delay=1000]);

Awaits ( blocks execution ) for a target for 'delay' amount of time.

If client had a target already, immediately returns true.
</br></br>
***
</br>
_int_ **Orion.GetTargetType**();

Get type of target.

Returns: 0 if there's no target, 1 - neutral, 2 - harmful, 3 - helpful.
