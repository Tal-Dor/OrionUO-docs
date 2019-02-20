# Text Window

**TextWindow is a static reference just like Orion so you can always get it.**
</br></br>
***
### Command Format

**NameSpace**.**name**(_**requiredParameters**_, [_optionalParameters=defaultValue_]);
</br></br>
***
</br>
_void_ **TextWindow.Open**();

Open the text box.
</br></br>
***
</br>
_void_ **TextWindow.Close**();

Close the text box.
</br></br>
***
</br>
_void_ **TextWindow.Clear**();

Clear the text box.
</br></br>
***
</br>
_void_ **TextWindow.Print**('text');

Type the text in the text box.
</br></br>
***
</br>
_void_ **TextWindow.SetPos**(x, y);

Move text windows to x and y screen coordinates.
</br></br>
***
</br>
_void_ **TextWindow.SetSize**(width, height);

Sets text windows size by given width and height.
</br></br>
***
</br>
_void_ **TextWindow.SaveToFile**('filePath');

Write contents of text windows into a file at filePath.
