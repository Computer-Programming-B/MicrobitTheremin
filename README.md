# Make a Theremin like musical instrument
![](ThereminPameliaStickley.jpg)![](Theremin.jpg)   
In this lab we will make a musical instrument that is controlled with the micro:bit light sensor. The light sensor will respond to the shadow of our hand, so we won't need to actually touch it to make it respond. This will create an instrument similar to a [Theremin](https://en.wikipedia.org/wiki/Theremin), an electronic musical instrument that is played without touching it.

### Step 1: Run this sample program

```python
from microbit import *
import music

while True:
    music.pitch(440,1000) #play A for one second
    sleep(1000)
```
The `import music` lets the program use functions from the micro:bit music module. By default sound output will be via the built-in speaker on the V2 micro:bit. The `music.pitch(frequency, milliseconds)` function takes two arguments and plays a pitch at the integer `frequency` given for the specified number of `milliseconds`.
In the sample program the frequency is set to 440 for 1000 milliseconds. When you run the program on a V2 micro:bit, you will hear a standard concert A for one second. Followd by one second of silence.

### Step 2: Modify the code
TBD

### Extensions
Feel free to modify your theremin circuit or code in any way you wish. Have fun and be creative, your theremin doesn't have to work or sound like any other

