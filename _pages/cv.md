---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* B.S. in Electrical Engineering, University of Illinois at Urbana-Champaign, 2029 (expected)
  * Minor in Psychology
  * Minor in Semiconductor Engineering
  * GPA: 4.00 / 4.00

Honors and Awards
======
* James Scholar Honors — Fall 2025, Spring 2026, Fall 2026
* Dean's List — Fall 2025, Spring 2026

Work experience
======
<!-- TODO: No current roles. Add research positions, internships, or on-campus
     jobs here as they come up. Format per entry:
* Term Year: Role Title
  * Organization
  * What you did (one or two lines)
-->

Projects
======
* **Electronic Pressure Piano** (Sept 2025 – Dec 2025)
  * Designed and built a pressure-sensitive electronic piano using force-sensitive resistors (FSRs) for real-time volume modulation.
  * Implemented 21 analog sinusoidal tone generators (C3–B5) with op-amp oscillators and RC networks; verified frequency accuracy on an oscilloscope.
  * Developed hardware control logic for multi-key detection and FSM-based octave selection, routing signals through multiplexers.
  * Integrated an AD605 voltage gain amplifier to control output gain from the average pressure of the keys pressed.

* **Dental Panoramic X-ray Segmentation** (Sept 2023 – Oct 2024)
  * Built a deep-learning pipeline for dental panoramic X-ray segmentation with U-Net as the base model.
  * Integrated CBAM attention mechanisms to improve feature representation and segmentation performance.
  * Proposed a novel data augmentation and regularization strategy, expanding the dataset ~1200× to improve generalization on limited medical imaging data.
  * Published and presented at the ECCV 2024 BioImage Computing Workshop (DOI: 10.1007/978-3-031-91721-9_17); code at [github.com/jaykim0413/seg-pano-extended](https://github.com/jaykim0413/seg-pano-extended).

Skills
======
* Programming: Java, Python, C++, Embedded C, Rust
* ML / scientific computing: PyTorch, NumPy
* Hardware & EDA: KiCAD, Altium Designer
* Instrumentation: Keysight oscilloscopes, bench power supplies

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Leadership and Activities
======
* Aug 2025 – Present: Electrical Team Member, RoboSub — iRobotics
  * Designed 2-layer band-pass filter PCBs to isolate four target frequency bands (25, 30, 35, 40 kHz) from amplified hydrophone signals, feeding an ADC front end to trigger operations.
  * Designed a 2-layer boost converter PCB stepping the battery's 5 V up to 12 V at 2 A to drive an additional motor on the autonomous submarine.

* Aug 2025 – Present: Steering Wheel Board Member & Software Team Member, Illini Electric Motorsports
  * Designed the schematic and PCB layout for the steering wheel and dashboard boards; manufactured the steering wheel PCB and validated power delivery (rail stability, ripple, load response) on the bench.
  * Verified quadrature-encoder PWM signals (duty cycle, phase offset, signal integrity) and wrote steering-wheel firmware in embedded C on STM32, establishing CAN communication and encoder processing.
