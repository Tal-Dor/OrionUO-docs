# Gump Object

`Version: 2.0.8.2`

### Command Format

NameSpace.name(requiredParameters, [optionalParameters=defaultValue]);

***

- int gump.Serial();

Returns gump serial.

***

- int gump.ID();

Returns gump id.

***

- int gump.X();

Returns gumps X screen coordinate.

***

- int gump.Y();

Returns gumps Y screen coordinate.

***

- bool gump.Replayed();

Returns true If gump response was already made.

***

- int gump.ReplyID();

Returns response button id if Replayed() was true.

***

- StringList gump.ButtonList();

Returns a list of all buttons within a gump.

***

- StringList gump.CheckboxList();

Returns a list with all checkboxes within a gump.

***

- StringList gump.RadioList();

Returns a list with all radio buttons within a gump.

***

- StringList gump.TilepicList();

Returns a list with all tile pics within a gump.

***

- StringList gump.GumppicList();

Returns a list with all gump pics within a gump.

***

- StringList gump.EntriesList();

Returns a list with all text entries within a gump.

***

- StringList gump.CommandList();

Returns a list with all commands within a gump ( in same order as received from server ).


***

- StringList gump.TextList();

Returns a list with all strings within a gump ( in same order as received from server ).

***

- String gump.Command(index);

Returns gump command by index.

***

- String gump.Text(index);

Returns gump textby index.

***

- bool gump.Select(hook);

Selects gump by a hook object (GumpHookObject).

Returns true if successfull.

***

- void gump.Close();
