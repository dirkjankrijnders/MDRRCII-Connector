MDRRCII-Connector
=================

This is a small interface board to connect the [Mini STM32 board](http://www.ebay.com/itm/MINI-V3-STM32F103RBT6-development-board-with-2-8-TFT-module-/121287420704?pt=Art_Prints&hash=item1c3d4b2b20) as used in [MDRRC II](http://members.home.nl/robert.evers/mdrrc2.htm) its peripherals. It is effectively all of the schematics in the manual on a nice board. It uses a DIN5 connector for I2C controller and also has a [S88N](http://www.s88-n.eu) pin-compatible RJ45 connection. Its power it receives from a 4-pin molex connector as commonly found in computers. By default this also powers the STM32, which is not desirable unless an USB isolator is used. 

It also includes a USB isolator, not necessary for normal operation, but when fiddling around I'd rather blow the 10 euro isolator than my laptops usb port. It also 

Unchecked Reichelt shopping card:
http://www.reichelt.de/?ACTION=20;AWKID=901501;PROVID=2084

STATUS
------
Board for Rev.0 are on order and recieved. The first board is build and very lightly tested with MDRRC version one, due to a rather lengthy remodeling of my train room (well actually, the creation of...). Below is a photo of the prototype. Testing with MDRRC-II is under way though.

![Photo of the first prototype](Output/Rev.0/IMG_1077.png)

<table>
<tr>
<th>Function</th><th>test</th>
</tr>
<tr><td>Power</td><td>Passed</td></tr>
<tr><td>Booster connection</td><td>Passed</td></tr>
<tr><td>S88N</td><td>Passed*</td></tr>
<tr><td>I2C</td><td>Failed, see issue #1</td></tr>
<tr><td>Programming</td><td>Untested</td></tr>
<tr><td>Expressnet</td><td>Untested</td></tr>
</table>
* Works, but S88N signal specifications remain untested until now.

LICENSE
-------

Both hardware and firmware are placed under the Creative Commons Attribution-ShareAlike 3.0 Unported License. See <http://creativecommons.org/licenses/by-sa/3.0/> and License.txt for more details.

Copyright 2014
Dirkjan Krijnders
<dirkjan@krijnders.net>
