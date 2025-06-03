# Obstacle Avoidance & Follow-Me Robot

## Description (EN)

This project presents the design and implementation of a mobile robot capable of autonomously avoiding obstacles and optionally following objects in front of it. The system uses an ultrasonic distance sensor and DC motors controlled by an Arduino microcontroller. Bluetooth functionality is also integrated for manual control via smartphone.

The robot was built as part of the "Robot Control Systems" course at the Petroleum-Gas University of Ploiești.

### Key Features
- Autonomous obstacle avoidance
- "Follow-me" mode: maintains safe distance from object ahead
- DC motors controlled via PWM
- Ultrasonic sensor for distance measurement
- Bluetooth control mode (manual override)
- Mecanum wheels for omnidirectional movement

### Technical Overview
The robot continuously reads the distance to objects using an ultrasonic sensor. If the distance drops below a safety threshold, it stops or adjusts its path accordingly. It can also follow an object placed in front of it at a stable distance, updating its speed and direction based on real-time measurements.

Control logic is implemented in C++ using the Arduino IDE, with sensor data acquisition, obstacle detection, and motor control all handled on the microcontroller.

### Documentation
Full technical report available here:  
[Documentation Obstacle avoidance & Follow me Robot.pdf](./Documentation%20Obstacle%20avoidance%20&%20Follow%20me%20Robot.pdf) (written in Romanian)

---

## Descriere (RO)

Acest proiect prezintă realizarea unui robot mobil autonom, capabil să evite obstacolele din mediul înconjurător și să urmeze un obiect aflat în fața sa. Sistemul se bazează pe un senzor de distanță cu ultrasunete și motoare DC, controlate printr-un microcontroller Arduino. De asemenea, robotul poate fi controlat de la distanță prin Bluetooth.

Proiectul a fost realizat în cadrul disciplinei „Sisteme de Conducere a Roboților” la Universitatea Petrol-Gaze din Ploiești.

### Funcționalități
- Evitare automată a obstacolelor
- Modul „Follow-me” – urmărirea unui obiect la distanță constantă
- Controlul motoarelor prin semnale PWM
- Măsurarea distanței cu senzor ultrasonic
- Modul Bluetooth pentru control extern
- Roti mecanum pentru mobilitate omnidirecțională

### Descriere tehnică
Robotul măsoară continuu distanța față de obstacole. Dacă un obiect este detectat sub pragul de siguranță, robotul oprește sau își modifică traiectoria. În modul „follow-me”, robotul menține o distanță constantă față de un obiect în mișcare, adaptând viteza și direcția.

Toată logica este implementată în C++ prin intermediul Arduino IDE, microcontrollerul preluând senzorii, procesând datele și controlând motoarele.

### Documentație
Documentația completă a proiectului este inclusă în fișierul:  
[Documentation Obstacle avoidance & Follow me Robot.pdf](./Documentation%20Obstacle%20avoidance%20&%20Follow%20me%20Robot.pdf)
