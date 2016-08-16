# LCD-16X2

#include <Wire.h> 
#include <LiquidCrystal_I2C.h>


LiquidCrystal_I2C lcd(0x3F,16,2);  // set the LCD address to 0x27 for a 16 chars and 2 line display

char HABITACIONN;
int llamadohabitacion = 0;
void setup()
{
  lcd.init();                      // initialize the lcd 
    // Print a message to the LCD.
   
  lcd.backlight();
  lcd.setCursor(0,0);
  lcd.print("T");
  lcd.setCursor(1,0);
  lcd.print("E"); 
  lcd.setCursor(2,0);
  lcd.print("S"); 
  lcd.setCursor(3,0);
  lcd.print("T"); 
  lcd.setCursor(0,1);
  lcd.print("L");  
  lcd.setCursor(1,1);
  lcd.print("C"); 
   lcd.setCursor(2,1);
  lcd.print("D");  
  
}


void loop()
{
}
