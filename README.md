# python-orvibo

Control Orvibo devices with Python 3. Currently supports the S20 WiFi Smart Switch.

## Usage

```python
from orvibo.s20 import S20

s20 = S20("x.x.x.x") # Discover the IP on your own.
print(s20.on) # Current state (True = ON, False = OFF).
s20.on = True # Turn it on.
s20.on = False # Turn it off.
```

There is also a command line version to achieve the same, e.g.

```
python cmd.py --server 1.2.3.4 --switch off
python cmd.py --server 1.2.3.4 --switch on
python cmd.py --server 1.2.3.4 --status
```

## Contributions

Pull requests are welcome. Possible areas for improvement:

* Discover configured devices (get IPs).
* Additional Orvibo devices.
* Expand S20 functions: Timers, configuration, etc

## Disclaimer

Not affiliated with Shenzhen Orvibo Electronics Co., Ltd.
