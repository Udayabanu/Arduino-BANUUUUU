#include <Adafruit_NeoPixel.h>
#ifdef __AVR__
#include <avr/power.h>
#endif

int const NUM_PIXELS = 12;
int8_t const PIN = 13;
;
Adafruit_NeoPixel strip;

void setup() {
  strip = Adafruit_NeoPixel(NUM_PIXELS, PIN, NEO_GRB+NEO_KHZ800);
  strip.begin();
  strip.show(); // Init all pixels to "off"
}

void loop() {
  // Colors are defined in 0xRRGGBB format. 
  strip.setBrightness(6);
  for (int i = 0; i < 12; i++) {
   strip.setPixelColor(i, 0x1801a9);
   strip.show();
   delay(69);
   strip.setPixelColor(i, 0x150812);
      strip.show();
   delay(10);
   strip.setPixelColor(i, 0xff7400);
      strip.show();
   delay(50);
}
}

 # Arduino-BANUUUUU
BanuBanuBanuBanuBanuBanuBanuBanuBanuBanuBanuBanuBanuBanuBanuBanuBanuBanuBanuBanuBanuBanuBanuBanuBanuBanuBanuBanuBanuBanuBanuBanuBanuBanuBanuBanuBanuBanuBanuBanuBanuBanuBanuBanu
