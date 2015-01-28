This lib is based on Adafruit lib to ws2801. Changed to be usable with apa102 led pixels.
The original library can be found here: https://github.com/adafruit/Adafruit-WS2801-Library

It was modified by Matan led
Have the license it should have. MIT/GPL/fuck it and be good people!

I used a data sheet I found in the link:
https://app.box.com/s/8oevda04rtxruji01vje

Speeds:
I conducted some tests with my 72 pixels led strip.
When use SPI connection:
A loop of 100 times strip.show() takes about 280 miliseconds
A loop of 10000 times Strip.setpixel() takes 4 miliseconds
When use bit-bang connection(just choose 2 pin you like):
A loop of 100 times strip.show() takes about 1300 miliseconds
Strip.setpixel() takes the same

It was enough for simple POV POC

Enjoy