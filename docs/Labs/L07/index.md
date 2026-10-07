# Lab #7 - Linkage Mechanisms

<img width="1387" height="928" alt="Screenshot 2026-10-06 093135" src="https://github.com/user-attachments/assets/a4c3989e-dfef-476f-a4ad-1765f91f6166" />

For this assignment, we are exploring what mechanism and linkages are and how we can design and print a mechanism that demonstrates their effects in 3D printing. A linkage is defined as a set of rigid links connected by pin or sliding joints that transmits motion and force.

## Research

For the research portion, I was tasked with finding two recent mechanisms or linkages and explain how they work and function.

### Compliant four-bar linkage mechanism for a robotic finger

<img width="697" height="507" alt="Screenshot 2026-10-07 102837" src="https://github.com/user-attachments/assets/97dbaa20-8449-47b9-b551-fb78026a686f" />

Source : US20190328550A1 on Google Patents

This medical/bionic prosthetic mechanism explains how four-bar linkage geometry converts actuation cable tension into smooth multi-joint finger bending in prosthetic hands. This can be utilized in the medical field as well the highly prominent robotics industry. 

### Knee joint mechanism without power source for an exoskeleton robot

<img width="655" height="227" alt="Screenshot 2026-10-07 103309" src="https://github.com/user-attachments/assets/be9a0b55-d980-4b74-830b-43b3b738447a" />

Source : US20230181409A1 on Google Patents

The robot part mechanism details of a four-bar linkage knee joint that replicates the human natural pivot center during gait cycles without heavy motor lockups. This can be utilized in the robotics and industrial industries.

### Snap-Fit Connection and Modular Linkage Assembly System

<img width="692" height="532" alt="Screenshot 2026-10-07 103741" src="https://github.com/user-attachments/assets/af18b626-243c-4b9c-96af-91f533fdc926" />

Source : US20030082986A1 in Google Patents

This patent details a mechanical joint system utilizing flexible cantilevered male prongs that deform elastically during insertion into a female pivot hole before snapping back out over a retaining rim. This can be utilized in the toy industry as well as in mechanical construction.

## Design

It was now time to start planning and designing my linkage mechanism. I wanted to design and print something that would be simplistic, but very high functioning with very little design flaws. After researching a little about linkages, I decided I wanted to construct a four-bar linkage that oscillates back and forth with constrained motion. The ability for the design to rock back and forth rather than it being a fixed connection is what makes it a linkage. The purpose was to convert hand-driven rotary input into a constrained rocker arc motion, demonstrating mechanical advantage and zero purchased hardware. This sort of part can be used in advanced mechanical systems or can even be something trivial like a stress or fidget toy. 

### Kinematic Layout

The first step in the planning/design process was to create a kinematic layout plan of the mechanism. 

<img width="825" height="516" alt="Screenshot 2026-10-06 095354" src="https://github.com/user-attachments/assets/f07965f3-36e8-4894-9d20-1b89e5bba2d8" />

<img width="920" height="506" alt="Screenshot 2026-10-06 100336" src="https://github.com/user-attachments/assets/7778612c-4d3e-467b-b41a-fa8b1f086320" />

The geometry and dimensions were randomly picked as I thought 30-80 mm was a good range to have for a print as it would not take a ton of time when it came to print the mechanism. In relation to one another, it was imperative the lengths were not identical, as the range of motion of the oscillation arc would be much less with identical dimensions. I also included a 45 degree fixed dimension angle between the ground(80 mm link) and the input crank arm(35 mm link). This would ensure that changing any dimension later on would not effect the overall geometry of the linkage. To test that the kinematic layout would allow for oscillation movement, I tried to move the arms back and forth and see how they moved. To my surprise, they were not moving how I thought they would. I discovered that during my sketching process the lines of the sketch were vertically constrained so the crank arm and coupler arms were not allowed to move freely as they should. 

### Designing Pins

Now that my rough kinematic sketch was created, the next step was to decide how exactly I want to affix my links together. The instructions of the assignment detail that components can either be printed or purchased, however I wanted to challenge myself. I wanted to try to print all of my components and still have a function linkage mechanism to show for it. Here was a table I created with all of the components that can be observed in my mechanism. 

<img width="866" height="398" alt="Screenshot 2026-10-07 111215" src="https://github.com/user-attachments/assets/c5f37076-e899-4538-8808-b56f87f924f3" />

As observed in the table, I opted to create some snap fit pins similar to the ones I created last week. these pins would keep the links affixed to one another, but have to allow for back and forth movement to occur. 

<img width="977" height="602" alt="Screenshot 2026-10-06 101009" src="https://github.com/user-attachments/assets/cf9e4c55-ad96-48f6-a4d2-e8cb69037571" />

<img width="1290" height="671" alt="Screenshot 2026-10-06 101257" src="https://github.com/user-attachments/assets/b9d69915-a090-402a-bf2c-3d6b209f41ea" />

When creating the rough geometry of the pins, I added a chamfer to allow for the pins to easily fit into the holes of the links. The problem was that my initial design had no overhang that would lock the pins in place from sliding out. I had to compensate for this by making a chamfer that extends out from the main shaft of the pin and sort of catches the top face of one of the links. 

<img width="1357" height="650" alt="Screenshot 2026-10-06 101952" src="https://github.com/user-attachments/assets/ee6059e4-150f-4bf7-8bd0-29ba9e77b81f" />

<img width="923" height="615" alt="Screenshot 2026-10-06 102301" src="https://github.com/user-attachments/assets/1ecd76fc-17a0-428d-a068-c9a958852ab8" />

The final component of the pin that was immensely important to add is the slot in the middle of the pin that allows the pin to elastically bend to fit into the interlocking links. Without the slot, the pins would be a rigid body and would not embrace their elastic properties. 

<img width="842" height="561" alt="Screenshot 2026-10-06 102619" src="https://github.com/user-attachments/assets/2ad44f90-4fa6-4cd0-a86c-f663f5d982e3" />

It was difficult to arrive at exact dimensions for my slot, so I decided to create a datum to ensure that the pins remained symmetric and even. 

<img width="758" height="680" alt="Screenshot 2026-10-06 103239" src="https://github.com/user-attachments/assets/9a302a3a-379e-4e79-a49b-476a29b0e477" />

<img width="556" height="496" alt="Screenshot 2026-10-06 103411" src="https://github.com/user-attachments/assets/22432a76-af87-4792-966f-15b194c7c391" />

Overall, the pins look effective and satisfactory. 
