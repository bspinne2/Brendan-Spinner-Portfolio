# Lab 10) RC2 Sliding Fit Design and Verification

This week's assignment was to SLA print an RC 2 sliding fit. This print is different than all of my past prints as it uses a more advanced 3D printer which utilizes more expensive resin rather than filament. 

<img width="1495" height="792" alt="Screenshot 2026-11-11 133309" src="https://github.com/user-attachments/assets/a4007518-253f-4a8c-a525-89a5478fd231" />

## Research & Planning

The ASME RC 2 (Sliding Fit) is designed for accurate location of mating parts where sliding motion is required without noticeable play. According to the Machinery’s Handbook, RC 2 fits maintain tight alignment with slightly greater maximum clearance than an RC 1 fit, allowing parts to move and turn easily under light loads. For this assignment, the utilization of clearances are ever so important as a slightly tighter clearance can reduce the ability for the fit to slide with ease. On the contrary, too loose of a clearance prevents the parts from being able to mate efficiently.

The clearance limits given by the ASME/Machinery's Handbook for nominal size are as followed:

Minimum Clearance (Cmin): [e.g., +0.005 mm]

Maximum Clearance (Cmax): [e.g., +0.020 mm]

Hole Tolerance Zone: [e.g., +0.012 mm / -0.000 mm]

Shaft Tolerance Zone: [e.g., -0.005 mm / -0.015 mm]

Considering Real-life applications, RC 2 fits are widely used in precision engineering components, including locating pins in manufacturing jigs/fixtures, low-speed control levers, alignment dowels, telescoping assemblies, and sliding gear selectors.

SLA resins undergo volumetric shrinkage (typically 1%–3%) during light-curing and post-curing. To compensate for this, it is important to expand hole and shaft features by a small clearance of between 0.03mm to 0.05mm.

When designing my mating parts, I got the idea for this part from precision tools like drill press depth stops and router tables. I wanted to design a sliding plunger pin with a top thumb knob and an adjustable stop collar. Using an RC 2 sliding fit makes sure the pin glides smoothly without wobbling, giving me repeatable control over the depth.

<img width="2547" height="3084" alt="IMG_3286" src="https://github.com/user-attachments/assets/12b2d395-9e92-412f-9365-e2739cef06c1" />

<img width="2433" height="2940" alt="IMG_3285 (1)" src="https://github.com/user-attachments/assets/0344e982-f70d-4a27-b4ea-6817dc5b866c" />

These were my rough sketches for my mating features.

## CAD Design

I started the design by parametrically modeling the dimensions for both the shaft and the bore components. 

<img width="768" height="141" alt="Screenshot 2026-11-03 103326" src="https://github.com/user-attachments/assets/2734fc9a-8982-46fe-9b58-b512cabdd1b8" />

### Bore Design

I then began to design the bore part of the fit;

<img width="641" height="582" alt="Screenshot 2026-11-03 103725" src="https://github.com/user-attachments/assets/0008b3cc-8419-45f3-a846-42e88a078d7f" />

<img width="762" height="553" alt="Screenshot 2026-11-03 103811" src="https://github.com/user-attachments/assets/3e311e1f-a04b-4f83-bb72-aae042ec53e1" /><img width="1272" height="725" alt="Screenshot 2026-11-03 105322" src="https://github.com/user-attachments/assets/6f30015b-aa61-4bc7-9a3c-4f2e637ad190" />

<img width="635" height="562" alt="Screenshot 2026-11-03 104234" src="https://github.com/user-attachments/assets/94891c7c-964a-46d8-850c-8bc8b06dfb05" />

I utilized the opinion of artificial intelligence to give me an estimate on what the magnitude of each of the dimensions should be. I created an open slot on one of the side faces of the bore to serve as a measurement feature after curing is done on the shaft. A digital caliper can be inserted in the open gap to record the diameter of the shaft. 

<img width="621" height="582" alt="Screenshot 2026-11-03 104457" src="https://github.com/user-attachments/assets/9010187c-caa5-4297-b8d7-de3bbbd46de2" />

I hollowed out the interior of the bore in order to reduce the overall material. This reduces cost and print time of the overall print.

<img width="650" height="492" alt="Screenshot 2026-11-03 104704" src="https://github.com/user-attachments/assets/299cf605-9bde-4b00-9f9c-2ea1822a9b54" />

<img width="857" height="627" alt="Screenshot 2026-11-03 104814" src="https://github.com/user-attachments/assets/12fa0b7e-eb9c-41fd-8a4a-aefb33cb6675" />

<img width="862" height="730" alt="Screenshot 2026-11-03 105842" src="https://github.com/user-attachments/assets/b69e2750-aebc-404c-b824-5d3e5f335eaa" />

### Shaft Design

When designing the shaft of the fit, it was crucial to design the main cylinder that mates with the bore to fit accurately with a perfect enough clearance to represent a true RC 2 sliding fit. a 0.05mm tolerances was used for diameter dimension.

<img width="832" height="705" alt="Screenshot 2026-11-03 110325" src="https://github.com/user-attachments/assets/df3f6c75-3c62-4458-b891-0fa5a432fb8d" />

I added a stopper element on the shaft to prevent any friction on the interior cut of the bore. 

<img width="518" height="696" alt="Screenshot 2026-11-03 110505" src="https://github.com/user-attachments/assets/55ffa58c-48a3-4d81-86fa-29ac7af27b48" />

The knob at the top serves as the part where the force is applied axially to the shaft.

<img width="707" height="557" alt="Screenshot 2026-11-03 110601" src="https://github.com/user-attachments/assets/9a200d89-dd12-47c8-a65a-1a0276b57374" />

<img width="720" height="511" alt="Screenshot 2026-11-03 110704" src="https://github.com/user-attachments/assets/c5daa7f4-9647-4247-a0e4-774da320de09" />

<img width="748" height="737" alt="Screenshot 2026-11-03 110949" src="https://github.com/user-attachments/assets/96eec0de-035f-4fd1-8e2e-d72f05f15647" />

Now that the main designs are complete, the next step is to test the amount of material in each of the features.

<img width="487" height="612" alt="Screenshot 2026-11-03 111335" src="https://github.com/user-attachments/assets/023f4af1-62d3-4937-b9a9-6f50eddc4cc3" />

<img width="483" height="590" alt="Screenshot 2026-11-03 111357" src="https://github.com/user-attachments/assets/7916b1d5-c212-4e74-9b25-e8ef7786665a" />

The total volume is equal to roughly 1.0522 cubic inches, which translates to about 17 milliliters. This satisfies the 20mL limit we were given.

## Preprocessing

Now that I had two features, I exported them into .step files and uploaded them into the Preform platform. This is the setup process that exports the CAD design into the printing procedure. 

<img width="1152" height="996" alt="Screenshot 2026-11-03 125919" src="https://github.com/user-attachments/assets/5e37d641-4a22-439f-b236-58d86d925b77" />

<img width="1902" height="1020" alt="Screenshot 2026-11-03 124346" src="https://github.com/user-attachments/assets/aecf6a3d-cb7f-4348-be77-b2e2b2d69bce" />

I utilized the auto-click feature which automatically set up supports for the two features. I then received assistance from one of the lab techs to help me print it. However, I ran into an issue where based on my geometry, printing would result in a build up of resin that would not be able to escape. 

I fixed this by adding small holes throughout the bore and shaft which allowed the liquid resin to leave. 

<img width="673" height="743" alt="Screenshot 2026-11-03 111435" src="https://github.com/user-attachments/assets/290ef536-2516-40bd-8b36-5689731c5a8c" />

<img width="387" height="661" alt="Screenshot 2026-11-03 123202" src="https://github.com/user-attachments/assets/d42632fd-be6e-44af-b26c-130805946456" />

<img width="991" height="737" alt="Screenshot 2026-11-03 123747" src="https://github.com/user-attachments/assets/e9ddad2c-065d-4d02-bafd-23e113dcbe68" />

This fixed the issue and gave me the okay to print.

## Printing

<img width="3024" height="4032" alt="IMG_3288" src="https://github.com/user-attachments/assets/84493079-d2fe-4cf0-a4e9-b6c7451e408f" />

The total print time for this fit was much larger than I had anticipated. I scaled down the size to 0.6 times the original to reduce the printing time from 2 hours to roughly 1 hour. The total volume reduced to about 14.2 mL. Once the print was complete, I put the building platform directly into the alcohol bath. The bath took about 5 minutes to complete.

## Post Processing

After pulling off all the support and polishing the finish, this was my final result;

<img width="3024" height="4032" alt="IMG_3289" src="https://github.com/user-attachments/assets/6bdaf0e4-e0a3-406e-8721-9b25263b0c0a" />

<img width="3024" height="4032" alt="IMG_3290" src="https://github.com/user-attachments/assets/4a73cfe6-2d8e-42ff-889a-80625ee7ca4b" />







