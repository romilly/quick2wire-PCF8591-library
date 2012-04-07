# PCF8591 8-bit A/D and D/A converter library and test suite

version 0.1 - this is a work in progres: neither the library nor the test have been written yet!

This is an Arduino library and test sketch for [nxp](http://www.nxp.com/)'s [PCF8591](http://www.nxp.com/documents/data_sheet/PCF8591.pdf) 8-bit A/D and D/A converter.

It requires Arduino 1.0 or later. If you want to use it with Arduino 22 you will need to modify some of the Wire calls.

The library should be installed in the usual way: in other words, the directory `library/PCF8591` and its contents should be copied to the `<arduino-1.0-install-dir>/libraries/` directory.

## Test process

The Adruino is wired up to a board carrying the PCF8591. The test sketch applies known voltages to the PCF8591's ADC channels and measures the voltage output by the DAC.

The tests are run repeatedly within `loop`, and the results are reported via Serial comms at 9600 baud.

This allows you to verify that the tests are actually testing things by removing and replacing the wires that connect the Arduino to the board under test.

There's a [Fritzing](http://fritzing.org/) schematic which describes the wiring between the board under test, and a photo of the test configuration.

 
