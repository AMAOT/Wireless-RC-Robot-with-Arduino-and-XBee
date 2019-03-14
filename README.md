Wireless RC Robot with Arduino and XBee
========================================

<table class="table table-hover table-striped table-bordered">
  <tr align="center">
   <td><a href="https://learn.sparkfun.com/tutorials/wireless-joystick-hookup-guide/"><img src="https://cdn.sparkfun.com/assets/learn_tutorials/5/7/0/Joystick_Tutorial-01.jpg" alt="Wireless Joystick with SAMD21"></a></td>
   <td><a href="https://learn.sparkfun.com/tutorials/experiment-guide-for-redbot-with-shadow-chassis"><img src="https://cdn.sparkfun.com/assets/learn_tutorials/3/5/6/Redbot_Kit-93.jpg" alt=""></a></td>
  </tr>
  <tr align="center">
    <td><i>Wireless Remote</i></td>
    <td><i>Assembled RedBot</i></td>
  </tr>
</table>

Example code using the wireless remote controller (SAMD21) to control the SparkFun RedBot (ATmega328P) via XBee. A character is pipelined between two serial UARTs using a pair of XBee Series 1 Transcievers. Make sure to use software serial example code for the RedBot to avoid bricking your XBee. This expands on SparkFun Inventor's Kit for RedBot.

Repository Contents
-------------------

* **/Firmware** - Example code 

Documentation
--------------
* **[Library](https://github.com/sparkfun/SparkFun_RedBot_Arduino_Library)** - Arduino library for the RedBot mainboard.
* **[Project Guide](https://learn.sparkfun.com/tutorials/wireless-rc-robot-with-arduino-and-xbees)** - Project guide.

XBee w/ Series 1 Firmware:  Point to Point Configuration
-------------------
[Digi Tutorial: XBee 802.15.4 (i.e. Wireless Serial)](https://www.digi.com/blog/basic-xbee-802-15-4-chat/)
  
* Master XBee (Transmitting, Controller)
  * CH = C
  * ID = 3333
  * DH = 0
  * DL = 1
  * MY = 0

* Slave XBee (Receiving, RedBot)
  * CH = C
  * ID = 3333
  * DH = 0
  * DL = 0 <- point to Master "MY"
  * MY = 1 <- Slave "MY", make it unique in the network.

Products that use this Library 
---------------------------------

* [ROB-13166](https://www.sparkfun.com/products/13166) - Basic RedBot Kit
* [ROB-12649](https://www.sparkfun.com/products/12649) - RedBot Experiment Kit
* [KIT-14051](https://www.sparkfun.com/products/14051) - Wireless Joystick Kit
* [WRL-15126](https://www.sparkfun.com/products/15126) - XBee Series 3 Configured for Series 1 Firmware

License Information
-------------------

This product is _**open source**_! 

Please review the LICENSE.md file for license information. 

If you have any questions or concerns on licensing, please contact technical support on our [SparkFun forums](https://forum.sparkfun.com/viewforum.php?f=152).

Distributed as-is; no warranty is given.

- Your friends at SparkFun.

_<COLLABORATION CREDIT>_
