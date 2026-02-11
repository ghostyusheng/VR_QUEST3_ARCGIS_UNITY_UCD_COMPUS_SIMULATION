version https://git-lfs.github.com/spec/v1
oid sha256:b92c6c60327cff5642522f55b8cb7ac721457d933c9cda365d4a12d8b196329e
size 98
![2026-02-11203335-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/98a0b679-8e3c-4c77-a127-4e5d7291b1bc)
![2026-02-11203335-ezgif com-video-to-gif-converter (1)](https://github.com/user-attachments/assets/09d9d332-6cb5-4ae3-b19d-f9f928f3ad83)
![2026-02-11203738-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/ff76226d-dd17-45bc-a6bc-c1c9f6960900)
<img width="1920" height="935" alt="Snipaste_2026-02-11_20-38-15" src="https://github.com/user-attachments/assets/d37948e1-66df-49d0-b48b-d14f68d256c2" />
<img width="1916" height="904" alt="Snipaste_2026-02-11_20-39-28" src="https://github.com/user-attachments/assets/341f13ce-22dd-4be6-800f-6b644920d488" />


1️⃣
VR Quest 3 ArcGIS Unity Campus Simulation

XR-based campus simulation system integrating ArcGIS spatial data into Unity runtime, deployed on Meta Quest 3.

2️⃣ Project Overview

This project implements an immersive XR campus simulation system built with Unity and deployed on Meta Quest 3.

The system integrates ArcGIS spatial data into a real-time Unity environment, enabling spatial visualization and interactive navigation within a 3D representation of UCD Belfield campus.

The primary goal of this project was to design a robust integration pipeline between GIS data, Unity runtime rendering, and XR device deployment.

3️⃣ System Architecture

这里写成结构说明：

High-Level Architecture

Unity (XR Runtime)
↕
ArcGIS SDK for Unity
↕
Python Backend (Spatial Data Preparation)
↕
Quest 3 Device Deployment

4️⃣ Core Features
Spatial Data Integration

Imported ArcGIS spatial datasets into Unity using ArcGIS SDK

Processed GIS layers and mapped geospatial coordinates into Unity world space

Managed terrain, road network and campus structure rendering

XR Interaction & Navigation

Implemented XR locomotion and interaction system

Optimized scene rendering for Quest 3 device constraints

Managed runtime performance for standalone headset environment

Backend Synchronization

Built Python-based spatial preprocessing pipeline

Implemented structured data flow between backend and Unity client

Ensured coordinate consistency and data normalization

Deployment & Device Debugging

Resolved SDK-level integration issues specific to Quest 3

Handled Android build configuration and XR plugin compatibility

Prepared deployment documentation and handover guide

5️⃣ Technical Stack

Unity (XR Interaction Toolkit)

ArcGIS SDK for Unity

Meta Quest 3

Python (Data Processing)

C#

Android Build Environment

6️⃣ Engineering Challenges

Instead of writing “it was hard”, write like this:

Coordinate System Alignment

One of the main technical challenges was aligning ArcGIS geospatial coordinates with Unity’s world coordinate system while maintaining spatial accuracy.

XR Performance Optimization

Standalone XR devices impose GPU and memory constraints. Scene complexity and asset loading strategies were optimized to maintain stable frame rate.

SDK Compatibility

Resolved version conflicts between Unity XR plugins and Quest 3 runtime environment.

7️⃣ Repository Structure

Assets/
Scripts/
Backend/
Build/
Documentation/

8️⃣ Deployment Guide (Short)

Install Unity version 2022.3.62f1

Import required XR and ArcGIS packages

Configure Android build target

Enable Quest 3 XR plugin

Build and deploy via ADB
