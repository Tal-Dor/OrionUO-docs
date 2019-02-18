# Menu Object

### Command Format

**NameSpace**.**name**(_**requiredParameters**_, [_optionalParameters=defaultValue_]);

***

- String menu.Serial();

Result: Menu serial number.

***

- String menu.ID();

Result: Menu identifier number.

***

- String menu.Name();

Result: Menu name.

***

- bool menu.IsGrayMenu();

Result: Gray Menu (chart) or normal.

***

- void menu.Select(index);

Choose menu by index element under current menu.

***

- void menu.Select('name');

Choose menu by item name under current menu.

***

- void menu.Close();

Close current menu without changes.

***

- int menu.ItemsCount();

Result: Item quantity in the menu.

***

- int menu.ItemID(index);

Result: ID of an item menu under specified index.

***

- String menu.ItemGraphic(index);

Result: Graphic of an item menu under specified index.

***

- String menu.ItemColor(index);

Result: Color of an item menu under specified index.

***

- String menu.ItemName(index);

Result: Name of an item menu under specified index.
