# stephenlong-audioplayer

Design a custom PCB for Bluetooth audio player using ESP32. The system includes an Audio Player and Album card using ESP32. There are two devices: one is the music player and another is the album. When album is powered on, it will pair with the player board automatically and transfer music streaming to the player. The player will output it. The block diagram was tested and you can design the main circuit based on the diagram. The problem is the power circuit. The Album will have the wireless charging receiver and the player board will have the transmitter. When the album is closed to the player board, it will be powered on by wireless charger. Dont need any battery and USB power in the album board. The player board will have the USB port as a power source.

The Album card consists of an ESP32, an SD card slot, and a Wireless charger. The Album will be powered by the Wireless Charger supplied by the Audio Player. The Album will read audio files from the SD card and transfer audio streaming to the Audio Player over Bluetooth LE.

The Audio Player consists of ESP32, Audio Stereo DAC, Wireless Power Transmitter, LEDs, and Switches. The Audio Player will receive the Bluetooth streaming from the Album and output it over the stereo microphone.


If users take Album away from the Audio Player, the audio streaming will be stopped because the Wireless charging is off. You can check the docs. It includes the block diagram and reference for the wireless charging receiver and transmitter.
