---
layout: project
title: "LpGL: Low-power Graphics Library"
subtitle: "OpenGL-compatible library for mobile AR headsets"
date: 2019-06-01
period: "2017 - 2020"
status: "completed"
technologies: ["C++", "OpenGL", "Computer Graphics", "AR/VR", "Mobile Systems"]
links:
  - title: "ACM MobiSys Paper"
    url: "https://dl.acm.org/doi/10.1145/3307334.3326103"
---

## Project Overview

OpenGL-compatible low-power graphics library designed specifically for mobile AR headsets (Microsoft HoloLens, Magic Leap One) that exploits user perceptual information to reduce power consumption.

## Key Innovation

Leveraging **user perceptual information** such as:
- Head orientation tracking
- Eye tracking data (gaze-aware rendering)
- Attention-based rendering optimization
- User-perception-aware graphics pipeline optimization

## Technical Achievements

- **OpenGL compatibility** - seamless integration with existing applications
- **22% energy reduction** in total system consumption
- **Real-time performance** for interactive AR applications (only ~46μs added latency per object)
- **User study validation** with 25 participants showing no significant impact on perceived visual quality
- **Extended battery life** from 3.0 to 3.9 hours on Magic Leap One

## Publications & Recognition

- 🏆 **Best Demo Award** - ACM HotMobile 2019
- 📄 **Main Conference Paper** - ACM MobiSys 2019 (22% acceptance rate)
- 🎯 **Demo Presentation** - ACM HotMobile 2019

## Technical Components

### 1. Gaze- and Head-Aware Rendering
- Leverages gaze and head orientation data to infer user's focal area
- Selectively simplifies or culls objects outside focal region

### 2. Mesh Simplification
- Reduces triangle count for 3D meshes outside core field of view
- Heavy simplification for peripheral/out-of-view objects to save GPU and memory

### 3. Dynamic Frame Rate Control
- Analyzes scene dynamics between frames
- Adjusts frame rate in real-time based on motion/viewpoint changes

### 4. Advanced Culling Techniques
- Beyond standard frustum culling
- Bounding box-based visibility checks for perceptually irrelevant regions

### 5. Reactive Display Complexity Control Engine
- Coordinates mesh simplification, frame rate adjustment, and culling
- Ensures energy efficiency with minimal user-visible degradation

## Master's Thesis

- **Title:** "Low-power Graphics Library Design for Mobile AR Headsets"
- **Institution:** Ajou University
- **Advisor:** Prof. JeongGil Ko
- **Completion:** February 2020

## Impact

- Enables longer battery life for mobile AR devices
- Maintains visual quality through perceptual optimization
- Provides drop-in replacement for existing OpenGL applications