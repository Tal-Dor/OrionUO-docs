# Timers

### Command Format

NameSpace.name(requiredParameters, [optionalParameters=defaultValue]);

***

- bool Orion.TimerExists('name');

Check if timer with given name exists.

Returns true if such timer exists.
***

- void Orion.SetTimer('name', [delay=0]);

Create/Change timer with 'delay' as initial value. Default is 0.

***

- int Orion.Timer('name');

Get current value of timer by name.

Returns -1 if such timer doesn't exist .

Returns time passed from timer initiation in ms.

***

- void Orion.RemoveTimer('name');

Removes timer with a given name.

***

- void Orion.ClearTimers();

Removes all existing timers.
