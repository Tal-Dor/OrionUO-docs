# Interactions With Files

### Command Format

**NameSpace**.**name**(_**requiredParameters**_, [_optionalParameters=defaultValue_]);

***

- FileObject Orion.NewFile();

Create a file object.

***

- bool fileObject.Open('filePath');

An attempt to open a file (or create a new one) by the filePath.

Result: true if the file is successfully opened.

***

- bool fileObject.Append('filePath');

An attempt to open the file by the filePath to the write-in (the pointer to the data is placed at the end of the file).

Result: true if the file is successfully opened.

***

- bool fileObject.Opened();

Verify the validity of the opened file.

Result: true if the file is open.

***

- void fileObject.Close();

Close the file.

***

- String fileObject.ReadLine();

Read the line before the line break (\ n).

Result: The result of reading the data.

***

- String fileObject.Read();

Read the word (up to blank-space " ").

Result: The result of reading the data.

***

- void fileObject.WriteLine('data');

Record the data string and move the string (\ n).

***

- void fileObject.Write('data');

Write down the data.

***

## Introduced in 2.0.16.0

- void fileObject.Remove(['filePath']);

Deletes file at filePath.

If filePath was an empty string or null reference, it'll close and try delete fileObject.
