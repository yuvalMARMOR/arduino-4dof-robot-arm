# Arduino 4DOF Robot Arm Project

A complete Arduino-based control system for a 4 Degrees of Freedom (4DOF) robotic arm with joystick control and position memory capabilities.

## 📋 Project Overview

This project demonstrates progressive development of a robotic arm control system, from basic servo testing to advanced features like pose memory and automated sequences.

**Note:** This project began with assembling the mechanical arm, then progressively developing the control software.

## 🎯 Features

- **Basic servo control and testing**
- **Dual analog joystick control** for precise movement
- **Position memory system** - save and recall arm poses
- **Automated sequences** - loop through multiple saved positions
- **Modular code structure** for easy learning and modification

## 📁 Project Structure
```
arduino-4dof-robot-arm/
├── hardware_tests/      # Initial hardware calibration and testing
├── basic_programs/      # Fundamental servo control programs
├── joystick_control/    # Joystick input and control implementations
└── memory_programs/     # Advanced features with position saving
```

## 🔧 Hardware Requirements

- Arduino board (Uno/Mega recommended)
- 4DOF robotic arm mechanical kit
- 4x Servo motors (180° range)
- 2x Analog joysticks (X/Y axes)
- External power supply for servos (5-6V, adequate current)
- Jumper wires and breadboard

## 📚 Code Files Description

### Hardware Tests
- **Code_for_0_Servo.ino** - Test servo at 0° position
- **Code_for_80_Servo.ino** - Test servo at 80° position
- **Code_for_180_Servo.ino** - Test servo at 180° position

### Basic Programs
- **servo_basic_test.ino** - Simple servo movement test
- **servo_control.ino** - Basic servo control implementation

### Joystick Control
- **read_joystick_values.ino** - Read and display joystick input values
- **dual_joystick_control.ino** - Control robot arm with dual joysticks

### Memory Programs
- **memory_single_pose.ino** - Save and recall a single arm position
- **memory_multiple_poses.ino** - Save and recall multiple positions
- **memory_with_loop.ino** - Automated playback of saved sequences

## 🚀 Getting Started

1. **Mechanical Assembly**
   - Assemble the 4DOF arm 
   - Ensure all joints move freely
   - Attach servos securely to each joint

2. **Hardware Setup**
   - Connect servos to Arduino PWM pins
   - Connect joysticks to analog input pins
   - Ensure proper power supply for servos

3. **Software Setup**
   - Install Arduino IDE
   - Load desired program from appropriate folder
   - Configure pin numbers if needed

4. **Testing Progression**
   - Start with `hardware_tests/` to verify servo operation
   - Move to `basic_programs/` for simple control
   - Try `joystick_control/` for manual operation
   - Explore `memory_programs/` for advanced features

## 🎓 Learning Path

This project is organized to support progressive learning:

1. **Assembly** → Build the mechanical structure
2. **Calibration** → Test individual servo positions
3. **Basic Control** → Learn servo movement programming
4. **User Input** → Implement joystick control
5. **Advanced Features** → Add memory and automation

## ⚙️ Pin Configuration

Typical pin setup (verify in each sketch):
- Servos: Digital pins 3, 5, 6, 9
- Joystick 1: A0 (X), A1 (Y)
- Joystick 2: A2 (X), A3 (Y)

## 📝 Notes

- Always power servos from external supply, not Arduino
- Calibrate servo angles for your specific hardware
- Start with low servo speeds when testing
- Use Serial Monitor for debugging (9600 baud)
- Ensure mechanical assembly is solid before running code

## 🔄 Future Improvements

Potential enhancements:
- [ ] Add speed control for smoother movements
- [ ] Implement inverse kinematics
- [ ] Add wireless control (Bluetooth/WiFi)
- [ ] Create GUI interface for position programming


## 📄 License

This project is open source and available for educational purposes.

## 🤝 Contributing

Feel free to fork this project and submit pull requests for improvements!

---
