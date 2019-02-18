# Menu

### Command Format

**NameSpace**.**name**(_**requiredParameters**_, [_optionalParameters=defaultValue_]);

***

- void Orion.InfoMenu();

Display information about the content of the last menu in the journal that came from the server.

(Introduced in OA 2.0.8.0) index - gump index, -1 or lastmenu will display information about last gump ( if it was there ).

***

- void Orion.WaitMenu('prompt', 'choice');

Waiting for the menu with the title 'prompt' to select object 'choice'.

(Introduced in OA 2.0.8.0) Choice can be numeric, it will chose a choice according to its index. You can also use 'random' - to get a random one.

***

- void Orion.CancelWaitMenu();

Cancel the menu waiting.

***

- int Orion.MenuCount();

Information about the number of open menus.

Result: the amount of open menus.

***

- MenuObject Orion.GetMenu('nameOrIndex');

Get the menu object by name/index.

Result: the object of type MenuObject or null if the menu with the specified name or index does not exist.

***

- void Orion.SelectMenu('name', 'itemName');

Make a choice in the client's open menu - 'name' of the item that named itemName.

***

- void Orion.CloseMenu('name');

Close the open menu 'name' in the client.

***

## Introduced in 2.0.15.0

- bool Orion.WaitForMenu([delay=1000]);

Awaits ( blocks execution ) for a menu for a given 'delay' of time in ms.

Returns true is a menu was received during the given delay.