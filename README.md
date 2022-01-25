# Make a Theremin like musical instrument
![](ThereminPameliaStickley.jpg)    
In this lab we will make a musical instrument that is controlled with the micro:bit light sensor. The light sensor will respond to the shadow of our hand, so we won't need to actually touch it to make it respond. This will create an instrument similar to a [Theremin](https://en.wikipedia.org/wiki/Theremin), an electronic musical instrument that is played without touching it.

You may find slides 116 - 122 of the [slide presentation](https://docs.google.com/presentation/d/1aiGcnPn8uoCJdX8p7_qoI3Hh3_KOhUtFeB3Byw0tacA/edit?usp=sharing) helpful in completing this assignment.

### Step 1: Run this sample program

```python
from microbit import *
import music

while True:
    music.pitch(440,1000) #play A for one second
    sleep(1000)
```
The `import music` lets the program use functions from the micro:bit music module. By default sound output will be via the built-in speaker on the V2 micro:bit. The `music.pitch(frequency, milliseconds)` function takes two arguments and plays a pitch at the integer `frequency` given for the specified number of `milliseconds`.
In the sample program the frequency is set to 440 for 1000 milliseconds. When you run the program on a V2 micro:bit, you will hear a standard concert A for one second, followd by one second of silence. If the second argument is set to `-1`, the music pitch will continue to sound until another music pitch is played.

### Step 2: Suggested steps to getting started
1. Create a variable `freq` that stores the current light sensor reading from `display.read_light_level()`
2. To get the frequency in the typical range of hearing, you could multiply it by 20 and add 200
3. Call `music.pitch(freq, -1)`. The second argument `-1` makes the sound continue until this is a new call to `music.pitch()`
4. Adjust the amount you multiply and add to the frequency to match the light levels in the room
5. Submit your code to google classroom. Since there is no visable aspect to this project, it is not necessary to submit a video of your program running.

### Extensions
Feel free to modify your theremin circuit or code in any way you wish. Have fun and be creative, your theremin doesn't have to work or sound like any other. You could also go back and add sound to your egg catcher game.

