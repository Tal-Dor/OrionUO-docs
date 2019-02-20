# Journal

### Command Format

**NameSpace**.**name**(_**requiredParameters**_, [_optionalParameters=defaultValue_]);
</br></br>
***
</br>
_void_ **Orion.ShowJournal**([linesCount=maxLines]);

Display the journal content in a text box, linesCount - the number of output lines.
</br></br>
***
</br>
_void_ **Orion.ClearJournal**(['pattern'], ['flags'], ['serial'=0], ['color'=0xFFFF]);

Clear the journal.

Without parameters - clears the whole journal of the assistant; Otherwise it works similarly to InJournal but including deletion.
</br></br>
***
</br>
_void_ **Orion.JournalIgnoreCase**([state=false]);

Enable / disable ignoring the register for searching text in the journal.
</br></br>
***
</br>
_JournalMessage_ **Orion.InJournal**('pattern', ['flags'], ['serial'=0], ['color'=0xFFFF], [startTime=0, endTime=0]);

Search for data in the journal.

- `pattern` - required string, which can consist of several lines separated via |

- `flags` - search flags in the journal: my/self - search for messages with player's serial; Sys/system - search for messages in the system chat. Can be combined with: 'my|sys'.

- `serial` - search for messages from the object with the specified serial. 0 ignores the filter by serial.

- `color` - search for messages with the specified color. 0xFFFF ignores the filter by color.

- `startTime` - initial time of search. 0 the initial time is ignored.

- `endTime` - the end time of the search. 0 the end time is ignored

Result: object of the type JournalMessage or null if nothing was found.
</br></br>
***
</br>
_JournalMessage_ **Orion.WaitJournal**('pattern', startTime, endTime, [flags], ['serial'=0], ['color'=0xFFFF]);

Waiting for the appearance of data in the journal.

- `pattern` - required string, which can consist of several lines separated via |

- `startTime` - initial time of search. 0 the initial time is ignored.

- `endTime` - the end time of the search. 0 the end time is ignored

- `flags` - search flags in the journal: my/self - search for messages with player's serial; Sys/system - search for messages in the system chat. Can be combined with: 'my|sys'.

- `serial` - search for messages from the object with the specified serial. 0 ignores the filter by serial.

- `color` - search for messages with the specified color. 0xFFFF ignores the filter by color.

Result: object of the type JournalMessage or null if nothing was found.
</br></br>
***
</br>
_JournalMessage_ **Orion.LastJournalMessage**();

Retrieve last message from Orion Assistant journal.

Result: object of the type JournalMessage or null if nothing was found.
</br></br>
***
</br>
_int_ **Orion.JournalCount**();

Returns: Amount of messages in journal.
</br></br>
***
</br>
_JournalMessage_ **Orion.JournalLine**(index);

Returns JournalMessage by index or null of index wasn't found.
