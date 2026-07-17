<img width="1723" height="667" alt="image" src="https://github.com/user-attachments/assets/edf69f8c-847a-40c1-88f2-08b5e5468ae1" /># date:16/7
# time spent:1hr
## description:
To plan my custom handheld Pokédex, I researched open sourced retro consoles and electronics websites like mouser to find parts that balance performance.For the brain, I chose the powerful ESP32-S3  I paired this with a sharp 3.5inc ips display. The system features a rechargeable 2500 mAh li-po battery for hours of battery life, a MicroSD card slot to store the massive library of Pokemonn data and images, and a USB-C port connected directly to the chip for easy charging and programming. I included a physical D-pad (Up, Down, Left, Right, and an OK button), A/B action buttons, a 1W speaker with a small amplifier to play sound or noises.
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
