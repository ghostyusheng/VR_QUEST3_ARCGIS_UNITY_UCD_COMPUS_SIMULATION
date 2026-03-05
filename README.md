version https://git-lfs.github.com/spec/v1
oid sha256:b92c6c60327cff5642522f55b8cb7ac721457d933c9cda365d4a12d8b196329e
size 98
```
This repository contains a technical prototype developed during a research project at University College Dublin.

All datasets used are publicly available or excluded from the repository.
This repository is shared for research and educational purposes.
```

![2026-02-11203335-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/98a0b679-8e3c-4c77-a127-4e5d7291b1bc)
![2026-02-11203335-ezgif com-video-to-gif-converter (1)](https://github.com/user-attachments/assets/09d9d332-6cb5-4ae3-b19d-f9f928f3ad83)
![2026-02-11203738-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/ff76226d-dd17-45bc-a6bc-c1c9f6960900)
<img width="1920" height="935" alt="Snipaste_2026-02-11_20-38-15" src="https://github.com/user-attachments/assets/d37948e1-66df-49d0-b48b-d14f68d256c2" />
<img width="1916" height="904" alt="Snipaste_2026-02-11_20-39-28" src="https://github.com/user-attachments/assets/341f13ce-22dd-4be6-800f-6b644920d488" />


# VR Quest 3 ArcGIS Unity Campus Simulation

XR-based campus simulation system integrating **ArcGIS spatial data into Unity runtime**, deployed on **Meta Quest 3**.

---

# Project Overview

This project implements an **immersive XR campus simulation system** built with **Unity** and deployed on **Meta Quest 3**.

The system integrates **ArcGIS spatial data** into a real-time Unity environment, enabling **spatial visualization and interactive navigation** within a 3D representation of the **UCD Belfield campus**.

The primary goal of this project was to design a **robust integration pipeline between GIS data, Unity runtime rendering, and XR device deployment**.

---

# System Architecture

## High-Level Architecture

```
        ArcGIS Spatial Data
              │
              ▼
     ArcGIS SDK for Unity
              │
              ▼
      Unity Simulation Engine
   (XR Interaction + Scenarios)
              │
              ▼
         Quest 3 Runtime
        (Immersive VR User)
```

---

# Core Features

## Spatial Data Integration

- Imported **ArcGIS spatial datasets** into Unity using **ArcGIS SDK for Unity**
- Processed GIS layers and mapped **geospatial coordinates into Unity world space**
- Managed rendering of:
  - Terrain
  - Road networks
  - Campus infrastructure

## XR Interaction & Navigation

- Implemented **XR locomotion and interaction system**
- Enabled immersive navigation within the campus environment
- Optimized scene rendering for **Meta Quest 3 standalone performance**
- Managed runtime constraints such as GPU usage and memory allocation

## Backend Synchronization

- Built a **Python-based spatial preprocessing pipeline**
- Implemented structured data flow between **backend processing and Unity client**
- Ensured **coordinate consistency and spatial data normalization**

## Deployment & Device Debugging

- Resolved **SDK-level integration issues** specific to Quest 3
- Configured **Android build environment** for XR deployment
- Managed **XR plugin compatibility**
- Prepared deployment documentation and **handover guide**

---

# Technical Stack

| Category | Technology |
|--------|-----------|
| Game Engine | Unity |
| XR Framework | XR Interaction Toolkit |
| Spatial Data | ArcGIS SDK for Unity |
| XR Hardware | Meta Quest 3 |
| Backend Processing | Python |
| Programming Languages | C# / Python |
| Deployment Platform | Android |

---

# Engineering Challenges

## Coordinate System Alignment

One of the main technical challenges was aligning **ArcGIS geospatial coordinates** with **Unity’s world coordinate system** while maintaining spatial accuracy within the simulation environment.

## XR Performance Optimization

Standalone XR devices impose **GPU and memory constraints**. Scene complexity and asset loading strategies were optimized to maintain **stable frame rates and smooth interaction**.

## SDK Compatibility

Several compatibility issues arose between **Unity XR plugins**, **ArcGIS SDK**, and the **Quest 3 runtime environment**, requiring version management and configuration adjustments to ensure stable builds.

---

# Repository Structure

```
Assets/
Scripts/
Backend/
Build/
Documentation/
```

---

# Deployment Guide

### 1. Install Unity

Install Unity version:

```
2022.3.62f1
```

### 2. Import Dependencies

Import required packages:

- XR Interaction Toolkit
- ArcGIS SDK for Unity
- Android Build Support

### 3. Configure XR Environment

- Set **Android** as the build target
- Enable **Quest 3 XR plugin**
- Configure XR settings within Unity

### 4. Build and Deploy

Build the project and deploy to the device using **ADB**.

Configure Android build target

Enable Quest 3 XR plugin

Build and deploy via ADB

---

# Author

**Yusheng Zhang**

MSc Intelligent Robotics / MSc Computer Science - VR 

Trinity College Dublin

University of York



