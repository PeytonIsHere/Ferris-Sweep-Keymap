# Ferris Sweep Keymap (Colemak DH)

This is my custom keymap for the Ferris Sweep split keyboard, using the **Colemak DH** layout. It includes multiple layers optimized for me.
Im using a Sea picro controler. I've had a lot of problems with flashing this (ai made this worse)
If you have anything to make this keymap better please fix it, thanks.

## Features
- **Colemak DH** as the base layout
- Just Three layers for navigation, symbols, and function keys

## How to flash an rp2040 board on a split keyboard
### **1. Compile the Keymap**
Run the following command to compile the firmware:
```bash
qmk compile -kb ferris/sweep -km peytonishere -e CONVERT_TO=promicro_rp2040
```

### **2. Flash the Firmware**
Flash the **left half**:
```bash
qmk flash -kb ferris/sweep -km peytonishere -e CONVERT_TO=promicro_rp2040 -bl uf2-split-left
```

Flash the **right half**:
```bash
qmk flash -kb ferris/sweep -km peytonishere -e CONVERT_TO=promicro_rp2040 -bl uf2-split-right
```
