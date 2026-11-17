# Final Project – Door Stopper

## Part 1) Define the problem and rough prototype

### Research

**The Spiral Design Process** is an iterative cycle made up of four stages: Planning (defining the goal and measurements), Risk Analysis (spotting potential problems early), Engineering (modeling and building), and Evaluation (testing and gathering feedback). Instead of trying to get everything perfect on the first try, this process helps my project by letting me quickly build a basic door wedge, test it when other doors slam, see if it's too stiff or too loose, and adjust my CAD dimensions for the next version.

**FDM 3D printers** build parts layer-by-layer, which makes them anisotropic—strong along the flat X-Y layers, but much weaker between stacked Z-axis layers. Since my prototype needs a flexible spring arm that bends every time the door closes, printing it upright would cause the layers to split and snap. To prevent this, I will print the spring arm flat on the build plate so the continuous filament strands follow the curve of the flex arm, and use a tougher, more flexible filament like PETG instead of brittle PLA.

**SLA resin printing** cures liquid resin with UV light, which causes the material to shrink slightly (usually around 0.5% to 1.5%) during printing and post-curing. If parts shrink unevenly, tight-fitting joints can warp or fail to snap together. Even though my main design uses FDM and laser cutting, accounting for shrinkage means scaling parts slightly up in CAD, keeping wall thicknesses uniform, and leaving a small clearance gap (around 0.2–0.3 mm) so mating pieces still fit accurately.

**Kerf** is the thin width of material burned away by the laser beam while cutting, which makes outer dimensions slightly smaller and inner holes or slots slightly wider than the CAD drawing. In my prototype, the 3D-printed spring wedge slides into slots on a laser-cut mounting plate, so an uncompensated kerf would make the fit too loose and cause it to rattle. I will measure the exact kerf on a small test cut first and offset my CAD slot dimensions inward by half the kerf width to get a tight, friction-fit joint.

### Problem Definition

**Problem 1: Violent Door Rattling from Air Pressure Waves**
Every time someone opens or closes a door in my house, the other closed doors in the house shake violently against their frames. This happens because standard door latches leave a few millimeters of play between the closed door and the doorframe stop, creating loud rattling noises. A non-damaging, spring-loaded wedge mounted to the frame can fill that gap and stop the shaking without making the door hard to open.

**Problem 2: Phone Charger getting stuck underneath my Mattress**
Quite often when I am working or studying at my desk, I charge my phone simultaneously. During this process, it is very common for the cable to get stuck underneath my mattress and pull my phone onto the floor or for the charging cube to fall out of the outlet and unplug the charging connection.

**Problem 3: Poor Laptop Airflow and Posture on a Flat Desk**
Using my laptop flat on a desk causes neck strain during long work sessions and blocks the bottom cooling vents, making the fans run loud. Basic folding stands tend to wobble while typing and leave charger cables tangled underneath. Combining rigid laser-cut side supports with custom 3D-printed corner grips and rear cable-routing clips would create a sturdy, elevated stand tailored to my laptop.

### Problem Selection

**Selected Problem**: Violent door rattling caused by household air pressure waves whenever another door is opened or closed. This problem fits the class manufacturing tools well because it combines a rigid, flat mounting plate (ideal for the laser cutter) with a custom curved, flexible spring arm (ideal for FDM 3D printing).

**Why & How I Want to Solve It**: The sudden rattling is loud, distracting, and happens constantly throughout the day. Existing adhesive foam strips either wear out quickly or make the door too hard to latch. Instead, I will design a two-part mechanical damper that mounts non-destructively to the doorframe stop using removable adhesive strips. When the door closes, the curved FDM spring arm compresses slightly against the door face to absorb the latch gap and eliminate vibration without requiring extra force to open or close the door.

### Concept Development

<img width="2765" height="2746" alt="IMG_3412" src="https://github.com/user-attachments/assets/8cea3e22-8934-40e1-b202-26ebe861ddd4" />

I generated a rough sketch of my design above that makes the idea of my design easier to visualize. The laser cut bracket will have two parallel, vertical slots that create a freedom of how tight the door movement should be. The goal is to create a 3D printed, flexible spring wedge which press-fit into the laser slots.

**Manufacturing Feasibility**: My goal is to print the FDM spring arm flat on its side in PETG (for flexibility and strong layer adhesion along the curve) with a 2–3 mm wall thickness. I also plan to apply a kerf offset (~0.15 mm) to the laser-cut slots so the 3D-printed tabs fit tightly without wobbling.

### 
