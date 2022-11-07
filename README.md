# ESP32Radio-V2, PCB v3.x
## Printed Circuit Board for the [ESP32Radio-V2 from Ed Smallenburg](https://github.com/Edzelf/ESP32Radio-V2)

Updates:
- 2022-11-06, PCB v3.1 Rev C

 ** **
 
As microcontroller this PCB uses the MH ET LIVE ESP32MiniKit.<br> 
The PCB is designed to allow the use of one mini amplifier module (PAM8403) and/or a bluetooth transmitter module (kcx_bt_emitter).<br>
There are connectors for the supported display types (TFT, LCD), the rotary encoder, the IR receiver and a expansion port with pins connected to GPIO12, GPI013, GPIO14 and GPIO34. MISO, MOSI, SLCK pins are also available on the expansion port.<br>
When using the PAM8403 amplifier, to avoid common noise problems, the Analog GND from the VS1053 must be connected to pin 8 of the PAM8403 chip. This solution proved to be very effective.<br>
Power supply is 5V DC.<br>
<br>
<br>
![ESP32_WebRadio_PCB_v3 2_01](https://user-images.githubusercontent.com/14356332/200154388-d73d5ee6-fb64-46e0-a4de-ef9e7894c342.jpg)
<br>
![ESP32_WebRadio_PCB_v3 2_02](https://user-images.githubusercontent.com/14356332/200154434-14eb3337-b357-42a4-9562-9909f6c829ba.jpg)
 <br>
 ** **
 <br>
**Example of one unit using the PAM8403 amplifier.**<br>
The black wire connects the Analog GND (marked as NC on the PCB) from the VS1053 to pin 8 of the PAM8403 chip.<br>
![ESP32_WebRadio_PCB_v3 2_03](https://user-images.githubusercontent.com/14356332/200154441-9933c375-fe29-425d-9619-b77ff17f3648.jpg)
 <br>
 ** **
 <br>
**Example of a second unit using the kcx_bt_emitter bluetooth module.**<br>
<br>
![IMG_20221106_040153_472](https://user-images.githubusercontent.com/14356332/200154453-ab6679a0-d180-4eff-9ae0-a9640cdbe652.jpg)
<br>
