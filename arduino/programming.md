# Arduino Programming
### The Arduino Programming Language
The Arduino programming language is similar to C++. (In fact, it really is just C++ with some modifications!) If you are already familar with Java, C, or C++, the Arduino programming language is easy to pick up. This lesson will focus on quirks specific to the Arduino programming language -- refer to the lessons on Java if you need a review on the basics.
### loop() and setup()
Every Arduino program you encounter will have the functions `void loop()` and `void setup()` in it. In fact, the program will not compile without these! Their function is self-explanatory; `setup()` is called exactly once when the Arduino is powered on or reset, and `loop()` is called continously after that. It is important to note that `setup()` is not typically used for defining variables, as they will only be available within the scope of that function and thus will not be able to be accessed in `loop()`.
### Data Types
Because the Arduino environment is based off of C++, data types are the same for the most part. The exception is the double on ATMEGA based boards such as the Arduino Uno -- it is 4 bytes (32 bits), the same as a float. The data types are listed below for reference:
- `boolean` (8 bit): Either true or false.
- `byte`    (8 bit): Number with a value 0-255, unsigned
- `char`    (8 bit): Number with a value -128-127, signed
- `word`	 (16 bit): Unsigned integer 0-65535
- `int`	 (16 bit): Signed integer -32768-32767
- `long`   (32 bit): 0-4294967295. Can be signed as well.
- `float`  (32 bit): Signed floating point number (decimal). Same as a double on ATMEGA boards.

### Input and Output
Arduinos communicate to the outside world through the various IO pins. The two main types of input and output are Digital and Analog (yes, there is serial, I2C, and other types but that's a story for another time).
##### Digital
Digital communication is very simple. As the Arduino runs on 5 volts, each pin is allowed to output either 5 volts or 0 volts, which leaves 2 states per pin. This is usually the preferred method because of its simplicity. However, because it operates in binary, communicating lots of data over a single digital input/output pin would be very slow.
##### Analog
Analog communication is similar to digital. Instead of sending either 5V or 0V, the pin can send a voltage in between. In software, analog inputs can detect with the precision of 0.04 volts (5v/1023). However, the reading is not always accurate, so an analog signal is usually used in sensors that can be "close enough". Unfortunately, because of the simplicity of Arduinos, they cannot send a true analog signal. Instead, they send a PWM (Pulse Width Modulation) output. This makes a pin oscillate between 0V and 5V. Depending on the cycle speed, the average output voltage may vary.

### Example Program

### Further Reading and References
