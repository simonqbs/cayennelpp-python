# Cayenne LPP

Tested on a Lopy running micropython.

## Instructions (for LoPy)

Copy `CayenneLPP.py` to the `lib/` directory and in your `main.py` use
this example code:

```python
from CayenneLPP import CayenneLPP

var cayenne = new CayenneLPP();
cayenne.add_temperature(1, 23.54);

# ... lora setup ...
s.send(cayenne.get_buffer())
```

## Credits

Based on: https://github.com/TheThingsNetwork/arduino-device-lib/blob/master/src/CayenneLPP.cpp