# KK2-Drone

# 🚁 Quadcopter Drone Development using KK2.1.5 Flight Controller

![Drone Image](drone.jpg)

## 📌 Project Overview

This project demonstrates the design, assembly, configuration, and testing of a custom-built quadcopter drone using a KK2.1.5 Flight Controller.

The drone was developed to understand UAV systems, flight dynamics, wireless communication, motor control, and embedded electronics. The project involved integrating brushless motors, ESCs, a radio transmitter-receiver system, and a Li-Po battery into a fully functional flying platform.

---

## 🎯 Project Objective

The main objectives of this project were:

- Understand quadcopter architecture
- Learn flight controller configuration
- Study drone flight dynamics
- Implement radio communication
- Control brushless motors using ESCs
- Perform calibration and flight testing
- Gain hands-on experience in UAV development

---

## 🛠 Components Used

| Component | Specification |
|------------|-------------|
| Flight Controller | KK2.1.5 |
| Motors | 1400KV Brushless Motors (4x) |
| ESC | 30A ESC (4x) |
| Frame | F450 Quadcopter Frame |
| Battery | 3300mAh Li-Po Battery |
| Transmitter | FlySky FS-i6 |
| Receiver | FlySky Receiver |
| Propellers | 10x4.5 Propellers |
| Connector | XT60 Connector |
| Power Distribution | Integrated Wiring |

---

## 📷 Project Images

### Drone Assembly

![Drone](images/drone-overview.jpg)

---

## 🏗 System Architecture

```text
FlySky FS-i6 Transmitter
            │
            ▼
      FlySky Receiver
            │
            ▼
   KK2.1.5 Flight Controller
            │
     ┌──────┼──────┐
     ▼      ▼      ▼
   ESC1   ESC2   ESC3   ESC4
     │      │      │      │
     ▼      ▼      ▼      ▼
    M1     M2     M3     M4
```

---

## 🔌 Circuit Connections

### Receiver to KK2.1.5

| Receiver Channel | Flight Controller Input |
|-----------------|------------------------|
| CH1 | Aileron |
| CH2 | Elevator |
| CH3 | Throttle |
| CH4 | Rudder |
| CH5 | AUX |

---

### Flight Controller to ESC

| KK2 Output | ESC |
|------------|------|
| M1 | ESC 1 |
| M2 | ESC 2 |
| M3 | ESC 3 |
| M4 | ESC 4 |

---

### ESC to Motors

Each ESC is connected to one brushless motor.

```text
Battery
   │
   ▼
 ESC
   │
   ▼
Motor
```

---

## ⚙ Working Principle

A quadcopter flies by varying the speed of four motors.

The KK2.1.5 Flight Controller continuously receives commands from the FlySky transmitter and stabilizes the drone using onboard sensors.

### Throttle

Controls altitude by increasing or decreasing motor speed.

### Roll

Moves the drone left or right.

### Pitch

Moves the drone forward or backward.

### Yaw

Rotates the drone clockwise or counterclockwise.

---

## 🧠 How the Flight Controller Works

The KK2.1.5 Flight Controller acts as the brain of the drone.

### Functions

- Reads pilot commands from receiver
- Measures drone orientation using sensors
- Calculates corrections using PID control
- Adjusts motor speed
- Maintains stability during flight

---

## 🚀 Flight Dynamics

For stable flight, opposite motors rotate in opposite directions.

### Motor Rotation Layout

```text
           Front

      M1          M2
      CW          CCW

         QUADCOPTER

      M4          M3
      CCW         CW

            Rear
```

CW = Clockwise

CCW = Counter Clockwise

---

## 🔋 Power Distribution

The 3300mAh Li-Po battery supplies power to all components.

```text
3300mAh Li-Po Battery
            │
            ▼
      Power Distribution
            │
   ┌────────┼────────┐
   ▼        ▼        ▼
 ESC1    ESC2    ESC3    ESC4
   │        │        │        │
   ▼        ▼        ▼        ▼
 Motor1 Motor2 Motor3 Motor4
```

---

## 🏗 Assembly Procedure

### Step 1

Assemble the quadcopter frame.

### Step 2

Mount the four brushless motors.

### Step 3

Install ESCs on each arm.

### Step 4

Mount the KK2.1.5 Flight Controller at the center.

### Step 5

Connect the FlySky receiver.

### Step 6

Wire ESC outputs to the flight controller.

### Step 7

Connect the battery.

### Step 8

Configure and calibrate the KK2.1.5 controller.

### Step 9

Install propellers.

### Step 10

Perform flight testing.

---

## 🧪 Testing and Calibration

### ESC Calibration

- Calibrated all ESCs
- Verified throttle response
- Checked motor synchronization

### Flight Controller Calibration

- Sensor calibration
- Receiver setup
- PID verification

### Flight Testing

- Hover test
- Stability test
- Yaw test
- Pitch test
- Roll test

---

## 💡 Challenges Faced

- ESC calibration
- Motor direction correction
- Flight controller tuning
- Weight balancing
- Receiver binding
- Flight stabilization

---

## 📚 Skills Learned

### UAV Systems

- Drone Architecture
- Flight Dynamics
- Radio Communication

### Electronics

- Power Distribution
- Wiring Integration
- ESC Configuration

### Embedded Systems

- Flight Controller Setup
- Sensor Calibration
- Control Systems

### Testing & Debugging

- Hardware Troubleshooting
- Flight Testing
- System Validation

---

## 📈 Results

✅ Successfully assembled quadcopter drone

✅ Configured KK2.1.5 Flight Controller

✅ Established wireless communication

✅ Achieved stable hover flight

✅ Completed system testing and validation

---

## 🔮 Future Improvements

- GPS Navigation
- Autonomous Flight
- Return-to-Home Feature
- FPV Camera Integration
- Telemetry Monitoring
- Obstacle Avoidance System

---

## 👨‍💻 Author

**Tejas Sanjay Sonone**

Electronics Engineering Student | Drone Enthusiast | UAV Developer

### Areas of Interest

- Drone Development
- Embedded Systems
- Robotics
- Artificial Intelligence
- UAV Technology

---

## ⭐ Project Summary

Designed and developed a custom quadcopter drone using a KK2.1.5 Flight Controller, FlySky FS-i6 radio system, 1400KV brushless motors, ESCs, and a 3300mAh Li-Po battery. Integrated flight control electronics, power systems, and wireless communication modules while performing assembly, calibration, testing, and flight validation. This project strengthened practical skills in UAV systems, embedded electronics, motor control, and flight dynamics.
