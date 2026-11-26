# Capstone Project: Make the Computer Draw a Box
**Nand to Tetris – I (ETCCNT301)**  
School of Engineering & Technology, K.R. Mangalam University  

**Student Name:** Ankit Kumar  
**Roll Number:** 2501010007  
**Personal Number K:** 07  

---

## Directory Contents
- `Part_A_Hardware/`: CPU, Memory, and Computer HDL implementations plus official `.tst`, `.cmp`, and `.out` files.
- `Part_B_Assembler/`: Python assembler, `.asm` practice programs, assembled `.hack` outputs, and `symbols.txt`.
- `Part_C_Box/`: `Box.asm`, `Box.hack`, browser emulator, and Box test/generation scripts.
- `Documentation/`: Project report, README, and viva preparation notes.
- `Assets/`: Generated box and hardware-test screenshots.

---

## How to Run the Assembler
To assemble `Box.asm` into `Box.hack`:
```bash
python Capstone/Part_B_Assembler/assembler.py Capstone/Part_C_Box/Box.asm
```

To test on other programs:
```bash
python Capstone/Part_B_Assembler/assembler.py Capstone/Part_B_Assembler/Add.asm
python Capstone/Part_B_Assembler/assembler.py Capstone/Part_B_Assembler/Max.asm
```

To run the Box program checks:
```bash
python Capstone/Part_C_Box/run_test.py
```

## Run the Hardware Simulator tests
Open the Nand2Tetris `HardwareSimulator.bat`, load each `.tst` script, and run it. Before running `Memory.tst`, set **View** to **Screen**. When prompted, click the Keyboard icon and hold uppercase `K` until the script continues. Confirm the final comparison succeeds.

---

To regenerate the two PNG files in this folder:
```bash
python Capstone/Part_C_Box/generate_screenshots.py
python Capstone/Part_C_Box/generate_test_screenshots.py
```

## How to Run in CPU Emulator
1. Open the Nand to Tetris `CPUEmulator.bat`.
2. Load Program: select `Box.hack`.
3. Set Animation to `Program & Data` or `No display` (Fast).
4. Click `Run`.
5. Focus the emulator and hold down any keyboard key -> solid black box appears at Row 7.
6. Release the key -> the box clears immediately back to white.
