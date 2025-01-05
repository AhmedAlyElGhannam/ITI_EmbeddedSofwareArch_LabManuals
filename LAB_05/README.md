Assignment for Lab 5
Deadline for Submission: Sunday, Jan 5, by 11 AM
Requirement: Software Implementation of Drivers

LED Driver:
Initialization: Initialize the LED driver with LED_init();
Set State: Set the LED state using LED_enuSetLedState(u8 Copy_u8LedName, u8 Copy_u8State);
Configurability: The LED driver must be configurable by the user to support different LED configurations and states.

Switch Driver:
Initialization: Initialize the switch driver with SWITCH_init();
Set State: Set the switch state using SWITCH_enuErrorStatus_t SWITCH_enuGetSwitchState(u8 Copy_u8SwitchName, u8* Add_pu8State);
Configurability: The switch driver must be configurable by the user to support different switch configurations and states.

Please ensure that all implementations adhere to the specified function prototypes and are thoroughly tested before submission.
