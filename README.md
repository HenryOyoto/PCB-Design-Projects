# PCB Design Projects

A collection of PCB design work — schematics, layouts, 3D board renders, and the
supporting documentation that goes with them. These are boards I designed for my own
projects, reviewed carefully, and — for the ones marked as fabricated — prepared,
ordered, and tested.

## What is in this repository

Each project folder contains the schematic, the layout, a 3D render or board photo, a
Bill of Materials, and a short write-up of the design intent, stack-up, and any notes
from the design review.

Typical contents per project:

- Schematic files
- PCB layout files
- 3D board renders and board photos (where fabricated)
- Bill of Materials (BOM)
- Fabrication notes (layer count, thickness, surface finish, design rules)
- A short design write-up

## Tools used

- KiCad 10 — used for the drone PCB
- KiCad 9 — used for the autonomous robot PCB
- KiCad 7 — used for the smart parking project PCB
- EasyEDA, Proteus, Eagle, Altium Designer — used for other and earlier work

The KiCad version used for each project is stated in that project's README, because
project files are not always forward-compatible between major KiCad versions.

## Projects

### 1. Drone PCB (KiCad 10)

Flight-controller board designed for a small drone build. Contains the microcontroller,
sensor connections, motor outputs, power regulation, and the connectors needed to
interface with the rest of the drone.

**Design highlights**

- Designed in KiCad 10
- Multi-layer board with a dedicated ground plane
- Power regulation for the flight controller and peripherals
- Motor output headers and sensor input headers
- Component layout chosen to keep signal paths short

**Status**

Designed and reviewed. Add fabrication notes and test results once the board has been
ordered and assembled.

**Folder contents**

- `schematic/` — KiCad schematic
- `pcb/` — KiCad layout
- `gerbers/` — Fabrication outputs (where shareable)
- `images/` — 3D render and photos
- `BOM.xlsx` — Bill of Materials
- `README.md` — Detailed write-up for this board

---

### 2. Autonomous Robot PCB (KiCad 9)

Control board designed for the autonomous 4-wheel robot project. Contains the ESP32,
motor driver connections, ultrasonic sensor headers, and power routing for the motors
and logic.

**Design highlights**

- Designed in KiCad 9
- Two-layer board with a ground pour
- Clear separation between motor power and logic power
- Headers for the ultrasonic sensors and motor driver
- Silkscreen labels for every connector

**Status**

Fabricated and populated. Board is used in the working autonomous robot prototype.

**Folder contents**

- `schematic/` — KiCad schematic
- `pcb/` — KiCad layout
- `gerbers/` — Fabrication outputs
- `images/` — 3D render and board photos
- `BOM.xlsx` — Bill of Materials
- `README.md` — Detailed write-up for this board

**Related project**

See the Arduino-IoT-and-Embedded-Projects repository, Autonomous 4-Wheel Robot.

---

### 3. Smart Parking Project PCB (KiCad 7)

Control board for the smart parking and management system. Handles the ESP32, infrared
sensor inputs, servo motor outputs, and the power and communication wiring for the
whole parking setup.

**Design highlights**

- Designed in KiCad 7
- Two-layer board
- Inputs routed for multiple infrared sensors
- Servo motor outputs with proper decoupling
- Separate power rails for the servos and the logic

**Status**

Fabricated and populated. Board is used in the working smart parking prototype.

**Folder contents**

- `schematic/` — KiCad schematic
- `pcb/` — KiCad layout
- `gerbers/` — Fabrication outputs
- `images/` — 3D render and board photos
- `BOM.xlsx` — Bill of Materials
- `README.md` — Detailed write-up for this board

**Related project**

See the Arduino-IoT-and-Embedded-Projects repository, Smart Parking and Management
System with M-Pesa Integration.

---

## How to view a design

- Install the matching EDA tool for the project. KiCad is free and covers most of the
  work here.
- Open the schematic first, then the layout.
- Gerber files, where included, can be viewed with any free Gerber viewer, including the
  one built into KiCad.

## Design notes

- All boards are designed with manufacturability in mind — sensible trace widths,
  clearances, silkscreen clarity, and fiducials where needed.
- Layer stack-ups and design rules are stated per project.
- Where a board has been fabricated and tested, this is noted in the project README
  along with any revisions.

## About

Designed and maintained by Henry Oyoto — Electronics and Computer Engineer working in
PCB design, Python programming, and technical documentation.

- GitHub: https://github.com/HenryOyoto
- LinkedIn: https://www.linkedin.com/in/henryoyoto
- Email: oyotohenry2021@gmail.com

## License

Design files are shared for reference and learning. Please credit the original work if
you reuse any part of a design. Where a specific project carries a different licence,
it is stated in that project's README.
