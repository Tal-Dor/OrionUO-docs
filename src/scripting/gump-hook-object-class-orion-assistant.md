# Gump Hook

### Command Format

**NameSpace**.**name**(_**requiredParameters**_, [_optionalParameters=defaultValue_]);
</br></br>
***
</br>
_int_ **hook.Index**();

Returns button index to select by this hook.
</br></br>
***
</br>
_void_ **hook.AddEntry**(index, 'text');

Adds a TextEntry hook by index and inputs text string.

index - index of text entry.

text - text entry input string.
</br></br>
***
</br>
_void_ **hook.AddCheck**(index, state);

Adds a hook for radio/checkbox and sets the state.

index - button index.

state - input state ( true/false).
