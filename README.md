# iBusFlySkyIA6B
Sample code for FS-IA6B (and possibly other receivers) for the Arduino Uno (and possibly other boards)
Using Bart Mellink's IBusBM library version 1.1.1
https://github.com/bmellink/IBusBM
Grab the IbusBM library from >Tools>Manage Libraries

Test Code for a FlySky FS-i6X transmitter and FS-iA6B receiver (10 channel).  This implementation only reads values from the receiver and does not transmit battery levels, etc. back to the handheld transmitter.

// Tested with Uno R3 and R3+ and is much less complex (one wire for all channels) and error prone than orginal PWM setup

// Use port 0 for serial communication on Uno R3, other boards have multiple serial ports.  Connect to uppermost/rightmost iBus pin on FS-iA6B receiver

// Note that because you're sharing a serial port with USB on the Uno, you may have to disconnect the cable from pin 0 and restart the Arduino IDE (and board) to get the upload working.

// Also note that in code channels start at zero but on the receiver they start at one, hence offset.
