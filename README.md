# TwinCAT 3 Logic & HMI Visualization

**Overview**
This project demonstrates foundational PLC logic and human-machine interface (HMI) integration using Beckhoff TwinCAT 3. It utilizes Structured Text (ST) to control visualization elements based on specific analog thresholds.

**Technical Environment**
* **Platform:** Beckhoff TwinCAT 3
* **Language:** Structured Text (ST)
* **Components:** Integrated PLC HMI, Virtual Meter, Rocker Switches, Indicator Lamps

**System Logic**
The system evaluates an incoming integer (`iNumber`) driven by an HMI meter and maps it to four distinct operational states using consecutive `IF/ELSIF` conditions:
* `0 to 8000`: Activates Lamp 1
* `8001 to 16000`: Activates Lamp 2
* `16001 to 24000`: Activates Lamp 3
* `> 24000`: Fallback state activating Lamp 4
