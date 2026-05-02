# TechMath±
An interactive math learning game for primary school children that turns basic arithmetic into a physical, embodied experience.

About the Project
TechMath is an interactive educational game designed to make basic mathematics engaging and intuitive for primary school children (ages 6–9). Instead of typing numbers on a keyboard or tapping a screen, children solve math problems through natural, physical interactions — using their hands, their bodies, and tangible objects.
The project is built around a simple idea: math should be felt, not just calculated. By translating numerical answers into physical gestures, we aim to lower the cognitive barrier to learning arithmetic and create stronger, more memorable associations between numbers and quantities.
This is an academic project developed as part of the Interaction Design (IxD) module at Hochschule Luzern (HSLU).

The Two Game Modes
✊ Squeeze It! (Hardware Mode)
Children solve math problems by squeezing a soft physical object equipped with an FSR (Force-Sensitive Resistor) pressure sensor. The harder they squeeze, the higher the on-screen number climbs. When they reach the correct answer, they hold steady for two seconds to submit.

Built with Arduino Nano + FSR pressure sensor
Communicates with the browser via the Web Serial API
Visualized with animated p5.js particle effects

✋ Finger Math (Webcam Mode)
Children show their answer using finger counting, just like they naturally would in a classroom. The webcam tracks their hands in real time, counts the fingers shown, and submits the answer when the child closes their hand into a fist.

Hand tracking powered by ml5.js HandPose
Adaptive difficulty system that scales with the child's performance
Supports answers up to 20 (using two-fist input for numbers above 10)

Technology Stack
Layer                 Technology
Creative coding       p5.js
Hand tracking         ml5.js HandPose
Hardware              Arduino Nano + RP-S40-ST FSR sensor
Hardware bridge       Web Serial API
Hosting               GitHub Pages

Getting Started

Clone or download this repository.
Open the project folder in VS Code and start a local server (e.g. Live Server).
Both Web Serial and webcam access require a real server — file:// will not work.
Open index.html in Chrome or Edge (Web Serial is not supported in Firefox or Safari).
Choose a game mode from the main menu and start playing.
For the Squeeze It! mode, you will additionally need:
An Arduino Nano flashed with a sketch that prints FSR:<value> over serial at 9600 baud.
An RP-S40-ST FSR sensor wired with a pull-down resistor.

Authors
This project was designed, developed, and produced by:

Nevzat Onay
Mert Karan Nazikoğlu

Both authors are students of the Interaction Design module at Hochschule Luzern (HSLU).

Copyright & Rights
© 2026 Nevzat Onay and Mert Karan Nazikoğlu. All rights reserved.
All intellectual property rights to this project — including but not limited to the source code, game design, visual design, concept, written documentation, and project name "TechMath" — belong exclusively to Nevzat Onay and Mert Karan Nazikoğlu.
This project may not be copied, modified, redistributed, republished, or used for commercial purposes — in whole or in part — without the explicit written permission of both authors. Any unauthorized use, reproduction, or derivative work constitutes a violation of the authors' rights.
Educational viewing and academic referencing are permitted, provided that proper attribution is given to both authors.
For licensing inquiries, collaboration requests, or permission to use any part of this project, please contact the authors directly.
