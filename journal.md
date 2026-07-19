# date:16/7
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
# date:17/7
# time spent:1hr
## description:
i have started the assigning footprints which seemed very easy but i honestly dont know which footprints i have to assign so I searched in the internet and found few but when i applied those in the footprints secction it resulted in errors ,so i had fixed each one many errors were because of the missing pads or the additional pads and now i had added all the footprints and it had no errors too,i am not sure these are permanent i am thinking to do more research and change the switches footprints to other because they may dont suit the deivice thinking of an gameboy switch design ,i will check tomorrow and cahnge those switches footprint again
## images:
<img width="1616" height="880" alt="image" src="https://github.com/user-attachments/assets/c47c2f2b-287b-4f05-b604-cd0705448779" />
<img width="1612" height="885" alt="image" src="https://github.com/user-attachments/assets/759019d2-f2e2-4461-bbcc-86c9bebc2283" />
<img width="762" height="687" alt="image" src="https://github.com/user-attachments/assets/8e4c47fd-af40-494a-8a05-040ebc0ac11b" />
<img width="757" height="678" alt="image" src="https://github.com/user-attachments/assets/38279388-fe3b-4843-9280-116d593442ff" />
<img width="742" height="771" alt="image" src="https://github.com/user-attachments/assets/18794b77-bb63-4605-8c8f-c1b6fe75f25b" />

-------
# date:18/7
# time spent:1.5hr
## description:
In yesterday's journal i have said that i had to change the footprints for the d-pad ,so after searching i had got an perfect footprints that will match and now i got all the objects in a bunch now before i route ,i must arrange all the parts in a perfect layoout so i had arranged all the parts slowly one by one.There were literally 15 capacitors,15 resistors ,and i had arranged in a layout so i had completed the layout and now it is time for the routing!!!
## images:
<img width="755" height="612" alt="image" src="https://github.com/user-attachments/assets/4dc5f05c-dc87-494a-90ae-0f76c07500f7" />
<img width="497" height="613" alt="image" src="https://github.com/user-attachments/assets/8628a73a-23ed-4dfd-b96c-43eefe48635c" />
<img width="730" height="632" alt="image" src="https://github.com/user-attachments/assets/4345f023-1aea-47d3-a38b-2784947a1050" />

-------
# date:18/7
# time spent:1.5hr
## description:
I had completed the routing part which was fun but at the esp2040 it was tough and confusing and then it took most of the time in figuring out how should i place the vias or how should move them,but atlast i have completed the erc and now it is time for the erc and some customisation!!
## images:
<img width="655" height="578" alt="image" src="https://github.com/user-attachments/assets/39d76a48-fcd5-4454-a807-19809433762d" />
<img width="887" height="708" alt="image" src="https://github.com/user-attachments/assets/854c9078-8f8d-4707-a2a9-372f5d222bfd" />

-------

# date:18/7
# time spent:0.75hr
## description:
I had started with the fixing the drc issues and i fixed all of them that were mainly some connection errors or the clearance aerrors,but i checkedd each of them and fixed all and then i have addded images of pokemon in this project and also made it on the sikscreen,now i had completed the pcb part,next is the cad building.
## images:
<img width="772" height="531" alt="image" src="https://github.com/user-attachments/assets/d3ea830c-127c-47dd-b388-aba81b2890ca" />
<img width="816" height="761" alt="image" src="https://github.com/user-attachments/assets/f9c23612-b54f-4666-a826-92c56c3bc645" />
<img width="740" height="655" alt="image" src="https://github.com/user-attachments/assets/429518fa-6e2f-451d-870c-c33e6d3bd492" />

-------
# date:19/7
# time spent:1hr
## description:
Now, i have started the cad part in my project first i have measured the dimensions of the pcb and then plotted in the fusion ,but one major issue is the pcb doesn't has the screen rather it have a small con 01*08 and then i should add the screen so i had searched for the different ypes of screen and i got these 2.8" ILI9341 SPI TFT Display but it was way to big compare to mypcb ,so i have changed it to 2.0" 320x240 Color IPS TFT Display  and it actually fit my case now i should start the case
## images:
<img width="1825" height="822" alt="image" src="https://github.com/user-attachments/assets/41ac2bee-076f-4c18-bcfb-f4c351c1903d" />
<img width="912" height="202" alt="image" src="https://github.com/user-attachments/assets/d701ae4d-d40f-4ca8-a9a8-21cef7f29af4" />
<img width="793" height="652" alt="image" src="https://github.com/user-attachments/assets/e815a362-fb84-43cb-b96a-c141f45ca176" />

-------
# date:19/7
# time spent:1hr
## description:
I had just started building the cad ,at first i built the base with some edges and then curved the corners so that it would be nice and then i had extruded and then i had cut the body for the wholes of the microsd slot and the usb c port which was honestly so time taking as i should measure each of the dimension in pcb and then cut the part in the cad, and then i checked few colors,and the colored it with a red glossy theme.

## images:
<img width="585" height="627" alt="image" src="https://github.com/user-attachments/assets/b6f0d201-b551-4c0d-b2c4-4469425cf61d" />
<img width="602" height="610" alt="image" src="https://github.com/user-attachments/assets/5d4c8b57-3fac-4f28-a89a-2203b2a53462" />
<img width="1182" height="241" alt="image" src="https://github.com/user-attachments/assets/bd2a0d27-cf6c-4dbb-b049-c92cd5488783" />

-------
# date:19/7
# time spent:1hr
## description:
I have just started the cad and too check the dimension of everything i just added the step file from the pcb and to the cad by downloading it and i uploaded in the fusion and then i had checked that the headers are small so i added some part for the base and then i made a cut through for the screen so that it doesn't looks empty.
## images:
<img width="1911" height="747" alt="image" src="https://github.com/user-attachments/assets/fc2c7de8-62b1-4d54-9574-2d97bb43fee6" />
<img width="816" height="727" alt="image" src="https://github.com/user-attachments/assets/ddaf63eb-9938-4bdd-a0e5-0c4f6d464690" />

-------
