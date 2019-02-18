# Interactions With Other Scripts

### Command Format

**NameSpace**.**name**(_**requiredParameters**_, [_optionalParameters=defaultValue_]);

***

- void Orion.Wait('delay');

Wait delay (milliseconds).

In addition, the value can take in the parameter string constants: moveitemdelay, waittargetdelay, useitemdelay, keepcorpsedelay.

***

- int Orion.Now();

Result: the current time in milliseconds.

***

- void Orion.LoadScript('filePath');

Load the script file.

***

- void Orion.Exec('functionName', [oneScriptRunning=false], [argumentsList]);

Start the function.

- - functionName - The name of the function to start.

- - oneScriptRunning - Check for a running instance of the function with the same name and prevent re-execution.

- - argumentsList - List of function parameters.

***

- void Orion.Terminate('functionName', ['functionsSave']);

Terminate the script. The function name register is important !!!

- - functionName - The name of the function to be terminated. Ends all functions with that name. If 'all' is specified - exits all functions except those that were specified in functionsSave.

- - functionsSave - Functions that do not need to be terminated are indicated by '|' ; For example, Orion.Terminate ('all', 'Heal | Loot | CheckMana') - terminates all working functions except Heal, Loot, CheckMana.

***

- bool Orion.ScriptRunning('functionName');

Check if the script is already running.

Result: true if the script is running.

***

## Introduced in 2.0.7.0

- void Orion.Launch('filePath', [arguments]);

Launching of external program from 'filePath' with optional 'arguments'.

***

- bool Orion.Contains(text, pattern, [ignoreCase=false]);

This function will check for a text pattern or a collection of patters ('patternOne|patternTwo|patternThree') within 'text' string.
Uses same logic as text searching in UO journal.

- - text - String with text to search within.

- - pattern - String with pattern(s) to search for.

- - ignoreCase - true - Ignore case is true by default.

Returns true if there's a match.

***

- StringList Orion.Split(text, [separator=' '], [skipEmptyWord=true]);

This function will split 'text' string into a list of strings by separator character. Default is space character.

- - text - string of text to split.

- - separator - character used as a separator for text string.

- - skipEmptyWord - true - skips empty words by default.

Returns a list of strings.

***

## Introduced in 2.0.8.0

- String Orion.OAVersion();

Returns: Current version number of OA, for example "2.0.8.0".

***

- bool Orion.Connected();

Returns: true if client is connected to a server and character is already in the world.

***

- String Orion.Time(['format'=hh:mm:ss.zzz]);

Returns: current time, example "13:27:41.508".

***

- String Orion.Date(['format'=dd.MM.yyyy]);

Returns: current date, example "26.05.2017".

***

- int Orion.Random([value=2147483647]);

Returns: random value starting from 0 and up to value-1.

***

- int Orion.Random(minValue, maxValue);

Returns: random value starting from minValue and up to maxValue-1.

***

## Introduced in 2.0.15.0

- void Orion.ActivateClient();

Activates client window.

***

- void Orion.ShutdownWindows(['mode']);

Shuts down your PC :) can add flags as 'mode'.

***

- bool Orion.OnOffHotkeys();

Get current state of hotkeys ( enabled/disabled )

Returns true if hotkeys are enabled, false if disabled.

***

- void Orion.OnOffHotkeys(state);

Sets hotkeys state.