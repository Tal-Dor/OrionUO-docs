# Lists -> Ignore

![lists_ignore](http://www.imageup.ru/img290/2713066/tab_lists_ignore.png)

Ignore lists that can be applied in scripts.

1) List of created ignore lists.

2) List of items in the ignore list.

3) Name - name of the ignore list.

4) Add list - to add a new list.

5) Edit selected list - to save changes to the selected list.

6) Remove list

7) Graphic - Graphic of the object in the format 0x0000.

8) Color - Color of the object in the format 0x0000.

9) Comment - a comment to the object (optional).

10) Add item - to add a new item to the selected list.

11) Edit selected item - to save changes to the selected item in the selected list.

12) Remove item - to remove the item from the selected list.

13) Item from target - to specify the object by using a target in the client from which you want to read the information.

***

"Graphic" and "Color" can be specified in the form of enumerations with delimiters | ;

Additionally, you can specify some filters for them:

- "!value" - not equal to the value
- "<value" - less than the value
- ">value" - more than the value

For instance:

Graphic: 0x0023
Color: >0x0010|!0x0021|!0x0032

Will ignore objects with the type 0x0023 of all colors starting from 0x0011 excluding 0x0021 and 0x0032.


Graphic: 0x042F
Color: !0

Will ignore objects with the type 0x042F only if they have a color.