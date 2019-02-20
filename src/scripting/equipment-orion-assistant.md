# Equipment

A group of commands to work with clothes and dress/undress.
#### Table of equipment layers:

  |   |   |   |   |  |
--|---|---|---|---|--|
 1 - RightHand |  7 - Gloves | 13 - InnerTorso  | 19 - Arms  | 25 - Mount  |  
 2 - LeftHand |  8 - Ring | 14 - Bracelet  | 20 - Cloak  | 26 - Buy  |  
 3 - Shoes | 9 - Talisman  | 15 - Face  | 21 - Backpack  | 27 - Resale  |  
 4 - Pants | 10 - Necklace  | 16 - Beard  | 22 - Robe  | 28 - Sell  |  
 5 - Shirt | 11 - Hair  | 17 - MidTorso  | 23 - Eggs  |  29 - Bank |  
 6 - Helmet |  12 - Waist | 18 - Earrings  | 24 - Legs  |   |  



### Command Format

**NameSpace**.**name**(_**requiredParameters**_, [_optionalParameters=defaultValue_]);
</br></br>
***
</br>
_void_ **Orion.SetDressBag**(['serial'=targetRequest]);

Change the serial of bag for clothes on "serial".

Request target to be aimed at the desired object, if parameters were not specified.
</br></br>
***
</br>
_void_ **Orion.UnsetDressBag**();

Reset the serial of bag.
</br></br>
***
</br>
_void_ **Orion.SetArm**('setName');

Set the weapon/shield.
</br></br>
***
</br>
_void_ **Orion.UnsetArm**('setName');

Clear setName.
</br></br>
***
</br>
_void_ **Orion.SetDress**('setName');

Set the clothes in the 'setName' (except weapons and shields).
</br></br>
***
</br>
_void_ **Orion.UnsetDress**('setName');

Clear setName.
</br></br>
***
</br>
_void_ **Orion.Arm**('setName');

Dress setName.

Before dressing, if the option of safe dressing is turned on, removes all clothes in layers 1/2 (left and right hand) and then the rest.
</br></br>
***
</br>
_void_ **Orion.Disarm**();

Disarm your weapon/shield.
</br></br>
***
</br>
_void_ **Orion.Dress**('setName');

Dress setName.

Before dressing, if the option of safe dressing is turned on, removes all clothes in layers 1/2 (left and right hand) and then the rest.
</br></br>
***
</br>
_void_ **Orion.Undress**();

Take off all but the weapons and shields.
</br></br>
***
</br>
_void_ **Orion.Unequip**('layerName');

Remove the object from the specified layer.
</br></br>
***
</br>
_void_ **Orion.Equip**('serial');

Dress the specified item.
</br></br>
***
</br>
_void_ **Orion.EquipT**('graphic', ['color'=0xFFFF]);

Find the item in the character backpack/sub-packs and bags with the type "graphic" and "color" (if required) and dress them.
