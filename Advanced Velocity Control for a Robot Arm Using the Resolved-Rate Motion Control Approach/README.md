# Advanced Velocity Control for a Robot Arm Using the Resolved-Rate Motion Control Approach

**Institution:** Imperial College London  
**Collaboration:** MathWorks Advanced Research & Technology Office  
**Supervisor:** Dr. Giordano Scarciotti  
**MathWorks Mentors:** Roberto G. Valenti, George Amarantidis, Rory Adams  

---

## Project Overview
This project develops an **advanced velocity-based motion control framework** for the UR5 robotic manipulator using the **Resolved-Rate Motion Control (RRMC)** approach in MATLAB Simulink.  
The work addresses **instability issues near kinematic singularities** by implementing both the **Moore–Penrose pseudoinverse (MP)** and **Damped Least Squares (DLS)** methods for inverse kinematics.

Key objectives:  
- Enable **smooth, accurate trajectory tracking** for redundant manipulators.  
- Provide a **modular, reusable Simulink framework** adaptable to industrial and research applications.  
- Benchmark **MP vs DLS** to evaluate robustness near singularities.  

---

## Repository Structure
Advanced-Velocity-Control-RRMC/
│

├─ Simulink_Model/ # Main Simulink implementation
│ └─ Integration.slx
│
├─ Report/ # Project documentation
│ ├─ Chen_Guan-Sheng_[EXTERNAL]_MathWorks_Project.pdf
│ └─ Chen_Guan-Sheng_Poster.pdf
│
├─ Figures/ (optional) # Key plots, diagrams, and simulation results
│
└─ README.md # Project description


---

## Features
- **Trajectory Generation** with trapezoidal velocity profiles.  
- **Forward & Inverse Differential Kinematics** for task ↔ joint mapping.  
- **Inverse Kinematics Methods:**
  - Moore–Penrose pseudoinverse (MP)  
  - Damped Least Squares (DLS) with tunable damping factor λ  
- **Joint-Space PID Control** converting desired velocities into torque commands.  
- **Safety Layers**: rate limiters, velocity & torque saturation for hardware transfer.  

---

## Key Results
- **DLS outperforms MP** near singularities with stable trajectory execution.  
- Achieved **sub-centimeter end-effector accuracy** in simulation.  
- Identified optimal **λ ≈ 0.03** for robustness vs accuracy trade-off.  
- Developed **grouped Kp allocation** strategy for smoother multi-axis motion.  

---

## Technical Stack
- **Tools:** MATLAB Simulink, Robotics System Toolbox, Simulation 3D  
- **Methods:** RRMC, DLS Inverse Kinematics, PID Control  
- **Robot:** UR5 Manipulator (simulated in 3D environment)  

---

## Files
- **Integration.slx** – Full Simulink implementation of the RRMC framework.  
- **Chen_Guan-Sheng_[EXTERNAL]_MathWorks_Project.pdf** – Technical project report.  
- **Chen_Guan-Sheng_Poster.pdf** – Project poster presentation.  

---

## Applications
- **Industrial Robotics & Smart Manufacturing**  
- **Rehabilitation & Assistive Robotics**  
- **Education & Research in Control Systems**  

---
