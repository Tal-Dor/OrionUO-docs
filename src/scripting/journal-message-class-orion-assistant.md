# Journal Message

### Command Format

**NameSpace**.**name**(_**requiredParameters**_, [_optionalParameters=defaultValue_]);

***

- String msg.Serial();

Result: Serial number of an Object, bounded with message.

***

- int msg.Timer();

Result: Temporary mark of the message.

***

- String msg.Color();

Result: Color of the message.

***

- String msg.Text();

Result: Message text.

***

- int msg.Flags();

Result: Message flags.

***

- int msg.FindTextID();

Result: Text index in search request from 0 to the number of sets in request.

***

## Introduced in 2.0.8.0

- void msg.SetText('newText');

Change journal message to 'newText' string.