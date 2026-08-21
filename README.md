# RADEXIUM™

### Radiation Detection & Sensing System

RADEXIUM™ is an independent radiation monitoring and sensing project created by **Akash K**.

The project explores how radiation measurements can be collected, processed, stored, monitored, and presented through a single system. The current version is software-based and uses simulated radiation data. The long-term objective is to connect the software with physical radiation-sensing hardware.

RADEXIUM is currently a **prototype and development project**, not a certified radiation detection instrument.

---

## About the Project

Radiation cannot be seen or detected directly by human senses. A monitoring system therefore needs to turn radiation measurements into information that can be understood and acted upon.

RADEXIUM was developed around this idea.

The current system simulates the behavior of a radiation-monitoring device and sends the resulting data to a web dashboard. The dashboard presents the current radiation condition, device status, historical readings, and other information in one place.

The basic data flow is:

```text
Radiation Simulation
        ↓
Data Processing
        ↓
Firebase Realtime Database
        ↓
RADEXIUM Dashboard
        ↓
Monitoring and Analysis
```

The software architecture is being developed first so that it can later be connected to physical hardware.

---

## Current Features

### Radioactivity Analytics

The main dashboard provides a live view of the simulated radiation system.

It currently displays:

* Radiation level
* Radiation status
* Battery level
* Alarm status
* Last update time
* Health-impact estimation

The simulator can move between different radiation conditions, allowing the dashboard to be tested under changing circumstances.

The current status categories include:

```text
SAFE
ELEVATED
MODERATE
HIGH
EXTREME
```

These categories are part of the project's current demonstration logic and should not be treated as official radiation-safety limits.

---

## Radiation History

RADEXIUM records radiation readings over time instead of displaying only the latest value.

The history section allows changes in radiation levels to be observed and provides the foundation for future trend analysis.

Further improvements to historical analysis are planned as the project develops.

---

## Device Simulation

The current version simulates several aspects of a radiation-monitoring device.

The simulator can generate:

* Changing radiation readings
* Different radiation conditions
* Battery level changes
* Device status
* Timestamps
* Alarm conditions
* Continuous updates

This makes it possible to develop and test the dashboard without requiring a physical detector.

The Python simulator was previously named:

```text
RADiSense - Multi-Simulator.py
```

The name remains in some parts of the project because RADEXIUM was originally developed under the name **RADiSense**.

---

## Battery and Alarm

Battery behavior is simulated alongside the radiation readings.

The simulated battery gradually decreases to represent the operation of a portable monitoring device.

The system also includes alarm logic for high radiation conditions and low-battery conditions.

These features are currently intended for demonstration and software testing. The behavior of a future physical device will depend on the hardware and its operating requirements.

---

## Radiation Units Guide

RADEXIUM includes a Radiation Units Guide to help users understand the measurements associated with radiation.

The guide covers concepts such as radiation dose and biological effect and introduces commonly used radiation units, including the **sievert (Sv)**.

The purpose of the guide is to provide context for the values displayed by the dashboard and to help distinguish between different types of radiation measurements.

---

## Health Impact Estimation

The dashboard includes a health-impact estimator based on the current simulated radiation level.

This feature is intended to provide an understandable interpretation of the simulated reading.

It is **not a medical assessment or a validated radiation-dose calculation** and should not be used for real-world health or safety decisions.

---

## Technology

RADEXIUM currently uses the following technologies:

| Purpose                        | Technology                         |
| ------------------------------ | ---------------------------------- |
| Radiation simulation           | Python                             |
| Data storage and communication | Firebase Realtime Database         |
| Web dashboard                  | Lovable                            |
| Source control                 | GitHub                             |
| Hardware simulation            | Tinkercad / Wokwi                  |
| Future hardware                | Microcontroller + radiation sensor |

---

## Firebase

Firebase Realtime Database acts as the communication and storage layer between the simulator and the dashboard.

The current development project uses:

```text
Firebase Project ID: radisense-8829
```

This identifier comes from the earlier RADiSense version of the project.

Private Firebase credentials and keys are not included in this repository.

---

## Dashboard

The RADEXIUM dashboard is developed using Lovable.

The current dashboard contains the following sections:

* Radioactivity Analytics
* Radiation History
* Display Settings
* Server Details
* About RADEXIUM
* Radiation Units Guide
* About the Creator

The interface uses a black, yellow, and white visual theme inspired by radiation-warning and scientific instrumentation design.

---

## Hardware Development

The current RADEXIUM system does **not** contain a completed physical radiation detector.

The present version is a software simulation.

The next major stage of development is the integration of a physical radiation sensor with a microcontroller.

The intended architecture is:

```text
Radiation Sensor
       ↓
Microcontroller
       ↓
Data Processing
       ↓
Network Connection
       ↓
Firebase
       ↓
RADEXIUM Dashboard
```

Potential hardware components being considered include:

* Radiation / Geiger sensor
* ESP8266-class microcontroller
* Display
* LEDs
* Buzzer
* Battery or other power source

Hardware development is planned for a later stage, with development currently targeted around **2027**.

The exact hardware design will depend on the selected sensor, calibration requirements, testing, and practical implementation.

---

## Development Status

### Completed

* Radiation simulation
* Variable radiation conditions
* Firebase integration
* Live dashboard
* Radiation analytics
* Radiation history
* Battery simulation
* Alarm simulation
* Device status monitoring
* Health-impact estimation
* Radiation Units Guide
* Dashboard settings
* Server information
* Initial software architecture

### Planned

* Physical radiation sensor
* Microcontroller integration
* Real sensor readings
* Hardware-to-cloud communication
* Physical alarm
* Hardware battery monitoring
* Hardware display
* Sensor calibration
* System testing and validation
* Expanded radiation analysis
* Configurable thresholds
* User profiles

---

## Project Evolution

RADEXIUM was originally developed under the name **RADiSense**.

As the project developed, its name and identity were changed to **RADEXIUM™**.

Some existing technical identifiers still use the previous name, including:

```text
radisense-8829
RADiSense - Multi-Simulator.py
RADiSense GitHub repository
```

These are legacy identifiers from earlier development and do not represent the current project name.

The current project identity is:

```text
RADEXIUM™
Radiation Detection & Sensing System
```

---

## Repository

The project was originally maintained under the repository name:

```text
innovatorakash88/RADiSense
```

The repository name may retain the original project name while the software and branding are being developed under RADEXIUM™.

---

## Limitations

RADEXIUM is still under development.

The current system has several important limitations:

* Radiation measurements are simulated.
* No calibrated physical radiation sensor is currently connected.
* Radiation categories are demonstration logic rather than regulatory limits.
* The health-impact estimator is not a medical or safety assessment.
* The system has not been certified for professional radiation monitoring.
* The physical hardware prototype has not yet been completed.

A real radiation-monitoring system would require appropriate sensors, calibration, testing, validation, safety considerations, and compliance with applicable requirements.

---

## Disclaimer

RADEXIUM™ is an independent prototype and development project.

It is not currently a certified radiation detector, medical device, industrial safety instrument, or government-approved radiation monitoring system.

The simulated readings and information produced by the current software should not be used to make real-world radiation-safety or medical decisions.

---

## License

### RADEXIUM™ Evaluation and Competition License

**Version 1.0 — 2026**

**Copyright © 2026 Akash K**
**Founder and Creator of RADEXIUM™ — All Rights Reserved.**

RADEXIUM™ is provided under the **RADEXIUM™ Evaluation and Competition License**.

The license allows limited use of the software for academic, research, evaluation, and competition purposes.

### Permitted Use

The Software may be used for:

* Academic demonstrations
* Research and evaluation
* Science fairs, exhibitions, and competitions
* Non-commercial internal review

### Not Permitted

Without written permission from the copyright owner, the following are not permitted:

* Copying or redistributing the source code
* Commercial use or monetization
* Modifying the Software or creating derivative works
* Claiming ownership of the Software
* Republishing the Software as another project
* Rebranding the Software or presenting it under another name

### Trademark

**RADEXIUM™** and its associated branding are claimed trademarks of **Akash K**.

Use of the RADEXIUM™ name, logo, or branding in a way that suggests ownership, endorsement, affiliation, or authorization is not permitted without prior written permission.

### Disclaimer

The Software is provided **"AS IS"**, without warranties of any kind.

The creator is not liable for damages or losses arising from the use, misuse, interpretation, or inability to use the Software.

### Termination

Any use outside the permissions granted by this license immediately terminates the license.

Upon termination, all unauthorized use of the Software must cease.

### Governing Law

This License is governed by the laws of **India**.

Any dispute relating to this License shall be subject to the applicable jurisdiction of the courts of India.

The complete license is available in the `LICENSE` file in this repository.

---

## Creator

**Akash K**

Founder and Creator of RADEXIUM™

RADEXIUM is a self-initiated project combining radiation science, software development, real-time data systems, and planned embedded hardware.

---

## Project Vision

The current version of RADEXIUM is only the beginning of the project.

The development path is intended to progress from:

```text
Software Simulation
        ↓
Real-Time Monitoring Platform
        ↓
Physical Sensor Integration
        ↓
Hardware Testing
        ↓
Calibration and Validation
        ↓
Complete Radiation Sensing System
```

The goal is to develop the software and hardware as parts of one system rather than treating the dashboard as a separate application.

---

**RADEXIUM™**
*Radiation Detection & Sensing System*

**Copyright © 2026 Akash K. All Rights Reserved.**
