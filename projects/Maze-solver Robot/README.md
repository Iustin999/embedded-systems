# Maze-solver Robot

## Descriere (RO)

Acest proiect reprezintă un robot autonom capabil să rezolve un labirint folosind un singur senzor de distanță și două servo-motoare pentru deplasare. Constrângerile impuse în cadrul competiției au limitat soluția hardware la aceste componente.

### Algoritm de navigație

Pentru a detecta direcțiile libere, robotul se rotește complet pe loc (nu doar senzorul), prin mișcarea diferențiată a roților: un servo merge înainte, celălalt înapoi. Astfel, robotul execută viraje precise fără a necesita un mecanism suplimentar pentru rotirea senzorului.

Strategia aleasă:
- La fiecare intersecție, robotul se rotește 90° spre stânga și verifică distanța față de obstacol.
- Dacă stânga este liberă, continuă deplasarea în acea direcție până la următorul zid.
- Dacă stânga este blocată, se rotește 180° (spre dreapta, față de poziția inițială) și avansează direct, fără a irosi timp măsurând în dreapta.

Mișcările au fost calibrate precis în funcție de durata de acționare a servo-motoarelor, astfel încât robotul să efectueze virajele la unghiuri exacte.

### Tehnologii utilizate

- Microcontroler programabil
- Senzor de distanță (HC-SR04)
- Servo-motoare pentru deplasare și rotire
- Control implementat în limbaj C



## Project Description (EN)

This is an autonomous robot designed to solve a maze using only one distance sensor and two servo motors for movement. The competition required the use of only these components, with no dedicated sensor rotation mechanism.

### Navigation algorithm

The robot rotates its entire body to scan the environment, using differential motion: one wheel moves forward while the other moves backward. This allows precise turning without additional hardware.

The implemented strategy:
- At intersections, the robot rotates 90° to the left and checks for free space.
- If the left side is open, it moves in that direction until it encounters the next wall.
- If the left is blocked, it rotates 180° (i.e., turns right relative to original heading) and proceeds without checking right, saving time.

Rotations were calibrated based on time to ensure accuracy and consistency.

### Technologies used

- Programmable microcontroller
- Distance sensor (HC-SR04)
- Servo motors for rotation and movement
- Control logic written in C
