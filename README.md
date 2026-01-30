# Python Continuous General DAQ (8 channels) — EXE Version

A general-purpose data acquisition (DAQ) program designed to read **analog voltage** data from an NI DAQ device, display it on a **real-time graph**, and record acquired data to a **CSV file**.

This repository contains the **Windows executable (.EXE)** version of the program.

---

## What the program does

- Reads analog voltage data continuously from an NI DAQ device
- Displays live data on a real-time graph
- Lets you initialise/configure channels (including scale and offset)
- Records data to a CSV file when you press **Record**
- Saves results into a **Results** folder

---

## Requirements

- Windows PC
- Valid Python install
- A compatible NI DAQ device (e.g., NI USB‑6009 / similar)
- NI software installed:
  - **NI‑DAQmx**
  - **NI MAX** (Measurement & Automation Explorer)

**Install links**
- NI‑DAQmx: https://www.ni.com/en/support/downloads/drivers/download.ni-daq-mx.html
- NI MAX: https://www.ni.com/en/support/downloads/drivers/download.system-configuration.html
- Python: https://www.python.org/downloads/ 

---

## How to run the EXE

1. Open the program folder (e.g., **General DAQ EXE 2023 Version 1**)
2. Run:
   - `DAQ_Main.exe`

<img alt="image" src="https://github.com/user-attachments/assets/473c04ec-031d-4b74-8427-ea0cb742807e" />

---

## How to use (typical workflow)

### 1) File name (optional)
If you want to define your own output file name, enter it in **File Name** and press **OK**.
- The program saves files as: **your defined name + date & time.csv**
- If you leave this blank, a default name is used (e.g., **Experiment Result + date & time.csv**)

<img alt="image" src="https://github.com/user-attachments/assets/5a2cc78e-f1f7-45e5-90d7-5bdc8033939d" />

---

### 2) Confirm the NI device name (first time setup)
If your PC connects to the NI device for the first time, the device name is often `Dev1`.

To confirm:
1. Open **NI MAX**
2. Go to **Devices and Interfaces**
3. Find your connected NI device and note its device name (e.g., `Dev1`)

<img alt="image" src="https://github.com/user-attachments/assets/7597f7b1-374a-4eee-833c-5ee6ed401627" />

---

### 3) Choose sample rate and configure channels
1. Choose the **Sample Rate**
2. Click **Initialise New Channels**
3. In the channel configuration window, for each channel:
   - Enter **Channel Name**
   - Enter **Scale**
   - Enter **Offset**
   - Tick **Select Channel**
4. Click **OK** when finished

<img alt="image" src="https://github.com/user-attachments/assets/0f101bee-d06d-4112-8a10-cad7f42f4cca" />

---

### 4) Start acquisition
Click **Start** to begin data acquisition and live plotting.

<img alt="image" src="https://github.com/user-attachments/assets/146a1aaa-a234-448d-b7ec-d80962345ee9" />

---

### 5) Recording data (two modes)
You can record at any point while the program is running by clicking **Record**.

#### Mode A — Record until you stop
- Leave **Use Record Time** unticked
- Press **Record**
- Data will save continuously until you press **Stop**

#### Mode B — Record for a fixed duration
- Enter a value in **Record Time (s)**
- Tick **Use Record Time**
- Press **Record**
- Data will record for the specified number of seconds

Recorded files are saved as **CSV** in the **Results** folder.

<img alt="image" src="https://github.com/user-attachments/assets/5fcedd2c-6e18-4a0e-aeee-3d1ece7fcf8b" />

---

### 6) Stop / run again
Press **Stop** to stop acquisition.

If you want to run again, you can start again from the sample rate step.  
You can also skip channel setup by selecting **Use Previous Configured Channels** instead of **Initialise New Channels**.

<img alt="image" src="https://github.com/user-attachments/assets/b6a0f7b9-60bb-4afd-bd5e-f9324771098b" />

---

## Output files

- Output format: **CSV**
- Location: **Results** folder
- File name: **your defined name + date/time**, or **default name + date/time**

---

## Support / contact

If you need help setting this up, or want to adapt it for a specific experiment, contact the **Electronics & Software Labs** team.
