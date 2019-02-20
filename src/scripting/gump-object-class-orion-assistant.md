# Gump Object

### Command Format

**NameSpace**.**name**(_**requiredParameters**_, [_optionalParameters=defaultValue_]);
</br></br>
***
</br>
_int_ **gump.Serial**();

Returns gump serial.
</br></br>
***
</br>
_int_ **gump.ID**();

Returns gump id.
</br></br>
***
</br>
_int_ **gump.X**();

Returns gumps X screen coordinate.
</br></br>
***
</br>
_int_ **gump.Y**();

Returns gumps Y screen coordinate.
</br></br>
***
</br>
_bool_ **gump.Replayed**();

Returns true If gump response was already made.
</br></br>
***
</br>
_int_ **gump.ReplyID**();

Returns response button id if Replayed() was true.
</br></br>
***
</br>
_StringList_ **gump.ButtonList**();

Returns a list of all buttons within a gump.
</br></br>
***
</br>
_StringList_ **gump.CheckboxList**();

Returns a list with all checkboxes within a gump.
</br></br>
***
</br>
_StringList_ **gump.RadioList**();

Returns a list with all radio buttons within a gump.
</br></br>
***
</br>
_StringList_ **gump.TilepicList**();

Returns a list with all tile pics within a gump.
</br></br>
***
</br>
_StringList_ **gump.GumppicList**();

Returns a list with all gump pics within a gump.
</br></br>
***
</br>
_StringList_ **gump.EntriesList**();

Returns a list with all text entries within a gump.
</br></br>
***
</br>
_StringList_ **gump.CommandList**();

Returns a list with all commands within a gump ( in same order as received from server ).

</br></br>
***
</br>
_StringList_ **gump.TextList**();

Returns a list with all strings within a gump ( in same order as received from server ).
</br></br>
***
</br>
_String_ **gump.Command**(index);

Returns gump command by index.
</br></br>
***
</br>
_String_ **gump.Text**(index);

Returns gump textby index.
</br></br>
***
</br>
_bool_ **gump.Select**(hook);

Selects gump by a hook object (GumpHookObject).

Returns true if successfull.
</br></br>
***
</br>
_void_ **gump.Close**();
