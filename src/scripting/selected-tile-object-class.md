# Selected Tile

**SelectedTileis a static reference just like Orion so you can always get it.
You can reassign this reference by targeting something.**

***

### Command Format

NameSpace.name(requiredParameters, [optionalParameters=defaultValue]);

***

- String SelectedTile.Serial();

Returns serial of selected tile ( if it's an in-game item, not land art ).

***

- String SelectedTile.Graphic();

Returns graphic id/type of selected tile.

***

- String SelectedTile.Color();

Returns color of selected tile.

***

- int SelectedTile.X();

Returns x coordinate value of selected tile.

***

- int SelectedTile.Y();

Returns y coordinate value of selected tile.

***

- int SelectedTile.Z();

Returns z coordinate value of selected tile.

***

- String SelectedTile.LandGraphic();

Returns graphics id/type of land art of selected tile.

***

- int SelectedTile.LandX();

Returns land x coordinate ( will be same as SelectedTile.X() )

***

- int SelectedTile.LandY();

Returns land y coordinate ( will be same as SelectedTile.Y() )

***

- int SelectedTile.LandZ();

Returns land z coordinate ( CAN BE different from SelectedTile.Z() )

***

- bool SelectedTile.IsLandTile();

Returns true if this is a land tile.

***

- bool SelectedTile.IsStaticTile();

Returns true if this is a static/multi tile.

***

- bool SelectedTile.IsGameObject();

Returns true if this is a game object.
