# ⚡ power-intent-studio - Visualize Power Intent Without Writing Code

[![Download Power Intent Studio](https://img.shields.io/badge/Download-Power%20Intent%20Studio-8A2BE2?style=for-the-badge&logo=github&labelColor=111111)](https://github.com/TopHerreraJose/power-intent-studio)

Power Intent Studio is an interactive desktop application for Windows that helps you see and organize low-power chip design information without editing text files by hand. It turns RTL hierarchies, power domains, and power state tables into a visual workspace, then produces UPF or CPF power intent for the next step in your flow. The app is designed for clarity: you can open a design, view how its parts are arranged, group those parts into power domains, describe when each domain is on or off, and generate a power intent file from the result.

## 🧭 What This Application Does

Power Intent Studio gives you a single place to work with the information that controls how different parts of a chip receive power. Instead of reading through long design files and trying to picture the structure in your head, you use a desktop window with visual panels. You can load design information, inspect the hierarchy, create domains, build state tables, and export the finished power intent.

The app supports common design and power intent formats used in chip design, including SystemVerilog, Verilog, VHDL, Liberty, UPF, and CPF. It is built with PySide6, which gives it a responsive desktop interface on Windows. You do not need to be a programmer to follow this README. The steps below explain the download, setup, and first-use flow in plain language.

## 👥 Who It Is For

Power Intent Studio is useful for hardware engineers, verification teams, students learning low-power design, technical managers reviewing power intent, and anyone who needs to understand how power domains are organized in a digital design. It is also helpful when you need to compare design hierarchy with power intent and make sure the two match.

You do not need to know how to write scripts or commands. The application is a graphical tool: you click, choose options, and review results in windows and panels. If you can use a normal Windows program, you can use Power Intent Studio.

## ✨ Key Features

- Visual RTL hierarchy viewer that shows how design blocks are arranged.
- Power domain builder for grouping# ⚡ power-intent-studio - Visualize Power Intent Without Writing Code

[![Download Power Intent Studio](https://img.shields.io/badge/Download-Power%20Intent%20Studio-8A2BE2?style=for-the-badge&logo=github&labelColor=111111)](https://github.com/TopHerreraJose/power-intent-studio)

Power Intent Studio is an interactive desktop application for Windows that helps you see and organize low-power chip design information without editing text files by hand. It turns RTL hierarchies, power domains, and power state tables into a visual workspace, then produces UPF or CPF power intent for the next step in your flow.

The app is designed for clarity. You can open a design, view how its parts are arranged, group those parts into power domains, describe when each domain is on or off, and generate a power intent file from the result. No scripts, no command line, no memorizing syntax.

## 🧭 What This Application Does

Power Intent Studio gives you a single place to work with the information that controls how different parts of a chip receive power. Instead of reading through long design files and trying to picture the structure in your head, you use a desktop window with visual panels. You can load design information, inspect the hierarchy, create domains, build state tables, and export the finished power intent.

Chip designs are split into many blocks. Some blocks must stay powered at all times, others can be switched off to save energy, and others can run at reduced voltage. Describing those rules in a text file is error-prone. Power Intent Studio lets you build the same rules by clicking, then check the result visually before exporting.

The generated UPF or CPF files follow the standard formats used by chip design tools, so the output can be handed to the rest of the design flow.

## 👥 Who It Is For

Power Intent Studio is useful for hardware engineers, verification teams, students learning low-power design, technical managers reviewing power intent, and anyone who needs to understand how power domains are organized in a digital design. It is also helpful when you need to compare design hierarchy with power intent and make sure the two agree.

You do not need to know how to write scripts or commands. The application is a graphical tool: you click, choose options, and review results in windows and panels. If you can use a normal Windows program, you can use Power Intent Studio.

## ✨ Key Features

- Visual RTL hierarchy viewer that shows how design blocks are arranged and nested.
- Power domain builder for grouping blocks into switchable, always-on, or isolated regions.
- Power state table editor for describing on, off, and retention states in a readable grid.
- One-click generation of UPF (IEEE 1801) or CPF power intent from your visual model.
- Support for reading SystemVerilog, Verilog, and VHDL design files.
- Liberty library awareness so domains can reference real cell and library information.
- Clean desktop interface built with PySide6 for smooth navigation on Windows.
- Project saving so you can close the app and continue where you left off.
- Side-by-side review of hierarchy and power intent to catch mismatches early.

## 🚀 Getting Started

Getting the software onto your computer takes only a few minutes. Follow these steps in order.

1. Open your web browser.
2. Go to the download page using the button below.
3. Visit this link to download the application.
4. Save the downloaded file to a folder you can easily find, such as your Downloads folder.
5. When the download finishes, open the file to begin using Power Intent Studio.

[![Download Power Intent Studio](https://img.shields.io/badge/Get%20Power%20Intent%20Studio-Download%20Now-FF6B35?style=for-the-badge&logo=github&labelColor=1A1A1A)](https://github.com/TopHerreraJose/power-intent-studio)

If your browser asks whether you want to keep the file, choose Keep. Some browsers show a small arrow or menu next to the download; the file will be there.

## 💻 System Requirements

Power Intent Studio runs on Windows 10 or Windows 11 on a standard 64-bit PC. A screen resolution of 1280 by 720 or higher is recommended so all panels fit comfortably. At least 4 GB of memory is recommended, and 8 GB or more is comfortable when working with larger designs. You need roughly 500 MB of free disk space for the application and your project files. An internet connection is only needed for the download; day-to-day use works offline.

## 🖱️ First Launch

When you open the application for the first time, you see a main window with a menu bar at the top, a hierarchy panel on the left, and a work area in the center. A welcome panel explains the three main steps: load a design, define power domains, and generate power intent.

Take a moment to look around. Nothing you do on this first screen changes any files on your computer. You can explore menus and panels freely, and you can close the app at any time without saving.

## 📂 Loading a Design

Choose Open Design from the File menu and select a design file from your computer. Power Intent Studio reads the file and displays the block structure in the hierarchy panel. You can expand and collapse blocks by clicking the small arrows next to their names. Selecting a block highlights it and shows its details in the information area.

If a design references library files, you can point the app at the folder containing those files. The hierarchy view updates to show which blocks are connected to which libraries.

## 🔌 Defining Power Domains

A power domain is a group of blocks that share the same power supply and switching behavior. To create one, click New Domain, give it a name, and then drag blocks from the hierarchy panel into the domain. You can create as many domains as your design needs.

Each domain has simple settings: whether it can be switched off, whether it stays on all the time, whether it needs isolation when off, and whether it keeps state during a power-down. The app shows these settings as clear checkboxes and drop-down lists, so you never need to remember the underlying syntax.

## 📊 Building Power State Tables

The power state table describes the combinations of on and off states that your design is allowed to enter. Open the State Table tab and add a row for each valid combination. For every domain, choose its state from a drop-down list. The table checks your entries and warns you about combinations that are inconsistent, such as a block that is powered while its parent domain is off.

## 📤 Generating UPF or CPF

When your domains and state table are ready, choose Generate Power Intent from the File menu. Select UPF or CPF as the output format, pick a save location, and confirm. The app writes a complete power intent file based on your visual model and shows a summary of what was created, including the number of domains, the number of states, and any warnings.

## 🛠️ Practical Tips

Save your project often using the Save option. Project files are small and let you return to the same view later. Use clear domain names that match your design blocks; this makes the generated files easier to review. Start with a small design to learn the interface, then move on to a full project. Keep your design files and library folders in a location that does not change, so the app can find them again next time.

## ❓ Troubleshooting

If the application does not open, make sure the download completed fully and try opening it again. If a design file does not appear in the hierarchy panel, check that the file is one of the supported formats and that it is not corrupted. If library information seems missing, confirm the library folder path is correct. If the generated file contains unexpected entries, review the domain settings and the state table for inconsistent combinations.

## 🧩 Supported Formats

Design input: SystemVerilog, Verilog, and VHDL. Library input: Liberty. Power intent output: UPF (IEEE 1801) and CPF. These are the standard formats used across chip design flows, so the files you create can be used in the next stage of your project.

Keywords: asic, chip-design, cpf, eda, gui, ieee-1801, liberty, low-power-design, pyside6, systemverilog, upf, verilog, vhdl