# Morse Pattern

## About

Designed by Jacob Joaquin. This pattern was originally used at Bedouin Tech 2017 in Dubai, lighting up The Crypto GeoTemple by The Eye.

## Setting the Morse Code Message

Open *generateMorse.py* and change the quote.

```python
quote = 'HELLO WORLD AND WELCOME TO ROOT ACCESS HACKERSPACE WERE READY TO BELIEVE YOU'
```

Run *generateMorse.py*. This will generate *encoded.h*.


## Choosing your Color Palette

You can used one of the pre-defined colors or create your own with the *rgb* macro.

```c
uint32_t orange = rgb(255, 64, 0);
uint32_t magenta = rgb(255, 0, 128);
uint32_t black = rgb(0, 0, 0);
uint32_t white = rgb(255, 255, 255);
uint32_t red = rgb(255, 0, 0);
uint32_t purple = rgb(128, 0, 128);
uint32_t green = rgb(0, 255, 0);
uint32_t cyan = rgb(0, 128, 128);
```

Add two or more colors to *palette[]* to change the color scheme.

```c
uint32_t palette[] = {black, magenta, cyan};
```

## Setting the frameDelay

To change the rate of change in the pattern, search for following line:

```c
const int frameDelay = 1000 / 60;
```

The units are *1000ms / framesPerSecond*.
