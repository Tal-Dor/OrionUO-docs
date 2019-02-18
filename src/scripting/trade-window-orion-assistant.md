# Trade Window

### Command Format

**NameSpace**.**name**(_**requiredParameters**_, [_optionalParameters=defaultValue_]);

***

- int Orion.TradeCount();

Result: the amount of open menus.

***

- String Orion.TradeContainer('index', 'container');

Get the container serial of the trade window with the index 'index' (from 0 to TradeCount () - 1) (or using the serial index 0x12345678).

container - Window identifier, right ('right' or '1') or left ('left' or '0').

Result: serial of the container.

***

- String Orion.TradeOpponent('index');

Get an opponent's serial of the trade window with the index 'index' (from 0 to TradeCount () - 1) (or using the serial index 0x12345678).

Result: opponent's serial.

***

- String Orion.TradeName('index');

Get the opponent's name of the trade window with the index 'index' (from 0 to TradeCount () - 1) (or using the serial index 0x12345678).

Result: opponent's name.

***

- bool Orion.TradeCheckState('index', 'container');

Obtain the status (confirmation) of the transaction in the trade window with the index 'index' (from 0 to TradeCount () - 1) (or using serial number index 0x12345678).

container - Window identifier, right ('right' or '1') or left ('left' or '0').

Result: the status of the checkbox is true / false.

***

- void Orion.TradeCheck('index', state);

Change the transaction confirmation status in the trade window with the index 'index' (from 0 to TradeCount () - 1) (or using serial number index 0x12345678).

state - new state, true (tick) or false (uncheck).

***

- void Orion.TradeClose('index');

Close the trade window with the index 'index' (from 0 to TradeCount () - 1) (or using the serial index 0x12345678).

***

## Introduced in 2.0.15.0

- bool Orion.WaitForTrade([delay=1000]);

Await for a trade window for a given 'delay' amount of time and blocking script execution.

Returns true if a trade window was received during this period.
