"# WBL-1" 

<b>What is WillowBee?</b>
 <p align="justify">WillowBee is an industrial wireless microcontroller module that is designed for LoRaWAN sensor end-node designs and embedded applications that need LoRaWAN communications. WillowBee uses the popular STM32WL Cortex-M4 microcontroller from ST Micro. This microcontroller combines a computer unit and a LoRaWAN radio on a single chip. </p> 

![image](https://github.com/WillowBeeLoRaWAN/WBL-1/assets/145584015/deb546bc-1ae0-4c34-b490-ac038ee0fad4)

<b>Install WillowBee Development Environment</b>

1. Open Windows Terminal
2. Create directory "md C:\bipom\devtools\WillowBee"
3. Get in the directory "cd C:\bipom\devtools\WillowBee"
4. Clone the repository "git clone https://github.com/WillowBeeLoRaWAN/WBL-1.git"

<b>Building LED example in Keil</b>

1. Open led_blink example "WillowBee\WBL1\examples\led_blink\MDK-ARM\led_blink.uvprojx"
2. Compile the example then, check the warning and error

<img src="https://willowsoft.co/wp-content/uploads/keil_build.png" width=60% height=60%>

<b>Flashing binary via USB</b>
1. Open the settings  Flash->Configure Flash Tools...
<img src="https://willowsoft.co/wp-content/uploads/keil-usb.png" width=60% height=60%>
2. Set the correct COM port in the menu that "Use an external tool for flash programming", then click "OK"
<code>C:\bipom\devtools\WillowBee\WBL1\loader\uCLoader\ucloader.exe  /p=<b>com9</b> 
 /f=C:\bipom\devtools\WillowBee\WBL1\examples\led_blink\MDK-ARM\led_blink\led_blink.hex /dll=stm32isp.dll</code><br>
3. Set SW1 position to program mode (PGM) as follows
<img src="https://willowsoft.co/wp-content/uploads/keil_pgm-1.jpg" width=20% height=20%>
4. Click on Load button as follows then, check the build output for success message
<img src="https://willowsoft.co/wp-content/uploads/keil_flash-1.jpg" width=60% height=60%>
5. Red and Green LED blinks as follows  
<img src="https://willowsoft.co/wp-content/uploads/led_blink.jpg" width=20% height=20%>
