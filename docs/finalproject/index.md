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

**Video Of Problem** : [![Final Project - Problem Explanation](https://img.youtube.com/vi/brH7joig8qw/hqdefault.jpg)](https://www.youtube.com/watch?v=brH7joig8qw)


### Concept Development

<img width="2765" height="2746" alt="IMG_3412" src="https://github.com/user-attachments/assets/8cea3e22-8934-40e1-b202-26ebe861ddd4" />

I generated a rough sketch of my design above that makes the idea of my design easier to visualize. The laser cut bracket will have two parallel, vertical slots that create a freedom of how tight the door movement should be. The goal is to create a 3D printed, flexible spring wedge which press-fit into the laser slots.

**Manufacturing Feasibility**: My goal is to print the FDM spring arm flat on its side in PETG (for flexibility and strong layer adhesion along the curve) with a 2–3 mm wall thickness. I also plan to apply a kerf offset (~0.15 mm) to the laser-cut slots so the 3D-printed tabs fit tightly without wobbling.

### Designing my Prototypes

#### Laser-Cut Bracket

Designing this feature was very easy and simplistic. I simply created a small rectangular sketch with two slots and equal distance away from the center of the rectangle. I made sure to account for clearance so that when my mating male part slides in effortlessly.

<img width="1048" height="661" alt="Screenshot 2026-11-17 115757" src="https://github.com/user-attachments/assets/4b3fb5f9-35d2-4412-a812-495f99d7fa7a" />

I exported this simple sketch into Epilogue and grabbed a 3mm thick piece of plywood. 

<img width="476" height="486" alt="Screenshot 2026-11-17 151114" src="https://github.com/user-attachments/assets/fc7e63d9-d792-4262-af12-cec080b1df82" />

The first cut for some reason did not cut all the way through, however I simply recut it and it came out perfectly.

<img width="3024" height="4032" alt="IMG_3413" src="https://github.com/user-attachments/assets/0dac98fc-c995-45bd-bd96-21ddc6510b14" />

#### 3D-Printed Wedge

Creating the geometry for this wedge only contained a few steps, especially considering that this would be a rough prototype for my final project.

<img width="760" height="117" alt="Screenshot 2026-11-24 001609" src="https://github.com/user-attachments/assets/fa8377ff-13a5-47e7-828c-0f606776f0a2" />

I began by parametrically designing the dimensions of the printed block to how I thought they would best fit with the already laser cut bracket. I kept the thickness of the beam to be only 3mm to account for the 3.2mm thickness of the bracket slot.

<img width="1263" height="803" alt="Screenshot 2026-11-17 120437" src="https://github.com/user-attachments/assets/5377a1cb-996d-4007-a1f7-7144c597f761" />

<img width="897" height="732" alt="Screenshot 2026-11-17 120832" src="https://github.com/user-attachments/assets/37672569-4fa7-4311-a75c-6289330b003c" />

I began with a 25mm long rectangle that matches the dimensions of the bracket so that they are relatively similar in size and so the printed wedge does not extend past the bracket itself in practice.

<img width="965" height="757" alt="Screenshot 2026-11-17 121149" src="https://github.com/user-attachments/assets/203b3c65-fe6d-4c3f-aaf4-198eee07825d" />

After extruding the base piece of the wedge, it was time to create the beams that adjoin into the slotted bracket.

<img width="772" height="812" alt="Screenshot 2026-11-17 121914" src="https://github.com/user-attachments/assets/3e150084-98b0-41a4-81e7-8e8ca62c3f1f" />

<img width="901" height="852" alt="Screenshot 2026-11-17 122020" src="https://github.com/user-attachments/assets/7308cf1c-fd09-46ad-b4e4-1df0b2937777" />

Now the initial rough design of my wedge was complete and it was time to print it out.

https://github.com/user-attachments/assets/158b476b-8166-47a3-a631-ccf171f15c79

<img width="4032" height="3024" alt="IMG_3439" src="https://github.com/user-attachments/assets/cde54b65-8ffd-4237-a21e-e9e937fbc787" />

<img width="4032" height="3024" alt="IMG_3440" src="https://github.com/user-attachments/assets/21d93c1c-1999-40a3-8aed-1cb508b45e98" />

<img width="4032" height="3024" alt="IMG_3441" src="https://github.com/user-attachments/assets/fd677d85-a248-46af-a606-410f50d462c3" />

After printing out the first copy of the wedge, it was very evident that I incorrectly dimensioned the distance between beams in relation to the distance between the slots on the bracket. Additionally, looking at the prototype, I gathered that having the beams extend across the entire wedge would be more optimal for a tighter fit.

### Peer Review 

After my rough plan and prototypes were complete, it was time to gather into groups and discuss my path forward and reflect on my work thus far.

My team members for this peer review were Atiba and Randy. Here are their peer review worksheets based off of my initial pitch.

<img width="2735" height="3168" alt="IMG_3464" src="https://github.com/user-attachments/assets/6caaff5d-351d-47c1-a110-a8877f372a27" />

<img width="2959" height="1905" alt="IMG_3465" src="https://github.com/user-attachments/assets/d7edbf22-92ff-4885-b20e-ac924974f48e" />

<img width="2687" height="2703" alt="IMG_3466" src="https://github.com/user-attachments/assets/b477275f-6326-43a2-af2e-64d1409c0a74" />

<img width="2994" height="1599" alt="IMG_3467" src="https://github.com/user-attachments/assets/b2f03d08-a7f3-40bf-9d55-3ccfdb7d1561" />

Both Atiba and Randy stated how they liked the originality of my project idea and were very optimistic about the practicality of my concept working as planned. They specifically emphasized how they liked the simplicity of my idea, and how I used the laser printer rather than the SLA printer. We discussed that my biggest obstacle would be ensuring that the right tolerances were implemented so that no other adhesive is required to keep the part intact and so that it is sufficient and does its job. Overall, my peer feedback was really helpful and reassuring for me to continue with my idea and enhance my project. 

## Part 2) Enhance the Prototype

### Fixing the Wedge

Based off my observations after the first print of the wedge, my next step was to go back and redesign my wedge to fit accurately with bracket.

<img width="762" height="127" alt="Screenshot 2026-11-24 011214" src="https://github.com/user-attachments/assets/25e6a9de-c9d9-49b6-9caa-2b25be773f9b" />

<img width="1411" height="997" alt="Screenshot 2026-11-24 011010" src="https://github.com/user-attachments/assets/4d5f05a0-9c91-4da6-ad81-a37801c07c0f" />

This time, I changed the overall thickness of the part from 20mm to 21mm. This ensures that the beam align evenly this time with the slots as they were not aligned correctly during the first print. I also changed the beam length so that it goes across the entire height of the wedge and is almost identical to its mating slot.

After fixing these simple things, I went to print and record how the two pieces affixed to one another.

#### Second Attempt Results & Observations

<img width="3024" height="4032" alt="IMG_3442" src="https://github.com/user-attachments/assets/aaf4a61f-d183-4045-8854-cf7a9649aaa2" />

<img width="3024" height="4032" alt="IMG_3443" src="https://github.com/user-attachments/assets/bc149672-d24a-4e34-af1c-972aa4b82d80" />

<img width="3024" height="4032" alt="IMG_3444" src="https://github.com/user-attachments/assets/15bd14c2-d45c-4ea7-9df5-bcee03b8a608" />

As can be observed from the pictures above, while this print was a lot closer to fitting into the slotted bracket, there was an evident printing error that made snapping into place difficult. I found out that having my print orientation on the side caused issues for my print as there was nothing for the top beam to layer on top of. My fix to this was to use a new build orientation.

#### Third Attempt Results & Observations

<img width="721" height="167" alt="Screenshot 2026-11-20 122237" src="https://github.com/user-attachments/assets/cbd4d0c5-2be2-431a-8258-d2ab65ddd342" />

<img width="856" height="361" alt="Screenshot 2026-11-20 122245" src="https://github.com/user-attachments/assets/ca8a6c2b-4e72-425a-bca4-a57cbe707f81" />

<img width="673" height="252" alt="Screenshot 2026-11-20 122254" src="https://github.com/user-attachments/assets/c775a927-d37d-419b-b6e8-f6122afa5b82" />

<img width="1902" height="946" alt="Screenshot 2026-11-20 142102" src="https://github.com/user-attachments/assets/378b9248-ecf6-4e8a-9766-ef7247720ae0" />

I did not fix any of the dimensions before reprinting, I simply rearranged the build orientation to be as it appears above.

<img width="3024" height="4032" alt="IMG_3445" src="https://github.com/user-attachments/assets/544e40d8-96a0-4061-98a0-571a8ebe5cbd" />

This was my reprinted wedge design. There was no printing issues with this print and the mating pieces joined together pretty well.

### Testing its Efficiency

Now that both of my parts for this project are sufficient enough, it is time to analyze how well it works.

<img width="3024" height="4032" alt="IMG_3468" src="https://github.com/user-attachments/assets/849fb013-f3b1-404b-9698-18d43337c7be" />

The picture above represents how the build is oriented in the door frame itself. The laser cut bracket is wedged in the crevasse between the door and the frame itself and that friction force is heavily responsible for the part staying steady and not succumbing to the affects of gravity. The tighter the clearance the plywood has between the frame and the door, the more resulting force that is pushed back against the door when the vibrations occur. I decided to implement this important utilization of clearances rather than using some other adhesive, command strip or screw to keep the door stopper afloat. This method is also the easiest method to implement and the most appealing to look at as command strips and screws can be quite the eye sore. 

**Video of Stopper working as intended** : [![Final Project - Testing Design](https://img.youtube.com/vi/yi7aH6xnD5M/hqdefault.jpg)](https://www.youtube.com/watch?v=yi7aH6xnD5M)

### Google Slide Presentation

[SoDe Final Project - Door Stopper.pdf](https://github.com/user-attachments/files/35350081/SoDe.Final.Project.-.Door.Stopper.pdf)

### Final Video Summary

[![Summary Video](https://img.youtube.com/vi/hFO7_BGBJk0/hqdefault.jpg)](https://www.youtube.com/watch?v=hFO7_BGBJk0)
