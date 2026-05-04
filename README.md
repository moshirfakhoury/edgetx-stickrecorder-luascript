**Important Note:**

Stick Recorder V2 is the latest and improved version of the script. The key change is that switch configuration is no longer stored in Global Variables (GV6 & GV7). Instead, settings are saved to a model-specific config file.

This removes the need to manually set up global variables for each model, frees them up for other uses, and provides a more flexible foundation for future enhancements—allowing additional configuration options to be stored and expanded over time.

**Overview:**

Stick Recorder is an EdgeTX Lua tool designed to record, browse, and replay stick movements from your radio. It provides a visual playback interface that allows pilots to review control inputs in real time, making it ideal for training, debugging, and flight analysis.

The tool reads recorded log files and recreates stick positions on-screen with accurate timing, giving you a clear and intuitive way to analyze how a model was flown. With built-in playback controls and time navigation, you can easily jump to specific moments and study inputs in detail.

**Features:**

- Real-Time Stick Playback:
Visualizes Aileron, Elevator, Throttle, and Rudder movements exactly as recorded.
- Accurate Timing System:
Playback matches the original recording speed using millisecond precision.
- File Browser:
Browse and select log files directly from the radio with filtering options.
- Jump to Time:
Enter a specific time (MM:SS) to instantly jump to any point in the recording.
- Play / Pause Control:
Pause and resume playback smoothly without losing sync.
- Motor / Arm / Flight Mode Display:
Logs and Displays Motor On/Off, Armed/Disarmed and Flight Mode.
- Streaming File Loader:
Loads large log files without freezing the radio UI.
- Clean UI Layout: 
Dual stick visualization with labeled channels and clear navigation.
- Model-Based Configuration:
Uses a per-model config file to store switch assignments and settings, eliminating the need for EdgeTX global variables and simplifying setup.

**Installation:**

- Download the StickRecorder ZIP file 
- Extract the contents of the ZIP file
- Find the last folder named Stick Recorder (folder will contain Stick Recorder.lua, strbg.lua & StickRecorder folder)
- Copy Stick Recorder.lua and paste into your transmitter's /SCRIPTS/TOOLS folder
- Copy StickRecorder folder and paste into your transmitter's /SCRIPTS/TOOLS folder
- Copy strbg.lua and paste into your transmitter's /SCRIPTS/FUNCTIONS folder

**Transmitter Setup:**

- Click on the SYS button
- Navigate to Global Functions
- Add a new Function with the below settings
- Trigger = ON
- Function = Lua Script
- Value = strbg
- Repeat = On
- Enable = True

**Configure the below Steps for each model:**

Optional - if you want Flight Modes to be logged, you need to set them up in the transmitter using the standard Flight Mode menu

<img width="478" height="271" alt="image" src="https://github.com/user-attachments/assets/47850d9c-3790-4c73-b83a-174885937e65" />

<img width="477" height="270" alt="image" src="https://github.com/user-attachments/assets/11f3b616-60fa-4418-bdb6-21e9cd5946d3" />

<img width="477" height="271" alt="image" src="https://github.com/user-attachments/assets/7910c2dd-3ddb-4274-8599-e103d0e1b807" />

<img width="477" height="269" alt="image" src="https://github.com/user-attachments/assets/9f48d255-cc35-45ba-a486-a4d4600d868c" />








