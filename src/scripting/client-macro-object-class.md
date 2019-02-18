# Client Macro Object Class

### Command Format

`NameSpace.name(requiredParameters, [optionalParameters=defaultValue]);`

***

#### MacroObject Orion.CreateClientMacro('action', ['subAction']);

Creates a MacroObject instance with gives action and possible subactions.

`Returns` a MacroObject object.


Example:

```javascript
//This creates a 'BandageSelf' client macro and instantly executes it.
Orion.CreateClientMacro('BandageSelf').Play(false, 1000);
```
***

#### void macro.AddAction('action', ['subAction']);

Add action entry to macros.

***

#### void macro.Play([waitWhileMacroPlaying=false], [delay=100500]);

Play macro in client.

Attention! Only 1 macro can be played in client at a time!

Multiple requests to play a macro while there's a macro already playing will cancel each other out. Last requested macro will be played.


`waitWhileMacroPlaying` Will wait if there's a macro already playing.

`delay` Delay to wait for current macro completion.
