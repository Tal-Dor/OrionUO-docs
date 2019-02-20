# Timers

### Command Format

**NameSpace**.**name**(_**requiredParameters**_, [_optionalParameters=defaultValue_]);
</br></br>
***
</br>
_bool_ **Orion.TimerExists**('name');

Check if timer with given name exists.

Returns true if such timer exists.</br></br>
***
</br>
_void_ **Orion.SetTimer**('name', [delay=0]);

Create/Change timer with 'delay' as initial value. Default is 0.
</br></br>
***
</br>
_int_ **Orion.Timer**('name');

Get current value of timer by name.

Returns -1 if such timer doesn't exist .

Returns time passed from timer initiation in ms.
</br></br>
***
</br>
_void_ **Orion.RemoveTimer**('name');

Removes timer with a given name.
</br></br>
***
</br>
_void_ **Orion.ClearTimers**();

Removes all existing timers.
