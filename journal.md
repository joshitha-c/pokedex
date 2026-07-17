<img width="1035" height="767" alt="image" src="https://github.com/user-attachments/assets/e8dfc168-db4e-439c-8149-b3118a6095a4" /># date:16/7
# time spent:1hr
## description:
To plan my custom handheld Pokedex, I researched open sourced retro consoles and electronics websites like mouser to find parts that balance performance.For the brain, I chose the powerful ESP32-S3  I paired this with a sharp 3.5inc ips display. The system features a rechargeable 2500 mAh li-po battery for hours of battery life, a MicroSD card slot to store the massive library of Pokemonn data and images, and a USB-C port connected directly to the chip for easy charging and programming. I included a physical D-pad (Up, Down, Left, Right, and an OK button), A/B action buttons, a 1W speaker with a small amplifier to play sound or noises.

------
# date:16/7
# time spent:1hr
## description:
I have successfully wired up the esp3 controller and the main power part for the Pokedex in kicad. First, I placed the ESP32-S3 chip right in the middle. Then, connected up the USB-C port so it can talk directly to the chip s data pins. To control the device, I added two tactical buttons: the Reset Button and also  which uses a resistor and capacitor to reboot the chip when pressed, and the Boot Button , which tells the chip to go into programming mode so I can upload the Pokedex software. Finally, I added all the basic power connections so everything has a safe now.
## images:
<img width="708" height="507" alt="image" src="https://github.com/user-attachments/assets/d2d0e04a-b77c-4f1a-b8ea-9334ded819fb" />
<img width="868" height="605" alt="image" src="https://github.com/user-attachments/assets/70baf7f5-7edc-4c52-9b8c-fe733dfd21d8" />

-------
# date:17/7
# time spent:1hr
## description:
so far i got the esp32-s3 chip put down right in the middle of the page and connected with usb-c port so it can connect with the data pins. i also added the reset and boot buttons with the little capacitor and resistor tricks so i can actually upload the pokedex software later. after that i started working on the power stuff with a tp4056 charger and also i added some input capacitors to clean up the noise. i messed up a many times by accidentally ran the main power wire straight through the ground pin of the regulator which would have made things worse but i somehow fixed it.The next step is  where i'll add the display screen and wire them up.
## images:
<img width="886" height="478" alt="image" src="https://github.com/user-attachments/assets/c15a50fc-dd93-4f43-a8ae-b827fbb8ea8b" />
<img width="1723" height="667" alt="image" src="https://github.com/user-attachments/assets/ff948acf-b935-448c-92a7-92d8f630288f" />
<img width="1327" height="787" alt="image" src="https://github.com/user-attachments/assets/36a4df69-9d7e-4e51-852e-2075619ce1a6" />

-------
# date:17/7
# time spent:1hr
## description:
So far i have moved on to the display, i placed an 8-pin connector for the ST7789 module, added a 100nF capacitor , and also connected the backlight to 3.3V, and mapped the SPI lines to GPIO10, GPIO8, GPIO9, GPIO11, and GPIO12.
I then added the a microSD card socket with a 100nF bypass capacitor and a 10k pull-up resistor . I initially made a few critical mistakes including an accidental dead short circuit across the capacitor and grounding the the resistor i then rechecked it and found the mistake and then i resolved it.
## images:
<img width="1121" height="676" alt="image" src="https://github.com/user-attachments/assets/65a50b19-6c93-48d8-a041-2a132ecc9267" />
<img width="1045" height="596" alt="image" src="https://github.com/user-attachments/assets/a7cc148a-eaad-443d-94bf-5959de8a2805" />

-------
# date:17/7
# time spent:1hr
## description:
first i have researched about different kinds of switches and then I added the buttons and sound for the device!For the D-pad and action buttons, i made a set up a layout using clicky little switches that sit right under a plastic cross cap, so every press feels responsive when you're clicking through menus. On the audio side, i kept a  that would've accidentally muted the whole thing but somehow fixed the error!
## images:
<img width="927" height="432" alt="image" src="https://github.com/user-attachments/assets/a4b7664d-8a31-4307-8793-ffd90ac7b779" />
<img width="696" height="365" alt="image" src="https://github.com/user-attachments/assets/94ac835c-83dd-4fc9-9963-105d5f8dea15" />
<img width="296" height="346" alt="image" src="https://github.com/user-attachments/assets/6ba5347d-30b3-495d-b643-d865078f7d43" />

-------
# date:17/7
# time spent:1hr
## description:
Firstly i searched about different types of rgb light neede i thoought to keep the red rgb light but thinking about the future need i thought to kep an neopixel stick so that it supports ll the rgb light for my pokedex and i have completed all the changes needed for the v1 and now i have ran erc and there were many erros i have fixed all of them there we around 30 errors fixed each of them by going through every error block and then i completed solving the every errors and the errors count has become to 0!!
## images:
<img width="1035" height="767" alt="image" src="https://github.com/user-attachments/assets/52927304-03e3-477d-8bd7-71ab62d87ae5" />
<img width="695" height="463" alt="image" src="https://github.com/user-attachments/assets/9ec4cacf-af38-4780-9c7f-8177b085e733" />
<img width="1127" height="793" alt="image" src="https://github.com/user-attachments/assets/4ad82eb1-092e-40a7-9513-391762363393" />
<img width="693" height="457" alt="image" src="https://github.com/user-attachments/assets/78169851-698c-4c8b-8bcf-b4b5ac382ad8" />

-------

