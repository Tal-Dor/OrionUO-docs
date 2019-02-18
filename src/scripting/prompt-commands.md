# Prompt

### Command Format

NameSpace.name(requiredParameters, [optionalParameters=defaultValue]);

***

- void Orion.WaitPrompt('text', 'serial'=0, 'type'=all);

Add a prompt hook.

- text - input text

- serial - serial of prompt object. If serial equals 0, serial check will be ignored.

- type - prompt type. all - all types; ascii - only ASCII prompts; unicode - only UNIDCODE prompts;

***

- void Orion.CancelWaitPrompt();

Cancel all prompt hooks.

***

## Introduced in 2.0.14.0

- bool Orion.PrompsExists();

Returns true if a prompt is active.

***

- String Orion.PromptSerial();

Returns prompt serial as string.

***

- String Orion.PromptID();

Returns prompt id as string.

***

- void Orion.SendPrompt('text');

Send prompt response ( if there's a prompt active ) with text input.
