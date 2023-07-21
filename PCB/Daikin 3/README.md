This is 3rd generation design that works with WESMO D1 Mini ESP32 clones like https://www.amazon.com/gp/product/B08PNWB81Z/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1 
Unlike the original design, I used a 5 volt step down converter and a TI level shifter 3.3v<->5v that should works with most units.
Board designed in EasyEDA for jlcpcb.com production. Jlcpcb production cost about $55 for 10 boards that much cheaper than original Faikon boards because of cheap single side assembly.


Advantages vs original design:
 - True level shifter for RX/TX with onboard 5v converted. Original design v1 level shift just RX pin but v2 design required 5v on pin 5 that some units does not have.
 - Do not invert RX pin that simplify config in esphome
 - 2x Cheaper to order because of economic vs standard PCB assembly


Disadvantages vs original design:
 - Required external ESP32 board
 - Bigger and bulky
 - Needs some assemply to attach D1 Mini ESP32 board