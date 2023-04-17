Hak5's Rubber Ducky is a keystroke injection tool disguised as a USB flash drive. It allows users to run pre-written scripts on a target computer as if a human were typing on the keyboard. Recreating a Rubber Ducky can be done using an inexpensive USB development board, such as the Digispark ATTiny85.

Please note that using a Rubber Ducky or similar device for unauthorized access or malicious activities is illegal and unethical. The following information is for educational purposes and should only be used with permission and for legitimate reasons, such as penetration testing or automating repetitive tasks.

Here's how to recreate a Rubber Ducky using a Digispark ATTiny85:

Materials needed:

Digispark ATTiny85 USB Development Board (can be purchased from sites like eBay or AliExpress)
A computer running Windows, macOS, or Linux
Steps:

Install Arduino IDE: Download and install the Arduino IDE from the official website (https://www.arduino.cc/en/software).

Configure the Arduino IDE for Digispark:
a. Open the Arduino IDE and go to File > Preferences.
b. In the "Additional Boards Manager URLs" field, add the following URL: http://digistump.com/package_digistump_index.json
c. Click "OK" to save and close the Preferences window.
d. Go to Tools > Board > Boards Manager.
e. Search for "Digistump AVR Boards" and click "Install".
f. Once installed, close the Boards Manager.

Select the Digispark board:
a. Go to Tools > Board and select "Digispark (Default - 16.5MHz)".
b. Ensure that the proper programmer is selected under Tools > Programmer > "Micronucleus".

Install the DigiKeyboard library:
a. Go to Sketch > Include Library > Manage Libraries.
b. Search for "DigiKeyboard" and install the "DigiKeyboard" library by Digistump.

Create the payload script:
a. Open a new sketch in the Arduino IDE.
b. Write or paste your payload script using the DigiKeyboard library to simulate keystrokes. You can find examples online or on the Digistump GitHub repository (https://github.com/digistump/DigistumpArduino/tree/master/digistump-avr/libraries/DigisparkKeyboard).

Upload the payload script to the Digispark ATTiny85:
a. Connect the Digispark ATTiny85 to your computer's USB port.
b. Click the "Upload" button in the Arduino IDE.
c. When prompted, unplug the Digispark and plug it back in. The payload script will be uploaded to the device.

Now you have a Rubber Ducky-like device using a Digispark ATTiny85. When plugged into a target computer, the device will execute the payload script as if a human were typing on the keyboard.

Remember to use this device responsibly and only for legitimate purposes.
