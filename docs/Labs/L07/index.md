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

<img width="740" height="250" alt="Screenshot 2026-10-07 113242" src="https://github.com/user-attachments/assets/87a213f4-f6da-4931-a87d-a8152f1d1e58" />

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

### Creating the Links

The next course of action was creating the four links of the mechanism. These would be the bodies that are adjoining together actually performing the back-and-forth oscillation movement of the linkage. I utilized the straight-slot tool to create the base of the links. I then created circular cuts to serve as the holes the pins would snap into. 

<img width="787" height="563" alt="Screenshot 2026-10-06 112817" src="https://github.com/user-attachments/assets/5ddf2a15-2e32-4a9f-92ea-6ede2ef1f9a6" />

<img width="1051" height="645" alt="Screenshot 2026-10-06 113339" src="https://github.com/user-attachments/assets/46ae9738-6bca-4174-b1c5-9ca619f13a0f" />

<img width="800" height="412" alt="Screenshot 2026-10-06 113645" src="https://github.com/user-attachments/assets/a46b9386-57ea-4693-a077-54eb51bbb5a5" />

This part was relatively simple as I was creating four pretty much identical parts where the only big difference was the differing lengths that were proportional with the kinematic model.

### Creating an Assembly/Affixing the Parts

For a good conceptual understanding of what the linkage mechanism should look like when the pins and links are connected, I decided to make an assembly in CAD that portrays the freedom of movement in the kinematic model.

The big trick with ensuring the links lined up accurately was the mate tool. To accomplish this task I made each overlapping hole of the links concentric with the link it was to connect to, and made the respective top and bottom faces of the links coincident so that there was no space between them. 

<img width="1340" height="641" alt="Screenshot 2026-10-06 114906" src="https://github.com/user-attachments/assets/619fbff3-b4fe-4704-a3b1-7ad660e53866" />

<img width="1438" height="761" alt="Screenshot 2026-10-06 120240" src="https://github.com/user-attachments/assets/2c8d7f60-583f-4220-a8e8-4f9d8dea993c" />

<img width="1036" height="662" alt="Screenshot 2026-10-06 120717" src="https://github.com/user-attachments/assets/ce6091d2-782e-458e-9091-2d3154651a00" />

After the links were all properly aligned with each other, the next step was to add the pins to the assembly. This step was relatively simple. I mated the exterior surface of the shaft of the pin to the interior surface of the respective holes. This was the finished product of this.

<img width="1421" height="635" alt="Screenshot 2026-10-06 120914" src="https://github.com/user-attachments/assets/dec8d82b-b025-4b53-b8ea-3c6d9dc254fb" />

<img width="1130" height="645" alt="Screenshot 2026-10-06 121101" src="https://github.com/user-attachments/assets/08fe8e68-ca70-4f48-a748-92b5fb4ab3f9" />

### Reflecting on Design

Throughout the links and pins, there were some tolerance and clearance decisions I decided on in order to ensure the mechanism was not rigid and worked indeed as a linkage as intended to. One of these choices was I made the hole diameters of the links 5.4mm while I kept the pin shaft diameter at 5.0mm. This was to allow a smooth rotation and prevent any joint stoppage. I also added a  0.30mm undercut on the cantilever pin head to flex through the hole and snap securely over the top link face. This allowed me to have some room to work with in terms of how tightly the pins fit into the links. 

Some design decision that I went with when designing the mechanism included choosing snap-fit pins rather than M3 screws to affix my links, choosing a 6mm arm thickness to prevent twisting or lateral flexing under movement, and printing horizontally so shear force does not snap pins along layer lines.

## 3D print 

Now it was time to print my linkage mechanism through Prusa slicer. Despite creating an assembly of all the pieces connected together, keeping them like that to print would significantly increase the print time of the build, so I decided to reseparate them so that they all lay flat and close together. 

<img width="1162" height="796" alt="Screenshot 2026-10-06 124535" src="https://github.com/user-attachments/assets/bf264b8d-c313-4493-aacb-01b19b91e973" />

<img width="880" height="490" alt="Screenshot 2026-10-06 124755" src="https://github.com/user-attachments/assets/68fb5947-c8dd-49b6-8df2-ecb9ea793468" />

<img width="601" height="168" alt="Screenshot 2026-10-12 173033" src="https://github.com/user-attachments/assets/674055e5-2ae2-4b97-85b1-4603e9591394" />

<img width="1886" height="1027" alt="Screenshot 2026-10-06 135429" src="https://github.com/user-attachments/assets/e6c30549-3d41-4575-bb0f-718d044d20a0" />

I chose to maintain a lot of the parameters for the slice. One I did choose to alter was the number of perimeters to 3 as increasing perimeters strengthens the eyes surrounding the holes so they don't fracture when snap-pins are pressed in. I also kept the Elephant foot compensation to 0.20 mm as this slightly trims the very first layer outline, preventing the bottom edge of my pivot holes from flaring out and binding against the pin heads.

I sliced the design and began to print;

<img width="3024" height="4032" alt="IMG_3095" src="https://github.com/user-attachments/assets/0fa04c11-a867-4094-8571-607d052ed350" />

https://github.com/user-attachments/assets/18809eed-ba67-4e28-8b94-ed1631ade683

<img width="3024" height="4032" alt="IMG_3097" src="https://github.com/user-attachments/assets/dc5125f7-c3a6-4ed8-89d5-d0a2886470d1" />

https://github.com/user-attachments/assets/409eb5c1-2116-4ae7-8388-fa99fbfd3733

Overall, the linkage mechanism was a success! The fits were a little loose, largely do to the clearances I applied to the links. If I want to make it a little tighter I would probably decrease the holes size to 5.2mm diameter rather than 5.4mm diameter, so I would definitely fix that. On the bright side, the pins fit perfectly and do not slide out at all. The oscillation movement of the links is beyond satisfactory. 

## Lessons Learned

The project required approximately 6 hours total broken down into 0.5 hours of patent research, 2 hours of SolidWorks CAD modeling, 0.5 hours of slicing, 1 hour of printing on the Prusa Core One, and 2 hours for post-processing and physical assembly. The most significant error occurred during CAD assembly when mate constraints failed because exported multi-body links defaulted to "Fixed" status; this was identified via SolidWorks rebuild warnings and resolved by setting the moving links to "Float". The 0.4mm designed clearance  worked successfully on the first print, though tightening the holes by an additional 0.1 to 0.2mm would compensate even better a tighter and less loose linkage movements that still oscillates, but feels a little more sturdy. 







