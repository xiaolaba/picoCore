# this is fork of https://github.com/nerdralph/picoCore
trying to json of github and easy installation.
testing, 2020-05-19

open Arduino IDE, File / Preference / Additional Broad manage, include the json following,  

https://xiaolaba.github.io/picoCore/package_xiaolaba_picoCore_index.json  


-----------------------------------------




# picoCore
Small Arduino/Wiring core for 8-pin tiny AVRs: ATtiny13 and ATtiny25-85 series.  Arduino Blink sketch compiled for the ATtiny85 is 64 bytes and for the ATtiny13 is 54 bytes.

I am writing this core from scratch, with code size and efficiency as the main goal.  I am making use of AVR assembler code when the code size and efficiency goals cannot be readily attained with C/C++.  Unlike the official AVR core, picoCore has compile-time checking of many arguments.  Calling digitalWrite(42) will cause a compile error with the message, "pin out of range". 


## Development Status
Work in progress as of spring 2020.

Several of the most commonly used functions are implemented as of v0.2. Support for Serial.print is planned for v0.3.

## Supported Functions
* [analogRead()](https://www.arduino.cc/en/Reference/AnalogRead)
* [analogWrite()](https://www.arduino.cc/en/Reference/AnalogWrite)
* [delay()](https://www.arduino.cc/en/Reference/Delay)
* [delayMicroseconds()](https://www.arduino.cc/en/Reference/DelayMicroseconds)   *wrapper for _delay_us()*
* [digitalRead()](https://www.arduino.cc/en/Reference/DigitalRead)
* [digitalWrite()](https://www.arduino.cc/en/Reference/DigitalWrite)
* [millis()](https://www.arduino.cc/en/Reference/Millis)   *Watchdog timer based. Will increase with steps of 16*
* [shiftIn()](https://www.arduino.cc/en/Reference/ShiftIn)
* [shiftOut()](https://www.arduino.cc/en/Reference/ShiftOut)

