# Journal Message

### Command Format

**NameSpace**.**name**(_**requiredParameters**_, [_optionalParameters=defaultValue_]);
</br></br>
***
</br>
_String_ **msg.Serial**();

Result: Serial number of an Object, bounded with message.
</br></br>
***
</br>
_int_ **msg.Timer**();

Result: Temporary mark of the message.
</br></br>
***
</br>
_String_ **msg.Color**();

Result: Color of the message.
</br></br>
***
</br>
_String_ **msg.Text**();

Result: Message text.
</br></br>
***
</br>
_int_ **msg.Flags**();

Result: Message flags.
</br></br>
***
</br>
_int_ **msg.FindTextID**();

Result: Text index in search request from 0 to the number of sets in request.
</br></br>
***
</br>
_void_ **msg.SetText**('newText');

Change journal message to 'newText' string.
