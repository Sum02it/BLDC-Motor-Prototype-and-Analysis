# BLDC-Motor-Prototype-and-Analysis
Design, prototyping, and experimental analysis of a 3-phase BLDC motor using Arduino, ESC, custom rotor, and stator windings.
# Brushless DC (BLDC) Motor: Prototype and Analysis

A hands-on Electrical Engineering project involving the design, construction, and experimental analysis of a three-phase Brushless DC (BLDC) motor prototype.

## 📌 Project Overview

This project focused on designing and building a small-scale BLDC motor prototype using a custom-built stator, rotor, permanent magnets, three-phase windings, an Arduino UNO, and a 30A Electronic Speed Controller (ESC).

The project involved mechanical design, electrical winding design, component selection, hardware assembly, and experimental testing of the motor.

## ⚙️ Working Principle

The BLDC motor operates through sequential energization of the stator windings.

```text
                 Arduino UNO
                      │
                   PWM Signal
                      │
                      ▼
                    ESC
                      │
                3-Phase Current
                      │
                      ▼
              Stator Windings
                      │
             Rotating Magnetic Field
                      │
                      ▼
              Permanent-Magnet Rotor
                      │
                      ▼
               Rotational Motion

The Arduino provides PWM control to the ESC, which energizes the three-phase stator windings in sequence. The resulting rotating magnetic field interacts with the permanent magnets on the rotor to produce rotational motion.

🔧 Hardware Components
Component	Specification
Arduino	Arduino UNO
ESC	30A Brushless ESC
Magnets	8 × 1.5 mm Neodymium magnets
Copper Wire	22 SWG, enamel coated
Stator	6-slot PVC ring with iron bolts
Rotor	4-pole plastic disc
Shaft	17 cm wooden shaft
Windings	Star-connected, 3-phase
Power Supply	Regulated DC supply
🛠️ Stator Design

The stator was constructed using a 6-slot PVC ring with iron bolts acting as poles.

The winding configuration consisted of:

6 coils
80 turns per coil
Double-layer winding
Star-connected three-phase configuration
120° phase shift
Approximate winding factor of 0.866
🔩 Rotor Design

The rotor was designed as a 4-pole plastic disc with:

8 neodymium magnets
8 × 1.5 mm circular magnets
Central wooden shaft

The rotor and stator were mechanically aligned and integrated to form the complete motor prototype.

💻 My Contribution
Proposed the BLDC motor project idea.
Created the CAD model for the motor design.
Supported component selection and design decisions.
Contributed to the overall design and analysis of the prototype.
🧪 Experimental Testing

The assembled prototype was tested using an Arduino, ESC, DC power supply, and oscilloscope.

During manual rotation of the rotor, induced three-phase sinusoidal back-EMF was observed.

The measured waveforms showed approximately 120° phase displacement between the three phases.

📊 Observations
Induced three-phase voltage was successfully detected.
Back-EMF waveforms were approximately sinusoidal.
Approximately 120° phase shift was observed between phases.
Rotor-stator alignment and mechanical fitting were verified.
Minor rotor vibration was observed.
⚠️ Challenges

The prototype experienced several practical limitations:

Weak magnetic field
High friction at the shaft-rotor interface
Less precise coil placement
ESC voltage limitations
Minor rotor vibration
No self-sustained rotation during testing
🚀 Future Scope

Possible improvements include:

Using stronger permanent magnets
Adding Hall-effect sensors for rotor position detection
Using better ball bearings to reduce friction
Improving the precision of coil placement
Using 3D-printed mechanical components
Improving the ESC and drive configuration
📁 Repository Contents
BLDC-Motor-Prototype-and-Analysis/
│
├── BLDC_Motor_Prototype_and_Analysis.pptx
├── BLDC_MOTOR.pdf
└── README.md
📚 Project Documentation

The project presentation and detailed documentation are included in this repository.

👨‍💻 Author

Sumit Kumar Chaudhary

Department of Electrical Engineering
IIT Bhubaneswar


### One thing I'd change before you commit

Your current GitHub repo name is:

**`BLDC-Motor-Prototype-and-Analysis`**

That's good. For the **resume**, use:

> **Brushless DC (BLDC) Motor: Prototype & Analysis**

The project is particularly valuable on your resume because it demonstrates **actual hardware + electrical machine design + CAD + experimental testing**, complementing your Smart LVDT simulation project. Your presentation documents the custom 6-slot/4-pole design, three-phase star-connected windings, and experimental back-EMF verification. :contentReference[oaicite:1]{index=1} :contentReference[oaicite:2]{index=2}

After pasting it into `README.md`, run:

```bash
git add README.md
git commit -m "Add BLDC project documentation"
git push