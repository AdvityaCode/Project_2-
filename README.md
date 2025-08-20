# 🚘 Automatic Headlight Control System

## Team Members
Emma Valente and Advitya Singh

## 🔦 Project Description
The Automatic Headlight Control System enhances vehicle safety by automating headlight operation based on ambient lighting conditions. 
The system integrates with the Driver’s Education Car Alarm System to ensure proper ignition procedures while providing an automated lighting solution. 
The ignition system ensures that the vehicle starts only when both occupants are seated and belted. 
The headlight system automatically turns headlights on or off depending on environmental light levels when set to AUTO mode.

Project 1 repository that Project 2 was built upon: https://github.com/AdvityaCode/Project1

## 📝 Testing Summary
All system behaviors were tested thoroughly, and all functionalities passed as expected. The table below summarizes the test results for both subsystems.

### Ignition Subsystem
| Specification | Test Result | Comment |
|--------------|------------|---------|
| Display "Welcome to enhanced alarm system model 218-W25" when the driver sits down. | Pass | Message displayed successfully. |
| Enable engine start (light the green LED) when both seats are occupied and seatbelts fastened. Otherwise, print appropriate error messages. | Pass | Ignition Enabled printed if ignitionLED is lit. All error messages display correctly otherwise. |
| Start the engine (light the blue LED, turn off Green) when ignition is enabled and ignition button is pressed. | Pass | Engine starts as expected. |
| Keep the engine running even if the driver/passenger unfastens seatbelt or exits. | Pass | Engine continues running despite seatbelt removal. |
| Stop the engine when the ignition button is pushed and released while running. | Pass | Engine stops as expected. |

### Headlight Subsystem
| Specification | Test Result | Comment |
|--------------|------------|---------|
| Turn on both low beam lamps when the headlight mode selector is set to ON. | Pass | Lights turn on as expected. |
| Turn off all lamps when the selector is set to OFF. | Pass | Lights turn off as expected. |
| In AUTO mode, turn off headlights after 2 seconds when light level is above daylight threshold. | Pass | Delay and operation work correctly. |
| In AUTO mode, turn on headlights after 1 second when light level is below dusk threshold. | Pass | Delay and operation work correctly. |
| Maintain previous headlight state when ambient light is between daylight and dusk levels. | Pass | System correctly holds the last state. |
| Turn off all headlights when the engine is turned off. | Pass | Headlights turn off as expected. |

## 🛠️ Notes
- All features were successfully implemented, and no issues were encountered during testing.
- The system meets all functional requirements and operates as intended.
- Test delays for headlight automation were verified using a mobile timer.
