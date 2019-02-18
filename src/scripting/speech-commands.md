# Speech

### Command Format

NameSpace.name(requiredParameters, [optionalParameters=defaultValue]);

***

- void Orion.Print(['color'], 'text');

Prints 'text' string into system chat.

If only 'text' string was passed, default color [no color] will be used.

color - message color.

text - message text.

***

- void Orion.CharPrint('serial', 'color', 'text');

Print a message above character with given serial.

serial - given character serial.

color - message color.

text - message text.

***

- void Orion.Say('text');

Display 'text' speech in client.

***

- void Orion.SetFontColor(state, ['color'=0x02B2]);

Changes font color of YOUR character to given color argument ( if given ) and disables/enables this feature by state argument.

state - can be either true or false.

color - message color.

***

- bool Orion.GetFontColor();

Returns state of Orion.SetFontColor() option.

***

- String Orion.GetFontColorValue();

Returns color value of Orion.SetFontColor() option.

***

- void Orion.SetCharactersFontColor(state, ['color'=0x02B2]);

Changes font color of all characters to a given color argument ( if given ) and disables/enables this feature by state argument.

state - can be either true or false.

color - message color.

***

- bool Orion.GetCharactersFontColor();

Returns state of Orion.SetCharactersFontColor() option.

***

- String Orion.GetCharactersFontColorValue();

Returns color value of Orion.SetCharactersFontColor() option.

***

## Introduced in 2.0.15.0

- void Orion.SayYell('some text');

Do 'yelling' speech.

***

- void Orion.SayWhisper('some text');

Do 'whisper' speech.

***

- void Orion.SayEmote('some text');

Do 'emote' speech.

***

- void Orion.SayBroadcast('some text');

Do 'broadcast' speech.

***

- void Orion.SayParty('some text');

Send 'text' to party chat.

***

- void Orion.SayGuild('some text');

Send 'text' to guild chat.

***

- void Orion.SayAlliance('some text');

Send 'text' to alliance chat.
