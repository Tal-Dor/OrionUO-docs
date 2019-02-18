# Gumps

### Command Format

**NameSpace**.**name**(_**requiredParameters**_, [_optionalParameters=defaultValue_]);

***

- void Orion.HelpGump();

Request for the help menu gump of the server.

***

## Introduced in 2.0.7.0

- void Orion.InfoGump([index=-1]);

Outputs data of a gump by its index. If index equals -1, last gump is taken.
***

## Introduced in 2.0.8.2

- GumpHookObjects Orion.CreateGumpHook('index');

Creates a gump hook object.

index - Return-value of gump button or 'cancel' or a 0 when closing a gump with RMB.

***

- void Orion.WaitGump(hook);

Enables a gump hook to catch an incomming gump.

When new hook is enabled by Orion.WaitGump, it will be added to a stack. All previously enabled hooks will be waiting as well.

hook - an object created by Orion.CreateGumpHook.

***

- void Orion.CancelWaitGump();

Removes **all **enabled gump hooks .

***

- int Orion.GumpCount();

Returns the amount of opened gumps from OA memory.

***

- GumpObject Orion.GetLastGump();

Get last gump sent by server.

Returns a GumpObject or a null reference.

***

- GumpObject Orion.GetGump(index);

Get gump by an index.

Returns a GumpObject or a null reference.

***

- GumpObject Orion.GetGump(serial, id);

Get gump by serial and id.

Returns a GumpObject or a null reference.

***

## Introduced in 2.0.15.0

- bool Orion.WaitForGump([delay=1000]);

Enables a gump hook and blocks thread for 'delay' amount of time in ms. Removes gump hook afterwards.

Returns true if a gump was received during delay period.
