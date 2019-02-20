# Context Menu

### Command Format

**NameSpace**.**name**(_**requiredParameters**_, [_optionalParameters=defaultValue_]);
</br></br>
***
</br>
_void_ **Orion.RequestContextMenu**('serial');

Send a context menu request for given serial.
</br></br>
***
</br>
_void_ **Orion.WaitContextMenu**('serial', index);

Add context menu wait hook.

- `serial` - serial of context menu object. If serial equals 0, serial check will be ignored.

- `index` - index of context menu choice, starting with 0.
</br></br>
***
</br>
_void_ **Orion.CancelContextMenu**();

Cancel all context menu hooks.
</br></br>
***
</br>
_bool_ **Orion.WaitForContextMenu**([delay=1000]);

Awaits context menu for 'delay' amount of time in ms.

Returns true is context menu was received during this period.
