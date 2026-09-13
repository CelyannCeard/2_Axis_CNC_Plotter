<h1 align="center">🛠️ 2-Axis CNC Plotter / Braille Machine</h1>

<p align="center">
  <i>A 2-axis cartesian writing machine and braille embosser built from scratch (CAD, 3D printing, and Arduino CNC control).</i>
</p>

<p align="center">
<img width="4096" height="3072" alt="IMG_20250602_205930" src="https://github.com/user-attachments/assets/66bf39e3-76ea-47d1-85ca-fbf79cdd02e2" />
</p>


## 📝 Overview
This project was developed during my 3rd year of engineering studies at Polytech Lyon (Industrial Systems & Robotics). The goal was to design, manufacture, and assemble a 2-axis industrial machine. 

Our team built a versatile **XY Plotter** capable of two main functions:
1.  **2D Drawing:** Accurately drawing complex shapes and texts on paper using a pen.
2.  **Braille Embossing:** (Initial scope) Punching relief dots on thick cardboard to create readable Braille documents for visually impaired individuals.

<br>

## ⚙️ My Contributions
As part of a 4-person team, I was the **Mechanical & Hardware Lead**. My responsibilities included:
*   **Mechanical Design (CAD):** I designed all custom structural parts, brackets, and slider mechanisms using **PTC Creo**. The design was inspired by open-source plotters but fully modeled to fit our specific constraints and budget.
*   **Fabrication:** Preparing the models for 3D printing and manufacturing the parts.
*   **System Assembly:** I led the physical assembly of the aluminum extrusions, linear rails, belts, pulleys, and structural 3D-printed parts.
*   **Hardware Integration:** I was responsible for wiring the electronics, including the NEMA stepper motors, the Arduino Uno, the CNC Shield, and the limit switches.

*(Note: The software integration, GRBL flashing, and G-Code generation were handled by my teammates).*

<p align="center">
<img width="595" height="281" alt="Capture d&#39;écran 2026-09-13 182711" src="https://github.com/user-attachments/assets/29f13a01-2c79-4eba-8a47-192db6321f84" />
</p>

<br>

## 📐 Mechanical Architecture
The machine is based on a standard H-bot / Cartesian XY gantry system.
*   **X & Y Axis:** Driven by **NEMA 17 Stepper Motors** paired with GT2 timing belts and 20-tooth pulleys.
*   **Linear Motion:** Ensured by 6mm precision steel rods and linear ball bearings for high stability and smooth translation.
*   **Z-Axis (Toolhead):** A custom toolhead actuated by a micro-servo motor lifts and lowers the pen/puncher.
*   **Structure:** Built around 20x20mm aluminum extrusions, corner brackets, and 3D-printed mounts (available in this repository).

<p align="center">
<img width="541" height="290" alt="Capture d&#39;écran 2026-09-13 183243" src="https://github.com/user-attachments/assets/e4572227-29f6-4f65-860a-26d4d351d7c2" />
</p>

<br>

## 📁 Repository Structure
This repository contains the mechanical assets of the project:
*   `/CAD_Parts/`: Contains the `.prt` (Creo) and `.stl` files of the 3D printed components (motor brackets, pulley mounts, toolhead slider, etc.).
*   `Pieces_2Axis.xlsx`: The Bill of Materials listing the mechanical and electronic components.

<br>

## 🚀 Results & Challenges
The machine was successfully assembled and the Arduino CNC Shield correctly received and executed G-Code via ChiliPeppr/GRBL. 
One of the main challenges was the structural rigidity required for the Braille function. Braille dots require precise 2.3mm spacing and significant downward force, which pushed the limits of our 3D-printed toolhead rigidity, leading us to focus primarily on the 2D drawing capabilities for the final demonstration.

<p align="center">
<img width="307" height="409" alt="IMG_20250604_133113" src="https://github.com/user-attachments/assets/c5193b6b-37c3-483b-a517-d6a1f370ba3a" />
</p>

---
*Project Team: Celyann CEARD (CAD & Assembly), Julien RIOU (Project Manager), Quentin DREULETTE (Software), Lucas GALMAR.*
