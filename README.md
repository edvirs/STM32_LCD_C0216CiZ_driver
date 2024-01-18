# STM32_LCD_C0216CiZ_driver
STM32 I2C Driver for the NHD-C0216CiZ-FSW-FBW-3V3 LCD Display

## Example

```c
#include "LCD_C0216CiZ_driver.h"

int main(void){ 
    //...main initializations...
    
    HAL_GPIO_WritePin(LCD_Reset_GPIO_Port, LCD_Reset_Pin, GPIO_PIN_SET);
    LCD_INIT();
    
    char *str = "Hello World!";
    LCD_PRINT_STR(str, 0);
}
```
