This is my LORA radio controller project! I wanted to make this because I am currently building a drone
that requires a capable LORA radio.
I have posted the Gerber files and BOM so you can produce your own functioning LORA radio controller.
The controller has two joysticks, two switches, and two potentiometers for inputs.  I also added
a buzzer to notify people when events happen, like connecting to a device. 





BUILDING 
To build this PCB, I would recommend ordering the PCB with a stencil because of the small and closely located parts on the board.
This PCB uses parts with pads exposed ONLY on the underside!
The PCB BOM does not include the REQUIRED RYLR998 LORA module; you can buy this on [Amazon](https://www.amazon.com/REYAX-RYLR998-Interface-Antenna-Transceiver/dp/B099RM1XMG/ref=sr_1_1?crid=3UDNJM86BEADO&dib=eyJ2IjoiMSJ9.TrUCyGx0qarh1587JZE8yvvpoC9gwe9bI9YRw3IJh5Zx1KMgEmUzJjvn7MXzx70qEOTY9Fq1M7de8QXRClEF1gXgdkHaO5Cp1hr_cBkrCVVQM3ZOe9HBNgby4LxkEoifRjcGB3QqjgsQhcNnanCQkIOsF3Hd2hs2Dmw3LSlU7O13KyXTs3yf6Vi8z0KqYX-fim7_xzP2ZXnVLrSlw5k8YtSw-LhxjmDXxdbevTJhjuQ.NWGx5ZOZ6Yl5I9t_tEakvIQr32iyknbT6vLo_iMR5xk&dib_tag=se&keywords=rylr998&qid=1781199705&sprefix=RYLR%2Caps%2C197&sr=8-1). 
Place the Lora module in these pins <img width="1047" height="578" alt="image" src="https://github.com/user-attachments/assets/7b2dad99-c150-4dc6-9eec-9693f6c23618" /> with the correct orientation according to the labeled pin on the module.
Here is the BOM, but you can also find the BOM.csv file in the repository:
| Designator | Footprint | Qty | Value | LCSC Part # |
|------------|-----------|-----|-------|-------------|
| BT1 | PinHeader_1x02_P2.54mm_Vertical | 1 | Battery_Cell | |
| C1, C16 | 0402 | 2 | 10uF | |
| C10, C9 | 0603 | 2 | 18pF | |
| C11, C15, C2, C3, C4, C8 | 0402 | 6 | 0.1uF | |
| C12, C6, C7 | 0805 | 3 | 1uF | |
| C13, C14 | 0603 | 2 | 4.7uF | |
| C5 | 0603 | 1 | 10nF | |
| D1, D2 | 0805 | 2 | LED | |
| D3 | 0603 | 1 | LED | |
| D4, D5 | LED_D5.0mm | 2 | LED | |
| F1 | CP_EIA-3528-12_Kemet-T | 1 | 22uF | |
| J1 | SAMESKY_UJ20-C-H-G-SMT-1-P16-TR | 1 | USB-C | |
| J2 | PinHeader_1x05_P2.54mm_Vertical | 1 | Conn_01x05_Socket | |
| J3 | PinHeader_1x05_P2.54mm_Vertical | 1 | Conn_01x05_Pin | |
| J4 | PinHeader_1x03_P2.54mm_Vertical | 1 | Conn_01x03_Pin | |
| L1 | 0603 | 1 | 120R | |
| LS1 | SPKR_PKM22EPPH4001-B0 | 1 | PKM22EPPH4001-B0 | |
| Q1, Q2 | SOT-23 | 2 | BSS806N | |
| R1 | 0603 | 1 | 39 | |
| R10, R11 | 0402 | 2 | 1k | |
| R12 | 0603 | 1 | 49.9K | |
| R13 | 0402 | 1 | 200k | |
| R14 | 0402 | 1 | 1.13K | |
| R15, R16 | POT_P120PK-x25_TTE | 2 | P120PK | |
| R17, R18, R19, R6 | 0402 | 4 | 10k | |
| R2, R3 | 0402 | 2 | 5.1k | |
| R20, R21 | 1206 | 2 | 5M | |
| R22, R23, R8 | 0603 | 3 | 330 | |
| R4, R5 | 0402 | 2 | 22 | |
| R7 | 0603 | 1 | 2.2k | |
| R9 | 0402 | 1 | 1.18k | |
| S1, S2 | SW_200MSP1T2B4M2QE | 2 | 200MSP1T2B4M2QE | |
| U1 | UFQFPN-48_7X7X0P55MM | 1 | STM32F103CBU6 | |
| U2 | SON50P150X150X80-6N | 1 | BQ29700DSER | |
| U3, U4 | XDCR_COM-09032 | 2 | Joy_Stick | |
| U5 | SOT-23-6 | 1 | USBLC6-2SC6 | |
| U6 | SOT-223-3_TabPin2 | 1 | AMS1117-3.3 | |
| U7 | QFN50P300X300X100-17N | 1 | BQ24072TRGTR | |
| Y1 | XTAL_ECS-240-8-33-AGN-TR | 1 | ECS-80-12-33-JGN-TR | |
