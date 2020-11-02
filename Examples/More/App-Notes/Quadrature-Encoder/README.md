## Rotary Encoder Examples:

These two examples were made for the [Photoelectric Rotary Encoder - H38S100B](https://labjack.com/support/app-notes/digital-IO/photoelectric-rotary-encoder-H38S100B) application note.  


### Quadrature-Input.vi
The Quadrature-Input.vi is a basic example that opens a device, configured it, and then reads back data.

### Quadrature_Input_Example_Application.vi
The Quadrature_Input_Example_Application.vi is a more advanced producer-consumer loop based application that can be built and run as a .exe.

### Changelog
v1: Switched to using "_READ_A" and 2s compliment calculations for determining position.
v0: Initial release.