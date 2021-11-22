# BiQu-B1-Klipper-Config

I'm getting a BiQu HermitCrab CAN Tool-Changer for my BiQu B1 Printer.
To Date, the Printer is running Marlin Firmware with Octoprint.

The HermitCrab CAN makes it necessary to move it from Marlin to Klipper, as support for multiple MCUs is required.

This is a draft configuration for the upcoming Modification of my BiQu B1 to run Klipper

Note that it is as of yet untested due to Hardware still being in the mail

Current Configuration:
- BiQu B1 w/ SKR 1.4 Turbo (instead of stock SKR 1.4)
- TMC 2209 Stepper-Drivers
- Sensorless Homing
- Linear Rails for X and Y
- Dual Z-Drive
- BL-Touch (3DTouch)
- Additional NeoPixels above Bed
- Bowden-Style Extruder upgraded to Dual-Gear Setup
- Stock Hot-End, but with Capricorn Tubing
- Replaced PSU with 350W MeanWell PSU

Changes coming with the Transition to Klipper
- Replacement of X, Y, Z Stepper Motors with 0,9° Steppers
- HermitCrab CAN Toolchanger (To add Support for Laser)
- BiQu H2 Extruder
- Additional ADXL345 hardmounted to Bed
- Replacement of bed with one that hopefully is less warped and has better insulation underneath
- As the new bed is slightly more powerful than the SKR1.4 is rated for, the installation of a separate Power-MOSFET to drive Bed-Power is also taking place


The intent is also to move the Chassis-Fans off of permanent power to switched outputs (possibly with Temperature-Sensing and PWM)
