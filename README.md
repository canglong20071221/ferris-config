# Ferris Sweep: Vertical Combo Layout (QWERTY)

This is a custom ZMK configuration for the **Ferris Sweep** (34-key split keyboard).

It features a standard **QWERTY** base, **Home Row Mods**, and a unique **"Vertical Barring"** system that replaces the number row. By pressing the gap between two vertical keys, you trigger numbers and symbols, eliminating the need to reach for a dedicated number layer.

## 🎹 Hardware Recommendations (Critical)

To make the "Vertical Barring" combos comfortable and consistent, specific hardware is highly recommended.

* **Switches: 20g - 25g Linear (e.g., gChoc, Purpz)**
    * **Why?** This layout relies on "barring"—using one finger to press two keys (one above the other) simultaneously. Heavier switches (50g+) make this difficult and fatiguing. Ultra-light switches allow you to actuate the combo effortlessly by pressing the gap between the keycaps.
* **Keycaps: Low Profile (MBK, MCC, or CFX)**
    * **Why?** Flat, low-profile keycaps have smaller gaps between rows, making it easier to bridge two keys with a single finger press.

## 🗺️ Base Layer (QWERTY)

The default layer is standard **QWERTY** with **Home Row Mods** for seamless access to Shift, Ctrl, Alt, and GUI.

|   |   |   |   |   |   |   |   |   |   |
|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
| Q | W | E | R | T | Y | U | I | O | P |
| **A**<br>^(Ctrl)^ | **S**<br>^(Alt)^ | D | **F**<br>^(GUI)^ | G | H | **J**<br>^(GUI)^ | K | **L**<br>^(Alt)^ | **;**<br>^(Ctrl)^ |
| Z | X | C | V | B | N | M | , | . | / |
|   |   | **Nav**<br>^(Delete)^ | **Shift**<br>^(Tab)^ |   | **Shift**<br>^(Space)^ | **Func**<br>^(Bksp)^ |   |   |

* **Thumbs:**
    * **Left Inner:** Tap for `Delete` / Hold for **Navigation Layer**.
    * **Left Outer:** Tap for `Tab` / Hold for **Shift**.
    * **Right Inner:** Tap for `Space` / Hold for **Shift**.
    * **Right Outer:** Tap for `Backspace` / Hold for **Function Layer**.

## 🔢 Vertical Barring (Combos)

Instead of a number layer, this layout uses **Combos**.
**Press the gap between the Top and Middle row keys simultaneously.**

### Numbers (Row 1 + Row 2)
**Press gap between Top & Home Row keys:**

| Left Hand | Result | Right Hand | Result |
| :--- | :--- | :--- | :--- |
| **Q + A** | **1** | **Y + H** | **6** |
| **W + S** | **2** | **U + J** | **7** |
| **E + D** | **3** | **I + K** | **8** |
| **R + F** | **4** | **O + L** | **9** |
| **T + G** | **5** | **P + ;** | **0** |

### Symbols (Row 2 + Row 3)
**Press gap between Home & Bottom Row keys:**

| Left Hand | Result | Right Hand | Result |
| :--- | :--- | :--- | :--- |
| **A + Z** | **`** (Grave) | **H + N** | **Home** |
| **S + X** | **'** (Apostrophe) | **J + M** | **[** (L Bracket) |
| **D + C** | **-** (Minus) | **K + ,** | **]** (R Bracket) |
| **F + V** | **=** (Equal) | **L + .** | **\\** (Backslash) |
| **G + B** | **Esc** | **; + /** | **End** |

## 🔽 Navigation Layer (Hold Left Thumb)

Designed for one-handed navigation using the Right Hand (VIM/HJKL style).

* **Right Hand:**
    * **Left / Down / Up / Right** (on Home Position)
    * **PgUp / PgDn** (Top Row)
    * **Enter** (Pinky)
* **Left Hand:**
    * Modifiers (Ctrl, Alt, GUI) are available on the home row to combine with arrows (e.g., `Ctrl` + `Left` to jump words).

## 🔧 Function Layer (Hold Right Thumb)

Standard F-Keys and System controls.

* **Left Hand:** F1 - F10.
* **Right Hand:** F11, F12, Caps Word, PrtSc.

## ⚙️ Custom / Tri-Layer (Hold Both Thumbs)

Press both thumb layer keys to access hardware controls.

* **Bluetooth:** Select Profiles (1-4) or Clear Connection.
* **Media:** Volume Up/Down, Mute, Brightness, Play/Pause.

## 🔋 Power Management

* **Physical Switch:** Use the dedicated slide switch to turn the keyboard off for travel.
* **Deep Sleep:** The keyboard enters deep sleep after **1 hour** of inactivity to save battery. Press any key to wake it.

---

### 🛠️ Flashing Instructions
1.  Download the `firmware.zip` from the latest GitHub Action run.
2.  Extract the `.uf2` file.
3.  Connect the keyboard via USB and double-tap the reset button to enter Bootloader mode.
4.  Drag and drop the `.uf2` file onto the `NICE_NANO` drive.
