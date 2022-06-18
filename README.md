# leather glove
Leather glove with gesture controlled moon cello and tool samples

This is a fun way of using gesture to trigger samples using £20 of hardware. The project is a mish mash of various people's work and is documented with the blessing of all involved.

The hex files for the Pure Data received and Pure Data transmitter come from written by the delightful sound artist and UK based D&T teacher Tom Fox. Find his work at @vulpstrements. He wrote up his version on his blog, where Neill Bogie's (nbogie on github) comments helped me figure out how to get Hairless Midi to work on my Mac https://vulpestruments.com/2018/11/21/how-to-connect-your-mini-mu-to-puredata/ 

For triggering the synth, I actually used Purr Data not Pure Data as I find it more reliable. The patch I've uploaded here is based on one written by Andrew Hockey, a composer and excellent sound wierdo you can find on twitter or insta @andrewrhockey. 

The sounds in the example file are recorded by me at the makerspace in Chicago Pumping Station One, except for the two cello sounds which are part of Sister Moon's awesome sound art project where she bounces samples of various instruments off the moon. Sister Moon is led by Martine-Nicole Rojina and the cello was played by Federico Bragetti.

HOW TO REPLICATE THIS PROJECT (on a mac)

1. Download and install Purr Data: https://github.com/agraef/purr-data/releases
2. Download and install Hairless Midi: https://projectgus.github.io/hairless-midiserial/
3. In Finder, search for and open Audio Midi setup, then click Window > show midi devices and enable the IAC driver. If you have trouble doing this, Neill has helpfully written up how to do that here: https://gist.github.com/nbogie/309848134aede2e57ee80a4b752b0294
4. Next, save the transmitter hex file to your "instrument" microbit and the receiver hex file to a second microbit.
5. The instrument microbit doesn't have to be plugged into your computer. Just power it with a battery pack. The receiver microbit must be connected to your computer with a USB cable.
6. Once both microbits have power and code, you can fire up Hairless midi. Select your USB microbit in the serial port dropdown, and your IAC driver in the midi out.
7. Make some noises! Download the pure data folder and open up the .pd file. 
