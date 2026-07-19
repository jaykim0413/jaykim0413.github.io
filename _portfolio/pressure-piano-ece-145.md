---
title: "Pressure Piano (ECE 145)"
excerpt: "An Electronic Pressure Piano with Pressure-Based Volume Control and Octave Control<br/><img src='/images/pressure-piano-ece-145-cover.png'>"
collection: portfolio
---

From August 2025 to December 2025 · ECE 145 final project

![Pressure Piano](/images/pressure-piano-ece-145-cover.png)

## Overview

A semester-long hardware design project: a pressure-sensitive electronic piano
that generates dynamically controlled audio through fully analog and digital
circuitry. Rather than simple on/off keys, it reads how hard each key is pressed
and shapes the sound in real time.

## How it works

- **Pressure sensing.** Force-sensitive resistors (FSRs) under the keys detect
  finger pressure, driving real-time volume modulation and multi-key input.
- **Tone generation.** 21 analog sinusoidal tone generators span three octaves
  (C3–B5), built from op-amp oscillators and RC networks; each was tuned and its
  frequency accuracy verified on an oscilloscope.
- **Control logic.** Tone selection and routing run through multiplexers and
  decoders, with a finite state machine handling octave selection.
- **Audio output.** An AD605 voltage-controlled amplifier sets output gain from
  the average pressure across pressed keys — harder presses play louder.

## What we took away

Most of the work was hands-on mixed-signal debugging and validation with
oscilloscopes and multimeters, and wrestling with noise mitigation and hardware
scalability.

## Follow-up

Following an issue noticed during the final demo, I'm currently working to
address the noise that appears when the lower notes (C–E) in octaves 3 and 5 are
played.
