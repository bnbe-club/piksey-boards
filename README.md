# Piksey Boards
The files contained in this repository have been derived from the following repository. <br>
https://github.com/watterott/ATmega328PB-Testing

### Installing On Arduino IDE 1.8+

**1. Add URL for Piksey Boards** <br/>
Start by adding the following URL to the Arduino Boards Manager. You can do this by opening up the preferences window (Windows: *File->Preferences*, OS X: *Arduino->Preferences*) and locating the "Additional Boards Manager URLs" section. 

If you already have an existing URL then simply add this URL to a new line. Click OK when done.

   ```
   https://github.com/bnbe-club/piksey-boards/raw/master/package_piksey_boards_index.json
   ```

**2. Install the boards** <br/>
Next, open up the boards manager (Windows: *Tools->Board->Boards Manager*, OS X: *Tools->Board->Boards Manager*)

Search for "Piksey Boards" and you should be able to locate an entry by "Bits N Blobs Electronics". Install the latest version (1.0.0) and close the window when done.

**3. Select the boards** <br/>
The new boards should now be available for use. Select the appropriate board under the *"Piksey Boards"* section (Windows: *Tools->Board*, OS X: *Tools->Board*). If you are using Windows, then you will also need to specify the COM Port like always (*Tools->Port*)

That's it! You can now start uploading your code.

### Backward Compatibility

The Piksey Pico and Nano are designed with the Microchip ATmega328PB microcontroller. This is a newer microcontroller and is not 100% pin compatible with the older ATmega328P commonly found in the Arduino Uno and Arduino Nano. The ATmega328PB has more features and is software compatible with the older ATmega328 which means that existing sketches for the Arduino Uno and Nano will run without the need to change the code. More information about the differences between the two microcontrollers can be found in the following document:

[Differences Between ATmega328PB and ATmega328P - AT15007](https://github.com/bnbe-club/piksey-boards/raw/master/docs/Atmel-42559-Differences-between-ATmega328P-and-ATmega328PB_ApplicationNote_AT15007.pdf)


