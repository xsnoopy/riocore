# blink
**blinking output pin**

outputs a fixed frequency / was used to indicate that the FPGA is runing / no control signals


![image.png](image.png)

## Basic-Example:
```
{
    "type": "blink",
    "pins": {
        "led": {
            "pin": "0"
        }
    }
}
```

## Pins:
*FPGA-pins*
### led:

 * direction: output


## Options:
*user-options*
### frequency:
blink frequency in Hz

 * type: float
 * default: 1.0
 * unit: Hz

### name:
name of this plugin instance

 * type: str
 * default: None


## Signals:
*signals/pins in LinuxCNC*


## Interfaces:
*transport layer*


## Full-Example:
```
{
    "type": "blink",
    "frequency": 1.0,
    "name": "",
    "pins": {
        "led": {
            "pin": "0",
            "modifiers": [
                {
                    "type": "invert"
                }
            ]
        }
    },
    "signals": {}
}
```

## Verilogs:
 * [blink.v](blink.v)
