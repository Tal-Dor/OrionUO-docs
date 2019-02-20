# Interactions With Files

### Command Format

**NameSpace**.**name**(_**requiredParameters**_, [_optionalParameters=defaultValue_]);
</br></br>
***
</br>
_FileObject_ **Orion.NewFile**();

Create a file object.
</br></br>
***
</br>
_bool_ **fileObject.Open**('filePath');

An attempt to open a file (or create a new one) by the filePath.

Result: true if the file is successfully opened.
</br></br>
***
</br>
_bool_ **fileObject.Append**('filePath');

An attempt to open the file by the filePath to the write-in (the pointer to the data is placed at the end of the file).

Result: true if the file is successfully opened.
</br></br>
***
</br>
_bool_ **fileObject.Opened**();

Verify the validity of the opened file.

Result: true if the file is open.
</br></br>
***
</br>
_void_ **fileObject.Close**();

Close the file.
</br></br>
***
</br>
_String_ **fileObject.ReadLine**();

Read the line before the line break (\ n).

Result: The result of reading the data.
</br></br>
***
</br>
_String_ **fileObject.Read**();

Read the word (up to blank-space " ").

Result: The result of reading the data.
</br></br>
***
</br>
_void_ **fileObject.WriteLine**('data');

Record the data string and move the string (\ n).
</br></br>
***
</br>
_void_ **fileObject.Write**('data');

Write down the data.
</br></br>
***
</br>
_void_ **fileObject.Remove**(['filePath']);

Deletes file at filePath.

If filePath was an empty string or null reference, it'll close and try delete fileObject.
