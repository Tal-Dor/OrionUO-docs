# Prompt

### Command Format

**NameSpace**.**name**(_**requiredParameters**_, [_optionalParameters=defaultValue_]);
</br></br>
***
</br>
_void_ **Orion.WaitPrompt**('text', 'serial'=0, 'type'=all);

Add a prompt hook.

- `text` - input text

- `serial` - serial of prompt object. If serial equals 0, serial check will be ignored.

- `type` - prompt type:
    - `all` - all types;
    - `ascii` - only ASCII prompts;
    - `unicode` - only UNIDCODE prompts;
</br></br>
***
</br>
_void_ **Orion.CancelWaitPrompt**();

Cancel all prompt hooks.
</br></br>
***
</br>
_bool_ **Orion.PrompsExists**();

Returns true if a prompt is active.
</br></br>
***
</br>
_String_ **Orion.PromptSerial**();

Returns prompt serial as string.
</br></br>
***
</br>
_String_ **Orion.PromptID**();

Returns prompt id as string.
</br></br>
***
</br>
_void_ **Orion.SendPrompt**('text');

Send prompt response ( if there's a prompt active ) with text input.
