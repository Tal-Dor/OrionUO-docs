# Equipment

A group of commands to work with clothes and dress/undress.

List of layers:

1 - RightHand

2 - LeftHand

3 - Shoes

4 - Pants

5 - Shirt

6 - Helmet

7 - Gloves

8 - Ring

9 - Talisman

10 - Necklace

11 - Hair

12 - Waist

13 - InnerTorso

14 - Bracelet

15 - Face

16 - Beard

17 - MidTorso

18 - Earrings

19 - Arms

20 - Cloak

21 - Backpack

22 - Robe

23 - Eggs

24 - Legs

25 - Mount

26 - Buy

27 - Resale

28 - Sell

29 - Bank


### Command Format

**NameSpace**.**name**(_**requiredParameters**_, [_optionalParameters=defaultValue_]);

***

- void Orion.SetDressBag(['serial'=targetRequest]);

Change the serial of bag for clothes on "serial".

Request target to be aimed at the desired object, if parameters were not specified.

***

- void Orion.UnsetDressBag();

Reset the serial of bag.

***

- void Orion.SetArm ('setName');

Set the weapon/shield.

***

- void Orion.UnsetArm ('setName');

Clear setName.

***

- void Orion.SetDress ('setName');

Set the clothes in the 'setName' (except weapons and shields).

***

- void Orion.UnsetDress ('setName');

Clear setName.

***

- void Orion.Arm('setName');

Dress setName.

Before dressing, if the option of safe dressing is turned on, removes all clothes in layers 1/2 (left and right hand) and then the rest.

***

- void Orion.Disarm();

Disarm your weapon/shield.

***

- void Orion.Dress('setName');

Dress setName.

Before dressing, if the option of safe dressing is turned on, removes all clothes in layers 1/2 (left and right hand) and then the rest.

***

- void Orion.Undress();

Take off all but the weapons and shields.

***

- void Orion.Unequip ('layerName');

Remove the object from the specified layer.

***

- void Orion.Equip ('serial');

Dress the specified item.

***

- void Orion.EquipT('graphic', ['color'=0xFFFF]);

Find the item in the character backpack/sub-packs and bags with the type "graphic" and "color" (if required) and dress them.