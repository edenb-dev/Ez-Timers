# Ez-TImers
Lightweight python library, that add's the ability to call functions repeatedly.

## Use cases

* Heart Beat - Check if a server connection is still live every x seconds.
* Updating Data - making a "real-live" connection to a DB.

*Any thing you need to execute every x times*

## How to use

### Initializing the timer

1. Download the file, and place it in a known directory.<br>
2. Import the module 'Repeated_Timer' to your python file.<br>

```
from Ez_Timers import Repeated_Timer
```

3. Initialize a Repeated_Timer object, with the interval, the task you want it to perform, and all the args / qwarg needed.


```
def foo():
    print("Hello")

My_Timer = Repeated_Timer(0.5, foo)
```

### Starting the timer

Execute the 'Start' function on your newly created Repeated_Timer object.

```
My_Timer.Start()
```

### Stoping the timer

Execute the 'Stop' function on your Repeated_Timer object.


*In this example the foo function will run every 0.5 seconds*


