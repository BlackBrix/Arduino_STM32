this repo is forked from [rogerclarkmelbourne/Arduino_STM32](https://github.com/rogerclarkmelbourne/Arduino_STM32)  
  
----  

the following readme.md is the original one from the original repo mentioned above  
  
I forked this repo to add a new board/variant (for experimantal/test-purposes) with:
* STM32F103VET6 (512kB Flash / 64kB RAM / 100pin)
* no "Maple USB reset hardware"
* no buttons 
* 2 LEDs on PC8 and PC9 
* 16MHz ext. crystal

In the code this board is called "BLACKBRIX_PLC" because this board is actually the mainboard of a mini-PLC (DIN rail / "smart-relay")  
  
  
**Installation:**  
* Download and install version 1.8.x of the Arduino IDE from [here](https://www.arduino.cc/en/Main/Software).
* Run the IDE, and on the Tools menu, select the Boards manager, and install the "Arduino SAMD Boards" from the list of available boards. This installs compiler support for ARM Cortex.
* Download a zip file containing the Arduino STM32 files from [here](https://github.com/BlackBrix/Arduino_STM32/archive/master.zip).
* for a normal Arduino-Installation:  
  * Unzip the content of the zip file, and place the 'Arduino_STM32' folder to [Arduino sketches folder]/[hardware]/[Arduino_STM32].  
  (e.g. on Windows the default [Arduino sketches folder] is like "C:\Users\USERNAME\Documents\Arduino\...")
  * Create the 'hardware' folder there if it does not exist yet.
* for a portable Arduino-Intallation:  
  * Unzip the content of the zip file, and place the 'Arduino_STM32' folder dirctly into the 'hardware' folder that is located in the arduino main-directory. (the main-directory is where the 'arduino.exe' is located)  
So we get [Arduino main directory]/[hardware]/[Arduino_STM32] in this case.
  * Create the 'hardware' folder there if it does not exist yet.
  
  
the complete WIKI of the original repo -> https://github.com/rogerclarkmelbourne/Arduino_STM32/wiki  
another wiki: http://wiki.stm32duino.com  
forum:  http://www.stm32duino.com
  
  
---- 




Arduino STM32  
=============  

## Notice

This software is experimental and a work in progress.
Under no circumstances should these files be used in relation to any critical system(s).
Use of these files is at your own risk.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

## Summary:  
This repo contains, the "Hardware" files to support STM32 based boards on Arduino version 1.8.x (some older versions may also work)  including [LeafLabs Maple, and Maple mini](http://www.leaflabs.com/about-maple/), and other generic STM32F103 boards  

***PRIMARY SUPPORT FORUM: http://www.stm32duino.com/***

***We are also on Gitter https://gitter.im/stm32duino/Lobby/***
[![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/stm32duino/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

## Background & Support:  
* Based on https://github.com/bobc/maple-asp, which is in turn based on LibMaple by Leaflabs  
* **Please read the wiki (https://github.com/rogerclarkmelbourne/Arduino_STM32/wiki) for full details**
* See also my blog: http://www.rogerclark.net/stm32f103-and-maple-maple-mini-with-arduino-1-5-x-ide/  
* **NEW: Main support site for using STM32 boards with the Arduino IDE: http://www.stm32duino.com/**  
* Original LeafLabs "Docs:" http://docs.leaflabs.com/docs.leaflabs.com/index.html


**YouTube Videos:** 
* 20141116: [Arduino 1.5.8 IDE with STM32 board](https://www.youtube.com/watch?v=-zwGnytGT8M)
* 20150413: [STM32 for Arduino 1.6.2 or newer (update)](https://www.youtube.com/watch?v=TePglhSkghg)
* 20150419: [Uploading via USB to Serial to STM32F103 boards](https://www.youtube.com/watch?v=G_RF0a0hrak)

## Additional Links & Info:  
* https://www.hackster.io/rayburne/4-dollar-90-mips-32-bit-72-mhz-arm-arduino  

## Purchase info:  
### Entry level boards

* [Ebay search for "arduino maple"](http://www.ebay.com/sch/i.html?_from=R40&_sacat=0&LH_BIN=1&_nkw=arduino+maple&_sop=15) (currently costs <$5 with shipping)
* [AliExpress search for "leaflabs maple"] (http://www.aliexpress.com/wholesale?catId=0&initiative_id=SB_20150607085526&SearchText=leaflabs+maple)

### Bigger boards (You need to load the stm32duino bootloader)

Some supplier have this board e.g.

*[ STM32F103VET ](http://www.ebay.com.au/itm/1PCS-STM32F103VET6-ARM-STM32-Minimum-System-Development-Board-Arduino-M77-/301433302819)

*[There is also a STM32F103ZET board which also works, however they are not always available. They have been listed as "STM32F103ZET6 Minimum System Development Board ARM STM32 Cortex-m3 M75"]
(http://www.ebay.com.au/itm/1pcs-STM32F103ZET6-Minimum-System-Development-Board-ARM-STM32-Cortex-m3-M75-/291305557264)

