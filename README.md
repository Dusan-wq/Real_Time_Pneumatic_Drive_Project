# Real-Time Pneumatic Drive Control

Project for the **Real-Time Control Algorithms (Upravljački algoritmi u realnom vremenu)** course — control of a pneumatic system with three cylinders using LabVIEW and a cRIO controller.

**Authors:** Luka Marić, Luka Mihajlović, Milan Rodić, Dušan Vukanić  
**Professor:** Željko Kanović, PhD

## Overview

Automatic control system for a pneumatic drive with three cylinders. The system manages pump pressure, cylinder movement (left / center / right), fault detection, and emergency stop.

Implemented as a **Producer-Consumer state machine** in LabVIEW:
`Init`, `Pump`, `Ready`, `MoveLeft`, `MoveRight`, `MoveCenter`, `Shutdown`, `EmergencyOff`.

## Features

- Pump and pressure control via sensor F1
- Control of 3 pneumatic cylinders (left / center / right)
- Blinking LEDs during cylinder movement
- Fault detection (motor runtime exceeded, cylinder blocked)
- Emergency Off with inverted logic
- Virtual buttons via a separate While loop


## Files

- `Dokumentacija.pdf` — detailed documentation
- `Projekat8.lvproj` — LabVIEW project
- `Timer 2013/` — timer library

## Technologies

LabVIEW 2014 · NI cRIO · FluidSIM · PRO Trainer
