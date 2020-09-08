# Ez-Timers
Lightweight python library, that add's the ability to call functions repeatedly.

## Use cases

* Heart Beat - Check if a server connection is still live every x seconds.
* Updating Data - making a "real-live" connection to a DB.
* Grate example on how to incorporate our module into your project **[Ez-Animations](https://github.com/edenb-dev/Ez-Animations)**

*Anything you need to execute every x seconds.*

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

To start the timer, execute the 'Start' function on your newly created Repeated_Timer object.

```
My_Timer.Start()
```

### Stoping the timer

To stop the timer, execute the 'Stop' function on your Repeated_Timer object.

**Execute 'Stop' will not stop the function midway.<br>**
**The funciton will still run till it finishes, but will not re-excute further.**  

```
My_Timer.Stop()
```


*In this example the foo function will run every 0.5 seconds.*


