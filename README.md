# ESP32 Pokedex Handheld Device

A retro Pokédex handheld built using an **ESP32 DevKit V1**, a **2.8" ILI9341 SPI TFT LCD**, directional buttons, a microSD card module, and a passive buzzer.

This project features a custom Pokédex UI with a Pokémon entry browser, a *"Who's That Pokémon?"* mini-game, real-time battery voltage monitoring, dual-core audio processing, and Wokwi simulation support.

---

## Features

* **Pokémon Browser:** View detailed entry pages including ID, name, type-colored badges, 16-bit RGB sprite bitmaps, movesets, and descriptive lore.
* **"Who's That Pokémon?" Mini-Game:** Guess the silhouette of random Pokémon with multiple-choice options and instant reveal animations.
* **Settings & Power Management:** Toggle sound effects, or trigger an ultra-low-power Deep Sleep mode using RTC wake-up configurations (`ext0` pin wake-up via the START button).
* **Battery Gauge:** Live battery percentage and graphical bar visualizer powered by ADC readings from GPIO36 (VP).
* **Dual-Core Audio Engine:** Background music runs on **Core 0** via FreeRTOS tasks (`xTaskCreatePinnedToCore`) to ensure smooth, lag-free UI rendering on **Core 1**.
* **Flexible Display Options:** Supports 16-bit RGB565 bitmap array drawing from memory or fast 24-bit BMP image reading directly from a MicroSD card.

---

## Hardware Requirements

| Component | Quantity | Details / Recommendation |
| :--- | :---: | :--- |
| **Microcontroller** | 1 | ESP32 DevKit V1 (30-pin / 38-pin) |
| **Display** | 1 | 2.8" ILI9341 SPI TFT LCD (240x320 resolution) |
| **Storage** | 1 | MicroSD Card SPI Module |
| **Input** | 8 | Tactile Push Buttons (D-Pad, A, B, Select, Start) |
| **Audio** | 1 | 5V / 3.3V Passive Buzzer |
| **Battery Sense** | 1 | Potentiometer (Wokwi) or Voltage Divider (LiPo Battery) |

---
---
## Tech Stack

### Software & Firmware:Wokwi online simulator.
### Hardware: Kicad,Fusion 360.
---

## 🤖 AI Usage Disclosure

> 🧠 **Minimal & Human-Led Development:**
> * **Software Debugging & Logic:** AI was used sparingly—primarily for diagnosing C++ type mismatch compiler errors and validating array index alignments.
> * **Hardware Layout & UI:** The physical pin layout, menu navigation state machines, pixel-art drawing logic, and FreeRTOS task assignment were designed manually to ensure optimal hardware performance and authentic retro aesthetics.

---
## How to Open and Use the ZIP Project in VS Code

Follow these steps to extract, open, and run the project inside Visual Studio Code using PlatformIO and the Wokwi Simulator.
The zip file:
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

#### Option B: Uploading to Real ESP32 Hardware
1. Connect your ESP32 board to your computer via a USB cable.
2. Click the **PlatformIO** alien icon on the left toolbar.
3. Under the **Project Tasks** section, expand `env:esp32dev` (or click the bottom status bar icons):
   * Click **Build** (`✓`) to compile the code.
   * Click **Upload** (`→`) to flash the firmware onto your physical ESP32.
   * Click **Serial Monitor** (`plug icon`) to view debugging terminal outputs at `115200` baud rate.

>  **Buzzer Audio in VS Code:**
> The **passive buzzer audio will NOT play** when running the Wokwi simulator inside the **VS Code Extension**. This is a known technical limitation of the local VS Code extension environment. 
> * If you want to **listen to the sound effects and music**, open the `diagram.json` file online directly at **[Wokwi.com](https://wokwi.com)**.

---

>  **Battery Level Simulation (Potentiometer Knob):**
> * In the simulator, the battery level is simulated using a **potentiometer (rotary knob)** wired to GPIO 36 (VP).
> * **How to test battery levels:** While the simulation is running, **click and drag the knob** on the potentiometer in the simulator window to increase or decrease the voltage.
> * Navigating to **Menu → Battery** will instantly reflect the real-time battery percentage and bar graph as you turn the knob!
# schematics:
<img width="1127" height="793" alt="image" src="https://github.com/user-attachments/assets/10bac07b-6264-4ffc-a163-201cada7d89c" />
## pcb files:
<img width="740" height="655" alt="image" src="https://github.com/user-attachments/assets/d298d322-bd23-4a5e-ab36-206e456b0f31" />
## cad case:
<img width="816" height="727" alt="image" src="https://github.com/user-attachments/assets/2ad9de9d-9f97-4a2e-bed9-9f6a601399b4" />
<img width="896" height="557" alt="image" src="https://github.com/user-attachments/assets/cf67cbe3-e9f6-4047-a0d0-d32c6082a08a" />
