# Engineering in Motion: Parallax QTI Line-Follower Robot

## 📌 Project Overview
This project showcases the design and implementation of a **line-following robot** using the **Parallax Boe-Bot platform** and **QTI infrared sensors**.  
The robot was engineered to detect and follow electrical tape tracks by processing real-time sensor input and executing adaptive movement routines.

Through this project, I demonstrated skills in **electronics, embedded programming, control logic, and problem-solving** while pushing my motivation to achieve more than the basic requirements.

## 📂 Contents of This Presentation
[Presentation PDF](Final%20Presentation.pdf)

## 🤖 Preview
[Line Follower Demo](./assets/0830.gif)

## ⚙️ Technical Implementation

### Hardware
- **Base Platform**: Parallax Boe-Bot  
- **Sensors**: QTI infrared emitter/receiver modules (x4)  
- **Custom Setup**:  
  - Adjustable sensor spacing for optimal line detection.  
  - Mounted with spacers and standoffs for stability.  
  - Tuned for ~¾ inch black electrical tape on a white background.

### Software
- **Language**: PBASIC (BASIC Stamp 2)  
- **Core Subroutines**:  
  - `Check_Qtis` → Reads sensor states (black = 1, white = 0).  
  - `LineFollowWithCheckQtis` → Implements control logic for movement.  
  - `Gosub Spin` → Handles edge-case turns.  

### Logic
- Developed **conditional loops** to interpret sensor states.  
- Created special handling for the **1–1 case** (when both middle sensors detect the line).  
- Implemented **curve, pivot, and rotate commands** for smooth navigation.  


## 🏆 Achievements

- **Functional Success**
  - Robot successfully followed lines on multiple course shapes (S-curves, intersections, closed loops).  
  - Stable performance after troubleshooting sensor spacing and turning logic.
 
- **Extra Challenges Completed**
  - Phototransistor separated into an independent conditional loop.  
  - Implemented **closed-loop 360° rotation** using knowledge from prior assessments.  

- **Performance Gains**
  - Initial runs were slow to avoid sensor misreads → **185 seconds**.  
  - After code and sensor optimization → **49 seconds** fast run.  


## 🛠 Troubleshooting Process

1. **Sensor Positioning**
   - Began with narrow spacing → too sensitive to small deviations.  
   - Widened spacing → allowed more room for corrections without losing the line.  

2. **Handling the 1–1 Case**
   - Turning off the axis of the wheels or chassis caused drift.  
   - Corrected to ensure turning was **aligned with the sensors**, keeping the robot on track.  

3. **Code Refinement**
   - Simplified conditions for faster loop execution.  
   - Balanced servo pulse widths for smoother left/right adjustments.  


## 🚀 Motivation & Reflection

This project represents more than just a line-following robot:
- It demonstrates **practical application of engineering concepts** (sensors, feedback loops, control systems).  
- It reflects **problem-solving resilience**, adapting when initial solutions failed.  
- It shows **curiosity and drive** to go beyond the minimum requirements and explore advanced challenges.  

By completing this project, I strengthened my foundation in robotics and confirmed my motivation to pursue **more advanced autonomous systems and engineering projects**.

##  For Me
This line-follower robot is both a **technical achievement** and a **personal milestone** in my engineering journey.  
It highlights my skills in **design, coding, testing, and iteration**, and—most importantly—my **motivation to keep building and learning**.
