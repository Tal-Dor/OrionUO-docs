# Selected Tile

**SelectedTile is a static reference just like Orion so you can always get it.
You can reassign this reference by targeting something.**
</br></br>
***
### Command Format

**NameSpace**.**name**(_**requiredParameters**_, [_optionalParameters=defaultValue_]);
</br></br>
***
</br>
_String_ **SelectedTile.Serial**();

Returns serial of selected tile ( if it's an in-game item, not land art ).
</br></br>
***
</br>
_String_ **SelectedTile.Graphic**();

Returns graphic id/type of selected tile.
</br></br>
***
</br>
_String_ **SelectedTile.Color**();

Returns color of selected tile.
</br></br>
***
</br>
_int_ **SelectedTile.X**();

Returns x coordinate value of selected tile.
</br></br>
***
</br>
_int_ **SelectedTile.Y**();

Returns y coordinate value of selected tile.
</br></br>
***
</br>
_int_ **SelectedTile.Z**();

Returns z coordinate value of selected tile.
</br></br>
***
</br>
_String_ **SelectedTile.LandGraphic**();

Returns graphics id/type of land art of selected tile.
</br></br>
***
</br>
_int_ **SelectedTile.LandX**();

Returns land x coordinate ( will be same as SelectedTile.X() )
</br></br>
***
</br>
_int_ **SelectedTile.LandY**();

Returns land y coordinate ( will be same as SelectedTile.Y() )
</br></br>
***
</br>
_int_ **SelectedTile.LandZ**();

Returns land z coordinate ( CAN BE different from SelectedTile.Z() )
</br></br>
***
</br>
_bool_ **SelectedTile.IsLandTile**();

Returns true if this is a land tile.
</br></br>
***
</br>
_bool_ **SelectedTile.IsStaticTile**();

Returns true if this is a static/multi tile.
</br></br>
***
</br>
_bool_ **SelectedTile.IsGameObject**();

Returns true if this is a game object.
