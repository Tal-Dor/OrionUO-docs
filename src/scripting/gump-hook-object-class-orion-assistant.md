# Gump Hook

`Version: 2.0.8.2`

### Command Format

NameSpace.name(requiredParameters, [optionalParameters=defaultValue]);

***

- int hook.Index();

Returns button index to select by this hook.

***

- void hook.AddEntry(index, 'text');

Adds a TextEntry hook by index and inputs text string.

index - index of text entry.

text - text entry input string.
***

- void hook.AddCheck(index, state);

Adds a hook for radio/checkbox and sets the state.

index - button index.

state - input state ( true/false).
