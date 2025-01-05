
void HSEVENSEG_vInit(void);

Purpose:
The HSEVENSEG_vInit function is responsible for initializing and configuring the pins of seven-segment displays based on the provided configuration.

Parameters:

   void

Return:
   void

Example : 
    HSEVENSEG_vInit();

____________________________________________________________________________________________________________________________________________________________________________

void HSEVENSEG_vSetValue(u8 Copy_enuSevenSegNum , u8 Copy_u8Value);

Purpose :
    HSEVENSEG_enuSetValue function is responsible for configuring a 7-segment display to show a specific value (0-9) 
on a particular segment module identified by Copy_enuSevenSegNum


Parmeters:

   Copy_enuSevenSegNum:
        Specifies which seven-segment display you want to control.

           Example:

           HSEVENSEG_SevenSegNum1 = 0 (First display)
           HSEVENSEG_SevenSegNum2 = 1 (Second display)
           .
           .

   Copy_u8Value:
 
    The value you want to display on the specified seven-segment display.

    Commonly, this parameter is expected to be a digit (0-9) because seven-segment displays typically represent single digits.

Return:
   void

Example : 
  HSEVENSEG_vSetValue(HSEVENSEG_SevenSegNum1 , 7);
____________________________________________________________________________________________________________________________________________________________________________
HSEVENSEG_enuErrorStatus_t HSEVENSEG_enuSetMultiDigitValue(u16 Copy_u16Value);

Purpose :
    The function HSEVENSEG_enuSetMultiDigitValue is used to display a multi-digit number (Copy_u16Value) across multiple seven-segment displays, 
depending on how many are configured (up to 4 in this case).

Parameters:

     Copy_u16Value :

        Description: This is the number to be displayed on the seven-segment displays.

        Expected Range:
            The range of valid input depends on the number of configured seven-segment displays:
                1 segment :  Valid values are  0-9.
                2 segments:  Valid values are  0-99.
                3 segments:  Valid values are  0-999.
                4 segments:  Valid values are  0-9999.


Return Type:
    HSEVENSEG_enuErrorStatus_t:
        An enumerated type that represents the status of the operation.
        Possible values:
            HSEVENSEG_enuSevenSegLimitError: Indicates that the input number exceeds the range supported by the number of configured seven-segment displays.
            .
            .
            .
Example : 
  HSEVENSEG_enuSetMultiDigitValue(4078);;
____________________________________________________________________________________________________________________________________________________________________________
