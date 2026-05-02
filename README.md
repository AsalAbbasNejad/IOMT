# PCG-Based Heart Sound Analysis for IoMT Applications

## Overview

This project focuses on processing and analyzing Phonocardiogram (PCG) signals for heart sound analysis. The main goal is to convert noisy heart-sound audio recordings into useful cardiac information that can support an Internet of Medical Things (IoMT) prototype.

The system takes a raw WAV heart-sound recording as input, applies preprocessing and filtering, detects the main heart sounds S1 and S2, segments the cardiac cycle into different phases, and extracts measurable features from each cycle.

> Note: This project is intended for signal processing and educational purposes only. It is not a medical diagnostic tool.

---

## Project Goal

The goal of this project is to develop a signal processing pipeline that can:

- Clean noisy PCG audio signals
- Remove powerline and high-frequency noise
- Detect S1 and S2 heart sound peaks
- Segment the cardiac cycle into S1, systole, S2, and diastole
- Extract timing and energy-based features
- Support further analysis for abnormal cycle or murmur detection

---

## What is PCG?

PCG stands for Phonocardiogram. It is a recording of the sounds produced by the heart during the cardiac cycle.

The two main heart sounds are:

- **S1**: The first heart sound, usually related to the closure of the mitral and tricuspid valves
- **S2**: The second heart sound, usually related to the closure of the aortic and pulmonary valves

Detecting these sounds helps divide the cardiac cycle into important phases.

---

## Processing Pipeline

The project follows this main workflow:

```text
Raw PCG Audio
      ↓
Preprocessing and Filtering
      ↓
Shannon Energy Envelope
      ↓
S1/S2 Peak Detection
      ↓
Heart Sound Segmentation
      ↓
Feature Extraction
      ↓
Result Visualization and Analysis
 
