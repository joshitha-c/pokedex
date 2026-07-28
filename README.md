# ESP32 Pokedex Handheld Device:
* Its a retro pokedex handheld built using an ESP32 DevKit V1, a 2.8" ILI9341 TFT LCD, directional buttons, a microsd card module, and a passive buzzer.
and in the v1 i have made the dedign in the kicad and then i had built the case and then the software part is built in wokwi simulator in this version i had built a pokedex which you can browse pokemon and then i also added a feature named who's the pokemon? which the player guesses the pokemon by image.
---

## Features

* Pokemon Browser:For the v1 version i had included only a few pokemons with their basic details like the attack type and description
* Who's That Pokemon? Mini Game: There is a section named who's the pokemon in which there would be a image beside that the user selects the correct pokemon in those options.
* Settings & Power: TYou can restart the device in the settings section and then mute the device in the settings section,In the simulator i have added a potentiometer hat can represent a battery aand you can see the percentage in the battery section in device.

* Flexible Display: The drawings are in the microsd which is then converted into bitmap arrays for displaying the pokemons.

---

## Hardware 


* Microcontroller- ESP32 DevKit V1 
* Display- 2.8" ILI9341 SPI TFT LCD 
* Storage- MicroSD Card SPI Module 
* Input-Tactile Push Buttons 
* Audio- 5V / 3.3V Passive Buzzer 
* Battery Sense Potentiometer (Wokwi) or Voltage Divider (LiPo Battery) 
---
## Tech Part:

### Software & Firmware:Wokwi online simulator.
### Hardware: Kicad,Fusion 360.
---

## AI Use:

* I also used some debugging errors and some color changes with layout and i learnt from ths ,how to use wokwi simulator.
---
## How to Open and Use the ZIP Project in VS Code

Follow these steps to extract, open, and run the project inside Visual Studio Code using PlatformIO and the Wokwi Simulator.
The zip file:it is in repo releases.
### 1. Unzip the Project Folder
1. Locate the downloaded `.zip` file on your computer.
2. Right-click the `.zip` file and select **Extract All...** (Windows) or double-click it (macOS).
3. Choose a destination directory (e.g., your Desktop or Projects folder) and finish the extraction.

---

### 2. Install Required Extensions in VS Code
If you haven't set up Visual Studio Code for ESP32 development yet, install the required tools:

1. Open **Visual Studio Code**.
2. Click on the **Extensions** icon on the left sidebar (or press `Ctrl + Shift + X`).
3. Search for and install the following two extensions:
   * **[PlatformIO IDE](https://marketplace.visualstudio.com/items?itemName=platformio.platformio-ide)** (Handles building and compiling C++ code for ESP32)
   * **[Wokwi Simulator](https://marketplace.visualstudio.com/items?itemName=Wokwi.wokwi-vscode)** (Simulates the ESP32 hardware and screen)

---

### 3. Open the Extracted Project
1. In VS Code, go to **File** $\rightarrow$ **Open Folder...** (or press `Ctrl + K, Ctrl + O`).
2. Navigate to the folder you extracted in **Step 1**.
3. Select the root folder (the folder containing `platformio.ini` and `wokwi.toml`) and click **Select Folder**.
4. If prompted with *"Do you trust the authors of the files in this folder?"*, click **Yes, I trust the authors**.

---

### 4. Build and Run the Project

#### Option A: Running in Wokwi Simulator (Virtual Hardware)
1. Open the **`diagram.json`** file from the left Explorer pane.
2. Press `Ctrl + Shift + P` (or `Cmd + Shift + P` on Mac) to open the VS Code Command Palette.
3. Type **`Wokwi: Start Simulator`** and press **Enter**.
4. The simulation window will open directly in VS Code, displaying the ILI9341 screen and animated buttons.

# Buzzer audio in vs Code:
* The buzzer noise when running the Wokwi simulator inside the VS Code . The vscode mutes the sounfd from the wokwi simulator so you can't hear it. 
* If you want to listen to the sound effects and music, open the diagram.json file online directly at **[Wokwi.com](https://wokwi.com)**.

---

#  Battery Level Simulation (Potentiometer Knob):
*  In the simulator, the battery level is simulated using a potentiometer (rotary knob).
* How to test battery levels: While the simulation is running, click and drag the knob clockwise on the potentiometer in the simulator window to increase or decrease the voltage.
# schematics:
<img width="1127" height="793" alt="image" src="https://github.com/user-attachments/assets/10bac07b-6264-4ffc-a163-201cada7d89c" />
## pcb files:
<img width="740" height="655" alt="image" src="https://github.com/user-attachments/assets/d298d322-bd23-4a5e-ab36-206e456b0f31" />
## cad case:
<img width="816" height="727" alt="image" src="https://github.com/user-attachments/assets/2ad9de9d-9f97-4a2e-bed9-9f6a601399b4" />
<img width="896" height="557" alt="image" src="https://github.com/user-attachments/assets/cf67cbe3-e9f6-4047-a0d0-d32c6082a08a" />
