<h1 align="center">🛠️ 2-Axis CNC Plotter / Braille Machine</h1>

<p align="center">
  <i>A 2-axis cartesian writing machine and braille embosser built from scratch (CAD, 3D printing, and Arduino CNC control).</i>
</p>

## 📝 Overview
This project was developed during my 3rd year of engineering studies at Polytech Lyon (Industrial Systems & Robotics)[cite: 6]. The goal was to design, manufacture, and assemble a 2-axis industrial machine[cite: 6]. 

Our team built a versatile **XY Plotter** capable of two main functions:
1.  **2D Drawing:** Accurately drawing complex shapes and texts on paper using a pen[cite: 6].
2.  **Braille Embossing:** (Initial scope) Punching relief dots on thick cardboard to create readable Braille documents for visually impaired individuals[cite: 6].

<br>

## ⚙️ My Contributions
As part of a 4-person team, I was the **Mechanical & Hardware Lead**[cite: 6]. My responsibilities included:
*   **Mechanical Design (CAD):** I designed all custom structural parts, brackets, and slider mechanisms using **PTC Creo**[cite: 6]. The design was inspired by open-source plotters but fully modeled to fit our specific constraints and budget[cite: 6].
*   **Fabrication:** Preparing the models for 3D printing and manufacturing the parts[cite: 6].
*   **System Assembly:** I led the physical assembly of the aluminum extrusions, linear rails, belts, pulleys, and structural 3D-printed parts[cite: 6].
*   **Hardware Integration:** I was responsible for wiring the electronics, including the NEMA stepper motors, the Arduino Uno, the CNC Shield, and the limit switches[cite: 6].

*(Note: The software integration, GRBL flashing, and G-Code generation were handled by my teammates).*[cite: 6]

<br>

## 📐 Mechanical Architecture
The machine is based on a standard H-bot / Cartesian XY gantry system[cite: 6].
*   **X & Y Axis:** Driven by **NEMA 17 Stepper Motors** paired with GT2 timing belts and 20-tooth pulleys[cite: 6].
*   **Linear Motion:** Ensured by 6mm precision steel rods and linear ball bearings for high stability and smooth translation[cite: 6].
*   **Z-Axis (Toolhead):** A custom toolhead actuated by a micro-servo motor lifts and lowers the pen/puncher[cite: 6].
*   **Structure:** Built around 20x20mm aluminum extrusions, corner brackets, and 3D-printed mounts (available in this repository)[cite: 6].

<br>

## 📁 Repository Structure
This repository contains the mechanical assets of the project:
*   `/CAD_Parts/`: Contains the `.prt` (Creo) and `.stl` files of the 3D printed components (motor brackets, pulley mounts, toolhead slider, etc.)[cite: 6].
*   `/Assembly/`: Screenshots and renders of the CAD assembly[cite: 6].
*   `BOM.pdf`: The Bill of Materials listing the mechanical and electronic components[cite: 6].

<br>

## 🚀 Results & Challenges
The machine was successfully assembled and the Arduino CNC Shield correctly received and executed G-Code via ChiliPeppr/GRBL[cite: 6]. 
One of the main challenges was the structural rigidity required for the Braille function[cite: 6]. Braille dots require precise 2.3mm spacing and significant downward force[cite: 6], which pushed the limits of our 3D-printed toolhead rigidity, leading us to focus primarily on the 2D drawing capabilities for the final demonstration[cite: 6].

---
*Project Team: Celyann CEARD (CAD & Assembly), Julien RIOU (Project Manager & Software), Quentin DREULETTE, Lucas GALMAR.*[cite: 6]
