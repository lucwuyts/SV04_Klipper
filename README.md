# Sovol SV04 – Klipper & OrcaSlicer Configuration

This repository contains my current Klipper configuration and OrcaSlicer profiles for the Sovol SV04.

## 📦 Overview

- Klipper firmware configuration
- Custom macros and tuning
- OrcaSlicer printer, filament, and print profiles

## 🙏 Credits

This setup is based on the excellent work from:  
https://github.com/Bully85/Sovol-SV04-Klipper

## 📁 Repository Structure
/config/ → Klipper configuration files
/orca/ → OrcaSlicer profiles


## 🔧 Klipper Configuration

The `config` folder contains all files used by Klipper on the printer, including:

- `printer.cfg` – main configuration file  
- macro files  
- additional includes and tuning parameters  

## 🧩 OrcaSlicer Profiles

The `orca` folder contains:

- printer profiles  
- filament settings  
- print profiles  

These can be imported into OrcaSlicer.

## ⚠️ Notes

- Runtime data such as logs, G-code files, and backups are intentionally excluded.  
- This repository is intended as a clean backup of configuration only.

## 🔄 Usage

Clone this repository to your Klipper configuration directory or use it as a backup/reference.



---

## 🔧 Installation Guide

### 1. Install Klipper

Install Klipper on your device (e.g. Raspberry Pi or BTT Pad) using your preferred method:

- KIAUH (recommended)
- Manual installation

Make sure Klipper, Moonraker and a web interface (Mainsail/Fluidd) are installed.

---

### 2. Backup existing config (IMPORTANT)

```bash
cp -r ~/printer_data/config ~/printer_data/config_backup

---

### 3. Clone this repository

Go to your printer data folder:

```bash
cd ~/printer_data

Clone the repo:
git clone https://github.com/<your-repo>.git

--- 

### 4. Copy configuration files

Copy the Klipper config:
cp -r <repo-folder>/config/* ~/printer_data/config/

--- 

### 5. Restart Klipper

Restart the firmware:
sudo service klipper restart

Or restart via your web interface (Mainsail / Fluidd).

--- 

### 6. Verify configuration

Check for errors in the Klipper console

Run a RESTART command if needed

Verify homing and movement before printing
