# Dean_Snyder_Projects_Portfolio
Github repository containing some of my personal and course projects in embedded systems, software, and hardware.

1. Verilog Processor
Built as part of Purdue's ECE 437 processor design course, this project documents the full evolution of a RISC-V processor implementation in SystemVerilog — from a single-cycle design, through a pipelined architecture, then adding instruction and data caches, and finally scaling to a multicore system. Each stage introduced new hardware design challenges around performance, hazard handling, cache coherence, and arbitration. RTL diagrams are included for each iteration to illustrate the architectural progression.

2. OOP C++ Chess Game
Originally built for a C++ object-oriented programming course to demonstrate class inheritance, this project grew into a fully featured chess engine. The course required only a minimal implementation, so the full ruleset was added independently — including knights, queens, pawn promotion, en passant, and castling — along with a terminal UI, a scoring system, and save/load functionality. The architecture uses an abstract base ChessPiece class that piece-type subclasses inherit from, with the board represented as a 2D vector object.

3. Embedded ESP32 Nintendo Switch
A handheld gaming console built to mimic the form factor and feel of a Nintendo Switch, developed out of interest in embedded systems and consumer electronics. The hardware includes dual joysticks, four buttons, a 4" touchscreen, an SD card reader, a speaker, and a tilt switch. It was first prototyped on a breadboard, then moved to a custom PCB with female connectors for each component module, with a 3D-printed case planned as the final step.

4. Embedded ESP32 Mini Computer
A self-contained handheld computer built around the ESP32, designed to replicate the core experience of a desktop computer in a pocket-sized device. Input is handled through a physical keypad (keyboard) and joystick (mouse), with a display, speaker, tilt sensor, ADC, IR remote receiver, and temperature sensor rounding out the hardware. The device runs MiniOS, a custom-coded launcher with 60+ apps and games. Like the Switch console, it was first prototyped on a breadboard and later moved to a custom PCB.

5. Facial Recognition Program
Developed as a component of a larger YOLO-based computer vision system used for artistic dance and theatre applications, where body keypoints drove real-time visual effects. The system needed to consistently distinguish between multiple people in frame, so a 2D facial recognition pipeline was built to run concurrently. MTCNN detects faces and assigns each person a tracked ID, InceptionResnetV1 converts face crops into feature vectors, and cosine similarity is used to match faces across frames by comparing against a rolling buffer of five stored images per identity.

6. DIY Programmable Watch
Built out of a personal interest in mechanical and luxury watches, this project is a wearable device centered on an RP2040 with a circular LCD display, housed in a custom CAD-designed case worn on a NATO strap. The dial is fully software-defined, and five custom watch face designs have been implemented — inspired by the Omega Speedmaster, Rolex Pepsi GMT, F.P. Journe Octa Lune, Ressence Type series, and H. Moser & Cie Endeavour. Rendering techniques like scanline clipping are used for complex dial elements such as moon phase sub-dials.

7. CadCode
Developed during an engineering internship at Logemann Brothers Co., CadCode is a Python tool that parses technical manufacturing drawings and automatically generates STL files ready for CNC machining. It was built to reduce manual CAD modeling time in the production workflow. The tool first extracts part dimensions from schematic files, then procedurally constructs and exports the 3D geometry. It was validated primarily on flat plates with hole patterns, corrugated plates, and cylindrical parts.

8. Rain-Sensing Windshield Wipers
A senior design project delivering a fully autonomous wiper control system that senses rain intensity and drives a wiper motor accordingly. The system is split across five subsystems: an IR-based rain sensor (measuring voltage drop across a phototransistor as water refracts the IR beam), a moisture and vibration sensor array, a decision algorithm that maps sensor readings to wiper speed in auto mode, a touchscreen UI with manual override controls, and a CAN bus communication link to a mock car ECU board. The two custom PCBs communicate over CAN with MCP2551 transceivers to simulate integration with a real vehicle — avoiding the complexity of proprietary OEM CAN protocols. A plexiglass windshield panel, motor mount, and PCB enclosures were all custom CAD-designed and 3D-printed for the demonstration.
