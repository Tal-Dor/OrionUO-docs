# Menu Object

### Command Format

**NameSpace**.**name**(_**requiredParameters**_, [_optionalParameters=defaultValue_]);
</br></br>
***
</br>
_String_ **menu.Serial**();

Result: Menu serial number.
</br></br>
***
</br>
_String_ **menu.ID**();

Result: Menu identifier number.
</br></br>
***
</br>
_String_ **menu.Name**();

Result: Menu name.
</br></br>
***
</br>
_bool_ **menu.IsGrayMenu**();

Result: Gray Menu (chart) or normal.
</br></br>
***
</br>
_void_ **menu.Select**(index);

Choose menu by index element under current menu.
</br></br>
***
</br>
_void_ **menu.Select**('name');

Choose menu by item name under current menu.
</br></br>
***
</br>
_void_ **menu.Close**();

Close current menu without changes.
</br></br>
***
</br>
_int_ **menu.ItemsCount**();

Result: Item quantity in the menu.
</br></br>
***
</br>
_int_ **menu.ItemID**(index);

Result: ID of an item menu under specified index.
</br></br>
***
</br>
_String_ **menu.ItemGraphic**(index);

Result: Graphic of an item menu under specified index.
</br></br>
***
</br>
_String_ **menu.ItemColor**(index);

Result: Color of an item menu under specified index.
</br></br>
***
</br>
_String_ **menu.ItemName**(index);

Result: Name of an item menu under specified index.
