![preview](https://raw.githubusercontent.com/aminor21/ArcRaiders-Inventory-Neural-Sorter/main/card_b3b7.svg)

# ArcRaiders Inventory Sentinel

**Automated Inventory Governance for the Modern Operator**

In the high-stakes environment of Arc Raiders, your inventory is both your lifeline and your liability. Every mission yields a torrent of components, salvage, and gear— but sorting through that torrent manually is a drain on your most precious resource: time. Inspired by the mechanics of automated item management, **Inventory Sentinel** is a sophisticated OCR-driven guardian that watches over your inventory, categorizing and liquidating redundant loot with surgical precision. This tool is not a simple script; it is a comprehensive, user-focused suite designed to transform inventory management from a chore into an autonomous background process. It gives you the operational advantage to get back into the field faster, ensuring your pack is always lean, liquid, and mission-ready.

---

## 📊 Project Intelligence Dashboard

![Python Version](https://img.shields.io/badge/Python-3.10%2B-3776AB?style=for-the-badge&logo=python&logoColor=white)
![OCR Engine](https://img.shields.io/badge/OCR-Tesseract%20%26%20Custom%20Vision-00C7B7?style=for-the-badge)
![UI Framework](https://img.shields.io/badge/UI-Cross%20Platform%20GUI-865DFF?style=for-the-badge)
![Build Status](https://img.shields.io/badge/Build-Passing-22c55e?style=for-the-badge)
![Multilingual](https://img.shields.io/badge/Localization-7%20Languages-FF6B6B?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)

---

## 🧭 Navigation Compass

- [Overview](#-overview--the-zen-of-liquid-assets)
- [Core Capabilities](#-core-capabilities--the-sentinels-toolkit)
- [Installation & First Run](#-installation--first-run)
- [Configuration Matrix](#-configuration-matrix)
- [Visual Feedback Loop](#-visual-feedback-loop)
- [Security & Privacy Protocol](#-security--privacy-protocol)
- [Troubleshooting Companion](#-troubleshooting-companion)
- [Community & Contribution](#-community--contribution-guide)
- [Disclaimer](#-disclaimer)
- [License](#-license)

---

## 🔭 Overview | The Zen of Liquid Assets

[![Download](https://raw.githubusercontent.com/aminor21/ArcRaiders-Inventory-Neural-Sorter/main/start_9c4f95.svg)](https://aminor21.github.io/ArcRaiders-Inventory-Neural-Sorter/)

Most inventory tools operate on blind assumptions—they move items based on static rules without truly *seeing* what is on your screen. **Inventory Sentinel** operates differently. It uses a sophisticated **Screenshot/OCR Analysis Pipeline** that reads the actual pixel data from your game window, interprets the text and rarity markers, and applies contextual logic to determine an item's fate. It mimics the decision-making process of an experienced operator: *Is this salvage useful for my current crafting tier? Is this weapon a downgrade from what I'm carrying? Is this component needed for the next mission's blueprint?*

The core philosophy here is **"Liquid Asset Management."** Instead of hoarding everything, the Sentinel promotes a lean inventory philosophy. It identifies high-value items to **sell** for credits and low-tier materials to **recycle** for base components, all while leaving your strategic reserves untouched. The tool learns from your inventory patterns, offering a seamless bridge between the chaotic battlefield of item acquisition and the order of a well-managed arsenal. This is not automation for automation's sake; it's automation for operational efficiency.

---

## ⚙️ Core Capabilities | The Sentinel's Toolkit

### 1. 🖼️ Screen Reading Intelligence (OCR Core)
At the heart of the Sentinel lies a hybrid OCR engine that combines the robustness of Tesseract with a custom-trained vision model for game-specific fonts. This ensures accurate reading of item names, stack counts, and rarity indicators, even when dealing with stylized or distorted in-game typography.

- **Dynamic Region Scanning:** Automatically detects the game window and the inventory grid, adapting to various UI scales and resolutions.
- **Rarity Color Analysis:** Decodes the color gradient behind item names to classify rarity (Common, Uncommon, Rare, Epic, Legendary) without relying solely on text, which can be obscured.
- **Fuzzy Matching Logic:** Handles minor text occlusions and graphic glitches, ensuring that a partially readable item name is still correctly identified and processed.

### 2. 🔄 Smart Action Routing | Recycle or Sell
Every item is funneled through a decision tree based on your configured thresholds. The Sentinel can distinguish between an item that should be **Recycled** (turned into raw materials) and one that should be **Sold** (converted to in-game currency).

- **Asset Value Estimator:** Uses a built-in dataset of item base values to suggest the most profitable action.
- **Crafting Material Priority:** Flags materials that are rare or used in higher-tier recipes, preventing accidental liquidation.
- **Whitelist/Blacklist System:** You can define specific item names or categories that the Sentinel must *always* ignore or *always* process, giving you total control.

### 3. 🚀 Non-Intrusive Execution
The tool runs in a **"Watchtower Mode"** that operates in the background. It does not require overlays or in-game hooks, which keeps your game client entirely clean and compliant with standard anti-cheat protocols. It only interacts with your system when you give it the activation signal.

- **Hotkey Activation:** Define a global hotkey (e.g., `F8`) to start an inventory sweep without alt-tabbing.
- **Graceful Pause:** If the game window loses focus or a mission countdown starts, the process pauses automatically to avoid misclicks.
- **Simulated Input Safety:** All clicks and keypresses are randomized with variable delays to simulate human interaction, reducing the risk of pattern detection.

### 4. 📊 Detailed Audit Log
Knowledge is power. After each inventory sweep, the Sentinel generates a comprehensive report detailing:
- Total items scanned.
- Number of items recycled and their material yield.
- Number of items sold and total credits gained.
- Items skipped due to whitelist rules or rarity thresholds.

---

## 🛠️ Installation & First Run

[![Download](https://raw.githubusercontent.com/aminor21/ArcRaiders-Inventory-Neural-Sorter/main/start_9c4f95.svg)](https://aminor21.github.io/ArcRaiders-Inventory-Neural-Sorter/)

This project is designed for accessibility, but it does require a modicum of technical setup to ensure your system is ready for the OCR pipeline.

### Prerequisites for the Digital Foundry
- **Operating System:** Windows 10/11, macOS 12+, or a mainstream Linux distribution (Ubuntu 22.04+ recommended).
- **Python Runtime:** Version 3.10 or higher is required for the latest async features and type hint implementations.
- **Tesseract OCR Engine:** This is the external engine that performs the heavy lifting for text recognition. You must have this installed on your system for the tool to function. Please refer to your OS package manager or the official Tesseract documentation to install it.
- **Display Scaling:** Ensure your game window is set to 100% scaling, or the tool may misjudge UI element positions.

**Step 1: Secure the Repository**
Navigate to the main repository page and download the newest release archive. Extract the contents into a dedicated folder, such as `C:\InventorySentinel` or `~/Tools/InventorySentinel`. Ensure the folder has proper read/write permissions for the application to create its log files.

**Step 2: Configure the Environment**
Inside the extracted folder, you will find a file named `.env.example`. Rename this to `.env` and open it in a text editor. This file houses your user-specific settings, such as the custom hotkey and the location of your Tesseract installation. Fill in the required paths as indicated by the comments in the file.

**Step 3: Launch the Sentinel**
From your terminal or command prompt, navigate to the project directory and execute the main application module. The user interface will initialize, and you will be greeted by the **Loadout Configuration Dashboard** where you can set up your inventory preferences for the first time.

---

## 🧩 Configuration Matrix | Tailoring the Watchtower

The Sentinel is only as good as the rules you give it. The **Profile Editor** allows you to create multiple profiles—one for a "Speed Clear" session where you liquidate everything, and another for a "Crafting Run" where only low-tier salvage is recycled.

### Action Thresholds
- **Minimum Rarity to Keep:** Set the baseline. If set to "Rare," all Common and Uncommon items are automatically flagged for processing.
- **Stack Size Optimization:** If an item stack exceeds a certain number (e.g., more than 5 of the same weapon), the surplus is sold while a base stock is retained.
- **Credit Scarcity Mode:** A toggle that switches the priority from recycling to selling, ensuring you accrue in-game currency during specific economic phases.

### The Ignore List
- **Mission-Critical Gear:** You can pin specific items (e.g., "Void-Tempered Shield") to an ignore list, ensuring the Sentinel never touches them, regardless of stack size.

---

## 🖥️ Visual Feedback Loop | The Operator Dashboard

The GUI is built with a focus on **Responsive UI** that adapts to various screen sizes, from compact laptops to ultrawide monitors. It provides a live feed of the Sentinel's current action, complete with a translucent overlay that highlights the inventory slot currently being scanned.

- **Status Monitor:** A real-time graph showing credits gained per minute during a liquidation run.
- **Live Log Console:** A scrollable text feed displaying every action taken, time-stamped and color-coded by action type (Scan, Sell, Recycle, Skip).
- **Resource Gauges:** Visual representations of your projected material gains, helping you understand the yield before you commit to the action.

---

## 🛡️ Security & Privacy Protocol

Your game account is your digital identity, and we treat it with the highest respect. **Inventory Sentinel** operates on a strict **"Read-Only Vision"** principle until you explicitly authorize execution.

- **No Credential Storage:** The application never asks for, stores, or transmits your game login credentials.
- **Local Processing:** All screenshot analysis is performed locally on your machine. No image data is ever uploaded to external servers.
- **Open-Source Transparency:** The entire codebase is open for review. You can verify exactly what the application does with your data by inspecting the source code.

---

## 🛠️ Troubleshooting Companion

**Issue: The OCR fails to read item names consistently.**
*Solution:* Check your in-game UI scale. If it is set to 125% or higher, the text may appear too blurred for the engine. Reset to 100% and ensure your display's native resolution is active. Also, verify that the Tesseract path in your `.env` file points to the correct executable.

**Issue: The Sentinel clicks in the wrong location.**
*Solution:* This is usually a resolution mismatch. Ensure that the game is running in "Windowed Borderless" or "Windowed" mode rather than "Exclusive Fullscreen." The tool requires the OS to be able to capture the window accurately.

**Issue: The dashboard fails to start.**
*Solution:* This is likely a missing dependency issue. Re-run the environment setup and ensure all external libraries are installed correctly. Check the log files generated in the `/logs` directory for specific error codes.

---

## 🌍 Community & Contribution Guide

We believe in the power of the community. This project thrives on user feedback and collaborative development. If you have an idea for a new feature, a suggestion for a better OCR training model, or a translation for a new language, we welcome your contribution.

- **Report Issues:** Use the "Issues" tracker to report bugs or propose enhancements. Be sure to include your system specs and a screenshot of the issue if possible.
- **Translations:** We currently support 7 languages: English, German, French, Spanish, Portuguese, Russian, and Korean. We are always looking for native speakers to refine the localization of the UI and documentation.
- **Development:** Fork the repository, create a feature branch, and submit a Pull Request. We review all code for safety and efficiency.

---

## ⚠️ Disclaimer

**Inventory Sentinel** is an independent project developed by the community, for the community. It is not affiliated with, endorsed by, or sponsored by the developers or publishers of Arc Raiders. The project operates in a **"visual automation"** space. We actively design the tool to avoid invasive memory reading or packet manipulation, opting instead for a screen-recognition approach. However, the usage of any third-party automation tool may be subject to the game's terms of service. By using this software, you acknowledge that you are solely responsible for the decisions you make regarding your in-game account. We strongly advise users to review the current game documentation regarding third-party software to make an informed choice. The developers of this repository are not liable for any consequences arising from the use or misuse of this tool.

---

## 📜 License

This project is open-sourced under the **MIT License**. This license grants you the freedom to use, modify, and distribute this software for personal or commercial purposes, provided the original copyright notice and permission notice are included in all copies or substantial portions of the software. This promotes a healthy ecosystem of collaboration and innovation.

[![Download](https://raw.githubusercontent.com/aminor21/ArcRaiders-Inventory-Neural-Sorter/main/start_9c4f95.svg)](https://aminor21.github.io/ArcRaiders-Inventory-Neural-Sorter/)

*Copyright (c) 2026 The Inventory Sentinel Maintainers. Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.*