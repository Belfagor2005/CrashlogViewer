# Crashlog Viewer for Enigma2 Image

![Plugin RadioGit](https://github.com/Belfagor2005/CrashlogViewer/blob/main/usr/lib/enigma2/python/Plugins/Extensions/CrashlogViewer/crash.png?raw=true)

[![Python package](https://github.com/Belfagor2005/CrashlogViewer/actions/workflows/pylint.yml/badge.svg)](https://github.com/Belfagor2005/CrashlogViewer/actions/workflows/pylint.yml) 
![Visitors](https://komarev.com/ghpvc/?username=Belfagor2005)


![Screen RadioGit](https://github.com/Belfagor2005/CrashlogViewer/blob/main/screen/screenshot.png?raw=true)

---

## 📄 Description

**CrashLogViewer** is an Enigma2 plugin designed to easily browse, view, and manage system crash log files. It supports multiple screen resolutions (2560x1440, 1920x1080, and lower) with an adaptive, user-friendly interface optimized for remote control navigation.

---

## ✨ Features

* 📁 **Automatic scan** for crash log files in typical system directories.
* 📊 Displays **file name, size, and creation date** for each log.
* 📺 Adaptive UI layout for **multiple screen resolutions**.
* 🎮 Remote control support with **color-coded actions**:

  * 🔴 Red: Exit plugin
  * 🟢 Green: View selected log
  * 🟡 Yellow: Delete selected log
  * 🔵 Blue: Delete all logs
  * ℹ️ Info: Show additional info
* 🗑️ Confirmations before deleting logs to avoid accidental loss.
* 🖥️ Internal log viewer integrated.

---

## 🚀 Installation

1. Copy the plugin folder to:

   ```
   /usr/lib/enigma2/python/Plugins/Extensions/CrashlogViewer/
   ```

2. Restart your Enigma2 device or reload plugins.

3. Launch the plugin from the **Extensions** menu.

---

## 🎯 Usage

* On launch, the plugin scans configured folders for crash logs.
* Navigate the list with remote arrows.
* Press **Green** to open and read a selected log.
* Press **Yellow** to delete the selected log (with confirmation).
* Press **Blue** to delete all logs (with confirmation).
* Press **Red** to exit.
* Press **Info** for more information about the plugin.

---

## 🛠️ Code Structure

* `CrashLogScreen` — Main UI and logic class managing scanning, listing, and user commands.
* Adaptive skin XML layouts tailored for screen resolutions.
* Uses Enigma2 widgets like `List`, `StaticText`, `ActionMap` for UI controls.
* File operations performed via Linux shell commands and Python's `os` and `stat` modules.

---

## ⚙️ Dependencies

* Enigma2 Python environment.
* Enigma2 UI modules (e.g., `Screen`, `List`, `StaticText`).
* Linux filesystem access with proper permissions.

---

## ⚠️ Notes

* The plugin depends on shell commands (`ls`) to list files and get metadata.
* Ensure the plugin has the correct permissions to read and delete log files.
* Intended for Enigma2 satellite receivers; functionality outside this environment is not guaranteed.

---

If you want, I can also help prepare:

* A detailed markdown with screenshots.
* Packaging instructions.
* Translation support.

Just let me know!
