---
title: "Pressure Piano (ECE 145)"
excerpt: "An Electronic Pressure Piano with Pressure-Based Volume Control and Octave Control<br/><img src='/images/pressure-piano-ece-145-cover.png'>"
collection: portfolio
---

From August 2025 to December 2025 · ECE 145 final project

<figure class="align-center" style="width: 420px">
  <video controls poster="/images/pressure-piano-demo-poster.jpg" style="width: 100%; border-radius: 6px;">
    <source src="/files/pressure-piano-demo.mp4" type="video/mp4">
    Your browser doesn't support embedded video — <a href="/files/pressure-piano-demo.mp4">download the demo</a>.
  </video>
  <figcaption>A short walkthrough of the completed build (with sound).</figcaption>
</figure>

## Overview

A semester-long hardware design project: a pressure-sensitive electronic piano
that generates dynamically controlled audio through fully analog and digital
circuitry. Rather than simple on/off keys, it reads how hard each key is pressed
and shapes the sound in real time.

<figure class="align-center" style="width: 400px">
  <img src="/images/pressure-piano-full-system.jpg" alt="The completed pressure piano: three breadboards wired together on the bench, powered from a lab supply.">
  <figcaption>The completed system — several breadboards spanning the octaves, powered from the bench supply.</figcaption>
</figure>

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

<figure class="align-center" style="width: 400px">
  <img src="/images/pressure-piano-key-press.jpg" alt="A finger pressing a key on the breadboard during testing.">
  <figcaption>Playing a key by hand during testing.</figcaption>
</figure>

<figure class="align-center" style="width: 400px">
  <img src="/images/pressure-piano-tone-board.jpg" alt="Close-up of a tone-generator board showing op-amp ICs and rows of resistors.">
  <figcaption>A tone-generator board — op-amp oscillators and the resistor networks that set each note.</figcaption>
</figure>

## Building and testing

Most of the work was hands-on mixed-signal debugging and validation with
oscilloscopes and multimeters, and wrestling with noise mitigation and hardware
scalability.

<figure class="align-center" style="width: 400px">
  <img src="/images/pressure-piano-breadboard.jpg" alt="An earlier single-breadboard build wired on the bench.">
  <figcaption>An earlier single-board build on the bench.</figcaption>
</figure>

<figure class="align-center" style="width: 400px">
  <img src="/images/pressure-piano-oscilloscope.jpg" alt="A benchtop oscilloscope displaying a captured trace during testing.">
  <figcaption>Checking signals on the bench oscilloscope.</figcaption>
</figure>

## Follow-up

Following an issue noticed during the final demo, I'm currently working to
address the noise that appears when the lower notes (C–E) in octaves 3 and 5 are
played.
