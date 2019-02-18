# Context Menu

### Command Format

NameSpace.name(requiredParameters, [optionalParameters=defaultValue]);

***

- void Orion.RequestContextMenu('serial');

Send a context menu request for given serial.

***

- void Orion.WaitContextMenu('serial', index);

Add context menu wait hook.

- serial - serial of context menu object. If serial equals 0, serial check will be ignored.

- index - index of context menu choice, starting with 0.

***

- void Orion.CancelContextMenu();

Cancel all context menu hooks.

***

## Introduced in 2.0.15.0

- bool Orion.WaitForContextMenu([delay=1000]);

Awaits context menu for 'delay' amount of time in ms.

Returns true is context menu was received during this period.
