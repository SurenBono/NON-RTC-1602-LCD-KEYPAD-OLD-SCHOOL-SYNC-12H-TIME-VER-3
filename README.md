# NON-RTC-1602-LCD-KEYPAD-OLD-SCHOOL-SYNC-12H-TIME-VER-3.1 also Non-NTP Non-RCC Nor GPS :)
-------------------------------------------------------------------------------------------------------

A simple, affordable bright timekeeping demo that reserves the mid-night oil 
within minute accuracy / day if compared to ancient hour glass + a candle .

MODULE
---------------------------------------------------------------------------------------------------------
- SMD UNO or similar (Nano,Mega..etc ) are open sourced to test.
- 4-bit 1602 LCD Uno Stackable Keypad.
- USB serial power & data cable.
- Pc with preferred online connection .

NOTE
----------------------------------------------------------------------------------------------------------
- Oscillators provide the basic timing and control for a microcontroller 
  and its peripherals. Commonly used oscillators are of crystal because of
  its well known stability and durability. It produces stable output for 
  prolonged time. Crystal oscillators are mainly works under the principle 
  of Piezo electric effect.
- 16 MHz Crystal Oscillator marks a SECOND on UNO or something similar.
- Crystal Osciilators Accuracy : + 1 min /day if compared to NTP time.
- Reset Second ( btnDOWN ) to re-sync.
- Incorporated binary,hex & decimal (byte) into timekeep project.
- Used https://maxpromer.github.io/LCD-Character-Creator/
- Developed on Win Xp ,donated version of ARDUINO 1.8.9 2019.03.15

BUG FIXED on V3.1
-------------------------------------------------------------------------------------------------------------
- Bigger digit from former 1 COL x 2 ROW / digit to 3 COL x 2 ROW / digit.
- Shifted AM/PM to start from 12:00 
- Added 2 button ,1-btnDOWN=RESET SECOND , 2-btnUP=AM/PM toggle.
- HR2 will remain blank until hour 10,11,12(HR2,HR).
- Assigned HR2 = 10 as if 0 to point to blank byte (254)/(" ") which was int NUM =0 in former versions.
- Assigned HR2 = 11 as if int NUM = 1 to point to a cloned bytes of BIG DIGIT one.

PRE-COMPILING TASK
--------------------------------------------------------------------------------------------------------------
- I assume you have the open sourced Arduino.cc IDE installed. Donation encouraged.
- Google search Install CH341SER driver for SMD UNO or similar.
- Select check proper port & board.
- Add LCDKeypad & TimerOne drivers into Arduino\libraries.
- Check if it compiled else learn to debug it.
- If compiled than Upload and keypad sync test to your local time..etc

CONTACT 
---------------------------------------------------------------------------------------------------------------
- surenbono76@gmail.com
- srotogargees@gmail.com
- https://srotogargees.business.site/

Original code by Jesse Tane for http://labs.ideo.com August 2008
Developed by 2019 Sroto&Gargees™




