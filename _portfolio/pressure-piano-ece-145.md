---
title: "Pressure Piano (ECE 145)"
excerpt: "An Electronic Pressure Piano with Pressure-Based Volume Control and Octave Control<br/><img src='images/pressure-piano-ece-145-cover.png'>"
collection: portfolio
---

From August 2025 to December 2025

As part of a semester-long hardware design project, I co-developed a pressure-sensitive electronic piano that generates dynamically controlled audio using fully analog and digital circuitry.\
The system uses force-sensitive resistors (FSRs) to detect finger pressure, enabling real-time volume modulation and multi-key input combinations. We designed and tuned 21 analog sinusoidal tone generators across three octaves using op-amp–based oscillators and RC networks, with tone selection handled through multiplexers, decoders, and a finite state machine for octave control. The project involved extensive hands-on debugging and validation using oscilloscopes and multimeters, as well as integrating a voltage-controlled amplifier (AD605) for audio output, highlighting challenges in mixed-signal design, noise mitigation, and hardware scalability.\
As a follow-up to some issues noted during the demo of our final product, I am currently working to address the noise generated when any of the lower notes (C ~ E) in octaves 3 and 5 are played.
