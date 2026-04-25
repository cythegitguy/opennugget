## Adafruit PCM5122 I2S DAC with Line Level Output - HW, I2C or SPI PCB

<a href="http://www.adafruit.com/products/6421"><img src="assets/6421.jpg?raw=true" width="500px"><br/>
Click here to purchase one from the Adafruit shop</a>

PCB files for the Adafruit PCM5122 I2S DAC with Line Level Output - HW, I2C or SPI. 

Format is EagleCAD schematic and board layout
* https://www.adafruit.com/product/6421

### Description

For converting digital I2S audio from your ESP32/RP2350 or Raspberry Pi, you'll need a digital-to-analog-converter (DAC). And the <b>Adafruit PCM5122 I2S DAC</b> is both powerful and easy to use - with excellent audio quality!  It's got clean, high-quality, stereo audio and does not need any MCLK signal, or I2C configuration. Literally just pipe some I2S audio in and it ill just work.

The default hardware mode is excellent for quick starts, and, for those who do want configurability such as volume control / software mute / EQ / filters, it's also easy to set up the chip for I2C or SPI interfacing with the two MODE pins.

The PCM5122 has excellent audio specs, with 112dB signal-to-noise/dynamic range, and -93 dB THD.

This breakout makes I2S digital audio easy: all you need to do is power it with 3~5VDC, and provide BCLK (bit clock), WSEL (left/right word select), and DIN (data in). The data lines are 3.3V logic only. By default it's configured for I2S but you can also do Left-Justified by toggling the Format pin. Audio can be 16, 24 or 32-bit wide, the chip will automagically determine the right format from the WSEL / BCLK ratio. No MCLK pin is needed, the chip will auto-generate it internally from the bit clock - or you can provide it on the MCLK input if you want.

For hardware (not I2C/SPI config mode) the other breakout pads provide:

* <b>Filtering</b> (change from normal to low-latency by pulling high)
* <b>De-emphasis</b>
* <b>Mute</b> (pull low to quickly set the outputs to ground), and de-emphasis for 44.1khz audio (default is off)
* Three <b>ATTenuation/gain</b> pins that can be used for changing the gain from -6dB to +15dB. See the datasheet's Table 3 for the pin-to-gain settings.

For I2C/SPI configuration mode, gain/volume, filtering and de-emphasis is done over digital register commands. The hardware Mute pin still works as expected.

The audio outputs are also available on breakout pads if you want to wire directly without using the 3.5mm jack. Audio output is not AC-coupled because it is centered on ground: you can plug it into anything that is either AC coupled or has the same ground reference. Note that this is a line-level output, it cannot drive headphones - the output is for no less than 1K ohm loads!

Each order comes with one I2S Stereo DAC breakout and some header you can solder on for breadboard usage.

### License

Adafruit invests time and resources providing this open source design, please support Adafruit and open-source hardware by purchasing products from [Adafruit](https://www.adafruit.com)!

Designed by Limor Fried/Ladyada for Adafruit Industries.

Creative Commons Attribution/Share-Alike, all text above must be included in any redistribution. 
See license.txt for additional details.
