# ESP32Radio-V2, PCB v3.x
## Printed Circuit Board for the [ESP32Radio-V2 from Ed Smallenburg](https://github.com/Edzelf/ESP32Radio-V2)

Updates:
- 2022-11-06, PCB v3.1 Rev C

 ** **
 
As microcontroller this PCB uses the MH ET LIVE ESP32MiniKit.<br> 
The PCB is designed to allow the use of one mini amplifier module (PAM8403) and/or a bluetooth transmitter module (kcx_bt_emitter).<br>
There are connectors for the supported display types (TFT, LCD, Nextion not tested), the rotary encoder, the IR receiver plus a expansion port with pins connected to GPIO12, GPI013, GPIO14 and GPIO34. MISO, MOSI, SLCK pins are also available on the expansion port.<br>
Circuit to turn ON/OFF the TFT backlight is also implemented. Control is done by the ESP32Radio software.<br>
Power supply is 5V DC.<br>
<br>

![ESP32_WebRadio_PCB_v3 2_01](https://user-images.githubusercontent.com/14356332/200154388-d73d5ee6-fb64-46e0-a4de-ef9e7894c342.jpg)

![ESP32_WebRadio_PCB_v3 2_02](https://user-images.githubusercontent.com/14356332/200154434-14eb3337-b357-42a4-9562-9909f6c829ba.jpg)
 <br>
 ** **

**Example of one unit using the PAM8403 amplifier.** <br><br>
The black wire on the picture isn't a patch, it connects the Analog GND (GBUF) from the VS1053 through a 47uF capacitor to VREF (pin 8) of the PAM8403 chip. This effectively cancels any noise on the speakers.<br>
Many hobbyists are hiding the huge problem of connecting an amplifier directly to the output of the VS1053B module. Everyone plugs in the headphones or amplifiers with a separate power supply and is happy with it. The problem is that as soon as you connect an amplifier with common ground to the VS1053 module, you hear very strong digital noise, which even drowns out the useful signal.<br>

![ESP32_WebRadio_PCB_v3 2_03](https://user-images.githubusercontent.com/14356332/200154441-9933c375-fe29-425d-9619-b77ff17f3648.jpg)
 <br>
 ** **

**Example of a second unit using the kcx_bt_emitter bluetooth module.** <br>

![IMG_20221113_050903_479](https://user-images.githubusercontent.com/14356332/201507650-d6aeef9c-f1ef-495b-8586-b36859739626.jpg)
<br>

