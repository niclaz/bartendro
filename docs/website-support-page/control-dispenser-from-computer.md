## Control a Dispenser from a Computer 

This is a guide on how to quickly control a Bartendro Dispenser from a computer. Mac, PC, Linux, it doesn't matter. As long as you have a USB port and a serial terminal application, you're good to go.

### Step 1 — Gather or Acquire the Parts Needed 

These are the items you'll need:
- FTDI Board https://www.sparkfun.com/products/9716
- RJ-45 Breakout https://www.sparkfun.com/products/716
- RJ-45 Connector https://www.sparkfun.com/products/643
- Some wire and a soldering iron.

### Step 2 — Solder Wires to the RJ-45 Breakout

- Solder wire to the appropriate pins.
- On the Sparkfun board, white-orange, which is normally pin 1 is mapped to pin 8 on the board, so be careful.
- You will need a minimum of 5 wires to run a pump. 24V, 5V, TX, RX, and ground.
- Note: On the Sparkfun board, white-orange, which is normally pin 1 is mapped to pin 8 on the board, so be careful.

### Step 3 — Connect to the FTDI Board

- Insert the wires into the FTDI board. Make sure that TX from the Dispenser goes to RX of the FTDI and vise versa.
- Connect 24V to the motor voltage pin, and make sure the ground is connected from your 24V source.

### Step 4 — Connect Using a Serial Terminal
- Connect using your serial terminal program. Like Terminal.app or Putty.exe
- Connect to the appropriate COM or /dev/tty.usbserial using a BAUD rate of 9600
- Type !!! and if everything is hooked up correctly, you should see a message that says "Party Robotics Dispenser at your service!"
- You can type help to see all the things you can do.
- This system is sensitive to typos, and you cannot backspace, so if you mess up a command, you will have to do it over.
- If you do not have a voltage of 12V or higher on the Motor Voltage pin, you will not be able to run the motor, so make sure that is connected up too

###  Comment: jerry Isdale - 09/23/2016 

"apparently the only documentation is in the code on GitHub. The dispensers we had did not seem to respond to the "?" binary protocol, but did work with the "!!!" text mode.... although there were all sorts of odd behaviors depending on when power and reset were applied to the dispenser and Teensy. Sometimes Dispenser would not respond, sometimes it would come up RED, sometimes it worked right. We were running with Teensy plugged into USB port of a Mac powerbook with +12v battery feeding the dispenser and thru a 12->5v supply to the teensy, etc. W/o battery teensy worked fine, but of course dispenser wouldnt. Adding the battery we sometimes needed to unplug Dispenser, reset teensy, then plug in dispenser. after that it worked - and could often restart completely."

[Source: http://support.partyrobotics.com/Guide/Control+a+Dispenser+from+a+Computer/14]
