# SkyAutoNet Autonomous Driving

<p align="center">
  <strong>Connected · Intelligent · Autonomous</strong>
</p>

<p align="center">
  Autonomous Driving Software Engineering
</p>

<p align="center">
  <a href="https://skyautonet.com/en/">Website</a>
  &nbsp;•&nbsp;
  <a href="https://github.com/SkyAutoNet-lab">GitHub Organization</a>
</p>

---

## About

**SkyAutoNet Autonomous Driving** is the autonomous driving software engineering organization at **SkyAutoNet**.

We develop software and system technologies that integrate **AI, robotics, vehicle control, embedded computing, and intelligent mobility** into reliable autonomous platforms.

Our engineering spans the complete autonomous driving software stack — from sensors and embedded platforms to perception, localization, planning, control, vehicle interfaces, and operator systems.

Our goal is simple:

> **Build autonomous systems that are safe, reliable, and deployable in the real world.**

---

## Engineering Domains

Our autonomous driving software is developed across multiple engineering domains.

| Domain                      | Focus                                                                    |
| --------------------------- | ------------------------------------------------------------------------ |
| **Autonomous Driving**      | Autonomous driving systems and vehicle platform integration              |
| **Perception**              | Camera, LiDAR, radar, object detection, lane detection and sensor fusion |
| **Localization**            | GNSS/RTK, IMU, LiDAR and multi-sensor localization                       |
| **Planning & Control**      | Path planning, trajectory generation and vehicle control                 |
| **Vehicle Control**         | LKAS, longitudinal/lateral control and actuator interfaces               |
| **Vehicle Interface**       | CAN, CAN-FD, ECU communication and vehicle state management              |
| **Linux & Embedded**        | Embedded Linux, kernel and system-level development                      |
| **Sensor & Device Drivers** | Camera, LiDAR, radar and hardware interfaces                             |
| **HMI & Visualization**     | Monitoring, visualization and operator interfaces                        |
| **System Integration**      | Hardware, software and vehicle-level integration                         |

---

## Technology Stack

### Languages

`C/C++` · `Python`

### Robotics & Middleware

`ROS 1` · `ROS 2`

### Computer Vision & AI

`OpenCV` · `CUDA` · `TensorRT`

### NVIDIA Platform

`NVIDIA Jetson`

### Multimedia & UI

`GStreamer` · `Qt` · `QML`

### Build & Deployment

`CMake` · `Docker` · `Git`

### Operating Systems

`Ubuntu` · `Embedded Linux`

---

## Autonomous Driving Software Stack

```text
┌─────────────────────────────────────────────────────────────┐
│                       Applications                          │
│                                                             │
│              HMI · Monitoring · Operations                  │
├─────────────────────────────────────────────────────────────┤
│                  Autonomous Driving                         │
│                                                             │
│   Perception · Localization · Planning · Control · Fusion   │
├─────────────────────────────────────────────────────────────┤
│                       ROS 1 / ROS 2                         │
│                                                             │
│       Nodes · Topics · Services · Actions · TF · DDS        │
├─────────────────────────────────────────────────────────────┤
│                Vehicle & Sensor Interface                   │
│                                                             │
│  Camera · LiDAR · Radar · GNSS · IMU · CAN / CAN-FD        │
├─────────────────────────────────────────────────────────────┤
│                    Embedded Platform                        │
│                                                             │
│ NVIDIA Jetson · CUDA · TensorRT · GStreamer · Linux        │
├─────────────────────────────────────────────────────────────┤
│                      Vehicle / Hardware                     │
│                                                             │
│        Sensors · ECUs · Actuators · Vehicle Platform        │
└─────────────────────────────────────────────────────────────┘
```

---

## Teams & Projects

### Autonomous

Core autonomous driving software and vehicle platform development.

**Repositories**

* [`autoware_common`](https://github.com/SkyAutoNet-lab/autoware_common)
* [`maxen_10x4`](https://github.com/SkyAutoNet-lab/maxen_10x4)
* [`maxen_wingbody`](https://github.com/SkyAutoNet-lab/maxen_wingbody)
* [`skyautonet_common`](https://github.com/SkyAutoNet-lab/skyautonet_common)
* [`skyautonet_autonomous`](https://github.com/SkyAutoNet-lab/skyautonet_autonomous)

**Team:** [`@autonomous`](https://github.com/orgs/SkyAutoNet-lab/teams/autonomous)

---

### Linux Kernel

Embedded Linux and NVIDIA Jetson platform development.

**Repositories**

* [`e-cam25-jetpack6.2.2`](https://github.com/SkyAutoNet-lab/e-cam25-jetpack6.2.2)

**Team:** [`@linux_kernel`](https://github.com/orgs/SkyAutoNet-lab/teams/linux_kernel)

---

### Low-Level Controller

Low-level vehicle control and platform-specific control software.

**Repositories**

* [`low_level_contoller`](https://github.com/SkyAutoNet-lab/low_level_contoller)
* `tata_lkas`

**Team:** [`@low_level_controller`](https://github.com/orgs/SkyAutoNet-lab/teams/low_level_controller)

---

## Vehicle Platforms

Our software is developed and integrated across multiple vehicle platforms.

### MAXEN

* MAXEN 10×4
* MAXEN Wingbody

### Other Platforms

* TATA LKAS
* NVIDIA Jetson-based autonomous driving platforms

---

## Development Workflow

We use a structured Git workflow to maintain stable, traceable and collaborative development.

### Branch Model

```text
main
 │
 │ stable / production-ready
 │
develop
 │
 ├── feature/<name>
 ├── fix/<name>
 │
 └── release/<version>
```

### Branch Naming

| Branch              | Purpose                        |
| ------------------- | ------------------------------ |
| `main`              | Stable / production-ready code |
| `develop`           | Active development             |
| `feature/<name>`    | New feature development        |
| `fix/<name>`        | Bug fixes                      |
| `release/<version>` | Release preparation            |

---

## Engineering Principles

### Safety First

Autonomous driving software operates in real-world environments where reliability matters.

We prioritize:

* Safe failure behavior
* Fault detection and recovery
* Deterministic execution
* Observability
* Reproducibility

### Field-Ready Engineering

Our software is developed not only for research and simulation, but for **integration with real vehicles and operational environments**.

### Modular Architecture

Platform, middleware, perception, localization, planning, control and vehicle interfaces are developed as modular components to enable reuse across different vehicle platforms.

### Performance

Real-time performance is considered throughout the stack — from sensor acquisition and GPU inference to system communication and vehicle control.

### Reproducibility

Development environments, dependencies and deployment configurations should be reproducible across development systems and target platforms.

---

## Repository Organization

Repositories are organized around engineering responsibilities and system boundaries.

```text
SkyAutoNet-lab
│
├── Autonomous Driving
│   ├── autoware_common
│   ├── skyautonet_common
│   ├── skyautonet_autonomous
│   ├── maxen_10x4
│   └── maxen_wingbody
│
├── Vehicle Control
│   ├── low_level_contoller
│   └── tata_lkas
│
└── Platform
    └── e-cam25-jetpack6.2.2
```

Each repository is responsible for a defined component, platform or engineering domain.

---

## Development Standards

### Software

* C/C++ for performance-critical and real-time components
* Python for tools, automation and research workflows
* CMake / colcon for build systems
* ROS 1 / ROS 2 for robotics middleware

### Platform

* Ubuntu-based development environments
* NVIDIA Jetson for edge AI and autonomous driving workloads
* Docker for reproducible environments where appropriate

### Collaboration

* Pull Request-based development
* Code review
* Issue tracking
* Versioned releases
* Team-based repository ownership

---

## Documentation

Each repository should provide documentation covering the following areas where applicable:

```text
README.md
├── Overview
├── Architecture
├── Requirements
├── Dependencies
├── Build & Installation
├── Configuration
├── Usage
├── Development
├── Troubleshooting
└── Release
```

Repository-specific architecture and development information should be maintained close to the codebase.

---

## Private Engineering Organization

All repositories within **SkyAutoNet-lab** are currently private.

This organization serves as the engineering workspace for SkyAutoNet's autonomous driving software development, including:

* Autonomous driving systems
* Perception and sensor fusion
* Localization
* Planning and control
* Vehicle interfaces
* Embedded Linux
* NVIDIA Jetson platforms
* Sensor and device drivers
* HMI and visualization
* Vehicle integration and validation

---

## SkyAutoNet

SkyAutoNet develops **smart mobility safety technologies and autonomous driving systems**.

The company brings together connected, intelligent and autonomous technologies to create safer mobility solutions and autonomous systems for specialized environments.

**Connected · Intelligent · Autonomous**

**Zero-Accident Mobility**

**Make Safety Deployable**

[Visit SkyAutoNet →](https://skyautonet.com/en/)

---

<p align="center">
  <strong>SkyAutoNet Autonomous Driving</strong><br>
  Building safe, reliable, and deployable autonomous mobility systems.
</p>
