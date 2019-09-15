# NON-RTC-1602-LCD-KEYPAD-OLD-SCHOOL-SYNC-12H-TIME-VER-3.1
...also non GPS ... and non NTP

BUG FIXED V2
-------------
- Shifted AM/PM to start from 12:00 
- Added 2 button ,1-btnDOWN=RESET SECOND , 2-btnUP=AM/PM toggle
- HR2 will remain blank until hour 10,11,12(HR2,HR)
- Assigned HR2 = 10 as if 0 to point to blank byte (254)/(" ") which was int NUM =0 in former versions.
- Assigned HR2 = 11 as if int NUM = 1 to point to a cloned bytes of BIG DIGIT one


create TimerOne folder ...  document/Arduino/libraries/TimerOne
....copy TimerOne.cpp & TimerOne.h into & experience it..
....are you experienced...

Original code by Jesse Tane for http://labs.ideo.com August 2008
Developed by 2019 Sroto&Gargees™
