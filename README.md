# Ez-TImers
Lightweight python library, that add's the ability to call functions repeatedly.

## How to use

1. Download the file, and place it in a known directory.<br>
2. Import the module 'Repeated_Timer' to your python file.<br>

```
from Ez_Timers import Repeated_Timer
```

3. Initialize a Repeated_Timer object, with the interval, the task you want it to perform, and all the args / qwarg needed.

'''
def foo():
    print("Hello")


My_Timer = Repeated_Timer(0.5, foo)
My_Timer.Start()
'''
