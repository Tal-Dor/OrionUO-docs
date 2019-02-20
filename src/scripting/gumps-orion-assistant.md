# Gumps

### Command Format

**NameSpace**.**name**(_**requiredParameters**_, [_optionalParameters=defaultValue_]);
</br></br>
***
</br>
_void_ **Orion.HelpGump**();

Request for the help menu gump of the server.
</br></br>
***
</br>
_void_ **Orion.InfoGump**([index=-1]);

Outputs data of a gump by its index. If index equals -1, last gump is taken.
</br></br>
***
</br>
_GumpHookObjects_ **Orion.CreateGumpHook**('index');

Creates a gump hook object.

index - Return-value of gump button or 'cancel' or a 0 when closing a gump with RMB.
</br></br>
***
</br>
_void_ **Orion.WaitGump**(hook);

Enables a gump hook to catch an incomming gump.

When new hook is enabled by Orion.WaitGump, it will be added to a stack. All previously enabled hooks will be waiting as well.

hook - an object created by Orion.CreateGumpHook.
</br></br>
***
</br>
_void_ **Orion.CancelWaitGump**();

Removes **all **enabled gump hooks .
</br></br>
***
</br>
_int_ **Orion.GumpCount**();

Returns the amount of opened gumps from OA memory.
</br></br>
***
</br>
_GumpObject_ **Orion.GetLastGump**();

Get last gump sent by server.

Returns a GumpObject or a null reference.
</br></br>
***
</br>
_GumpObject_ **Orion.GetGump**(index);

Get gump by an index.

Returns a GumpObject or a null reference.
</br></br>
***
</br>
_GumpObject_ **Orion.GetGump**(serial, id);

Get gump by serial and id.

Returns a GumpObject or a null reference.
</br></br>
***
</br>
_bool_ **Orion.WaitForGump**([delay=1000]);

Enables a gump hook and blocks thread for 'delay' amount of time in ms. Removes gump hook afterwards.

Returns true if a gump was received during delay period.
