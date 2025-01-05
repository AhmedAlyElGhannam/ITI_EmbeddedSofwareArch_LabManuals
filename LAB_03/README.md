void MDIO_vInit(void);

Purpose:
The DIO_init function initializes all digital I/O pins based on the configuration defined in the PinCfg array.

Parameters
  void  
Return:
  void
______________________________________________________________________________________________________________________________________________________

OPTIONAL IF YOU NEED TO IMPLMENT IT 

void MDIO_vSetPin(uint8_t Copy_u8PortNum, uint8_t Copy_u8PinNum, uint8_t Copy_u8Value);

Purpose:
The DIO_setPin function is used to control the digital state of a specific pin on a given port in a microcontroller.
It allows setting a pin to either a high (logic 1) or low (logic 0) state.

Parameters

    uint8_t Copy_u8PortNum:
        The port number to which the pin belongs.

    uint8_t Copy_u8PinNum:
        The specific pin number within the selected port to be modified.

    uint8_t Copy_u8Value:
        The desired state to set the pin to:
        -High state (logic 1).
        -Low state (logic 0) .
Return:
  void
______________________________________________________________________________________________________________________________________________________

Application: Controlling 3 LEDs with 3 Buttons

This application simulates a simple digital control system where three push-buttons are used to control the state of three LEDs independently. 
Each button corresponds to a specific LED, allowing users to turn the LED on or off by pressing the associated button.


