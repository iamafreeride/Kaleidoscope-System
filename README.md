# Kaleidoscope System

> A distributed physical entropy generation system based on optical chaos and environmental randomness.

---

https://iamafreeride.github.io/Kaleidoscope-System/

# Overview

The Kaleidoscope System is a physical entropy generation architecture that utilizes optical chaos, environmental perturbations, and distributed sensing nodes to continuously generate high-entropy data.

Unlike traditional pseudo-random number generators (PRNGs), this project focuses on harvesting randomness from real-world physical phenomena.

The concept is inspired by the visual complexity of the Cloudflare LavaRand (lava lamp wall), while extending it into a scalable, distributed, multi-node entropy network.

---

# Design Goals

* Harvest entropy from naturally occurring physical phenomena.
* Utilize complex optical reflection to amplify environmental variation.
* Support distributed entropy collection across multiple geographic locations.
* Detect degraded or predictable entropy sources automatically.
* Scale from a small experimental prototype to room-scale installations.

---

# System Architecture

```
Physical Environment
        │
        ▼
Optical Chaos Chamber
        │
        ▼
Camera / Sensors
        │
        ▼
Entropy Extraction
        │
        ▼
Node Entropy Output
        │
        ▼
Distributed Entropy Pool
        │
        ▼
Seed Generation
```

---

# Entropy Sources

The system intentionally combines numerous independent physical variables.

## Optical

* Ambient light
* Artificial light
* Reflection
* Refraction
* Diffusion
* Shadow
* Polarization (optional)

## Environmental

* Airflow
* Wind direction
* Temperature
* Humidity
* Atmospheric pressure
* Vibration
* Acoustic noise

## Hardware

* CMOS sensor noise
* Dark current
* Shot noise
* Thermal noise
* ADC quantization error
* Sensor timing jitter

---

# Single Node

A node may consist of any computing platform capable of reading sensors and producing digital output.

## Required Components

* Computer or microcontroller
* Camera or optical sensor
* Enclosure
* Reflective objects
* Mounting materials

Component selection is unrestricted.

Possible implementations include:

* ESP32-S3
* Raspberry Pi
* Linux PC
* Industrial controller

Possible image sensors include:

* OV3660
* OV2640
* OV5640
* USB Camera
* Industrial Camera

---

# Prototype Example

Container

* Shoebox

Reflective Objects

* Broken mirrors
* Broken glass bottles
* Crumpled aluminum foil
* Metal sheets
* Transparent materials

Mounting

* Shoelaces
* Springs
* Hot glue
* Adhesives
* Flexible supports

Construction

* Drill multiple holes into the enclosure.
* Suspend or fix reflective objects randomly.
* Allow environmental influence from airflow and lighting.

---

# Data Collection

Example:

* 30 FPS image capture
* RAW sensor frames

Possible extracted features include:

* RGB values
* Bayer RAW
* Grayscale
* Pixel differences
* Histograms
* Edge detection
* Frequency-domain analysis
* Temporal variation

---

# Entropy Extraction

Raw sensor data should not be used directly.

Instead, entropy should be extracted using a cryptographic mixing process.

Possible extractors include:

* SHA-256
* SHA-3
* BLAKE3
* HKDF
* XOR folding (preprocessing)

The output is an arbitrary-length alphanumeric seed or binary entropy stream.

---

# Distributed Architecture

Multiple independent nodes can operate simultaneously.

Example deployment:

* Taipei
* Tokyo
* London
* New York
* Arctic
* Antarctic
* Vehicles
* Aircraft
* Ships
* Drones

Each node contributes entropy to a shared entropy pool.

```
Node A
     │
Node B
     │
Node C
     │
Node D
     │
Entropy Pool
     │
SHA-3 / BLAKE3
     │
Generated Seed
```

---

# Node Health Monitoring

Nodes are continuously evaluated.

Possible failure conditions include:

* Nearly identical output over time
* Static image
* All-black frames
* All-white frames
* Sensor failure
* Communication loss
* Entropy below threshold
* Abnormally repetitive output

Failed nodes are automatically excluded from the entropy pool until recovery.

---

# Scalability

The architecture is intended to scale across many deployment sizes.

Examples include:

* Shoebox prototype
* Desktop device
* Wall installation
* Entire room
* Building
* Global distributed network

---

# Potential Applications

* Random number generation
* Cryptographic seed generation
* Security research
* Distributed entropy services
* Chaos visualization
* Interactive installations
* Experimental physics

---

# Project Status

Concept / Experimental

This repository currently documents the architecture and design concepts of the Kaleidoscope System.

Future work may include:

* Prototype hardware
* Entropy evaluation
* Software implementation
* Statistical randomness testing
* Distributed node synchronization

---
