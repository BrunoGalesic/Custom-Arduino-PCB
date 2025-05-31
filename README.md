Custom Arduino UNO-Style Board

This project is a custom-designed Arduino UNO-style board, created with KiCad 8.0, focusing on improved RF characteristics and robust performance. It features a 4-layer PCB design with enhanced power and ground integrity, additional user controls, and thoughtful RF/EMI protections.


 Features:
 
 4-layer PCB with wider power and ground traces for reduced resistance and improved signal integrity.
 
Increased via count on tracks to enhance current capacity and minimize impedance.

Polyfuse for overcurrent protection—resistance increases with temperature rise to protect circuits.

Varistor for surge voltage protection—acts as an insulator under normal conditions and conducts to ground when voltage spikes occur.

Ferrite bead filters (BLM21) to block high-frequency noise while passing low-frequency signals.

USB port shield to mitigate EMI, acting like a Faraday cage connected to ground.

ATmega16U2-MU microcontroller for USB-to-serial conversion, enabling USB communication.

16 MHz external crystal oscillator connected via capacitors for stable clock signals.

4 pushbutton switches and a 7-segment display connected via an I2C port expander for expanded user interaction.


 Design Considerations:
 
 Emphasis on RF performance and signal integrity with multi-layer routing and shielding.
 
Thoughtful placement of components to reduce noise and EMI interference.

Added hardware elements such as TVS diodes for ESD protection on sensitive lines (like RESET).

Designed with educational intent—to explore PCB design, RF characteristics, and protection mechanisms.



 Learning Outcomes:

 The polyfuse: how it increases resistance with temperature due to excessive current.
 
The varistor: how it remains non-conductive at normal voltages and conducts during surges to ground.

The ferrite beads (BLM21): low impedance at low frequencies, high impedance at high frequencies, acting as filters.

USB shielding: how the shield connects to ground and functions like a Faraday cage to prevent EMI.

ATmega16U2-MU: an 8-bit microcontroller used for USB-to-serial conversion.

Crystal oscillators: using piezoelectric effect for stable frequency generation, needing capacitors to ground.

RF oscillators (LC and RC): in radio circuits and microcontrollers.

ICSP (In-Circuit Serial Programming) for direct microcontroller programming.

TXLED and RXLED for visual indication of data transmission and reception.
