# Speech

### Command Format

**NameSpace**.**name**(_**requiredParameters**_, [_optionalParameters=defaultValue_]);
</br></br>
***
</br>
_void_ **Orion.Print**(['color'], 'text');

Prints 'text' string into system chat.

If only 'text' string was passed, default color [no color] will be used.

`color` - message color.

`text` - message text.
</br></br>
***
</br>
_void_ **Orion.CharPrint**('serial', 'color', 'text');

Print a message above character with given serial.

`serial` - given character serial.

`color` - message color.

`text` - message text.
</br></br>
***
</br>
_void_ **Orion.Say**('text');

Display 'text' speech in client.
</br></br>
***
</br>
_void_ **Orion.SetFontColor**(state, ['color'=0x02B2]);

Changes font color of YOUR character to given color argument ( if given ) and disables/enables this feature by state argument.

`state` - can be either true or false.

`color` - message color.
</br></br>
***
</br>
_bool_ **Orion.GetFontColor**();

Returns state of Orion.SetFontColor() option.
</br></br>
***
</br>
_String_ **Orion.GetFontColorValue**();

Returns color value of Orion.SetFontColor() option.
</br></br>
***
</br>
_void_ **Orion.SetCharactersFontColor**(state, ['color'=0x02B2]);

Changes font color of all characters to a given color argument ( if given ) and disables/enables this feature by state argument.

`state` - can be either true or false.

`color` - message color.
</br></br>
***
</br>
_bool_ **Orion.GetCharactersFontColor**();

Returns state of Orion.SetCharactersFontColor() option.
</br></br>
***
</br>
_String_ **Orion.GetCharactersFontColorValue**();

Returns color value of Orion.SetCharactersFontColor() option.
</br></br>
***
</br>
_void_ **Orion.SayYell**('some text');

Do 'yelling' speech.
</br></br>
***
</br>
_void_ **Orion.SayWhisper**('some text');

Do 'whisper' speech.
</br></br>
***
</br>
_void_ **Orion.SayEmote**('some text');

Do 'emote' speech.
</br></br>
***
</br>
_void_ **Orion.SayBroadcast**('some text');

Do 'broadcast' speech.
</br></br>
***
</br>
_void_ **Orion.SayParty**('some text');

Send 'text' to party chat.
</br></br>
***
</br>
_void_ **Orion.SayGuild**('some text');

Send 'text' to guild chat.
</br></br>
***
</br>
_void_ **Orion.SayAlliance**('some text');

Send 'text' to alliance chat.
