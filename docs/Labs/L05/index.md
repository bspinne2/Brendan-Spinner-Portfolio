# Lab #5) Design a Snap Fit

The objective of this assignment is to design an object with a snap fit structure, meaning that the two parts connect without the use of any bolts, screws, or adhesives. The snap fit rather utilizes it's friction and pressure designed through its geometry to join the two pieces together. The basis of my design for one of the parts was supposed to resemble a cantilever beam with a transverse load as well as an axial load applied onto it's edge. 

<img width="1260" height="607" alt="Screenshot 2026-09-22 095656" src="https://github.com/user-attachments/assets/b5a8f867-8476-4ff0-874e-4a9b4a93d00c" />


## Initial Planning and Calculations

The first step to designing my parts was to calculate for knowns and unknowns, and utilize what I do know to solve for what we do not know. The instructions for the modeling portion of the assignment can be observed below;

<img width="1335" height="387" alt="Screenshot 2026-09-22 100447" src="https://github.com/user-attachments/assets/145acea8-30f0-4227-b8a5-16da43ebb733" />

Since the material I was to use is PLA, I discovered a common Young's Modulus for the material is 3.5GPa or 507,632 psi. The yield strength was found to be 50 MPa. the safety factor was required to be 3.5. I was then tasked with choosing a magnitude for the axial load and the transverse load within a given range. I chose 8 lbf and 2 lbf respectively. My other calculated values can be observed in my on paper calculations below;

<img width="3024" height="4032" alt="IMG_2999" src="https://github.com/user-attachments/assets/6010bd3a-91c7-4420-9026-2665104527e6" />

When choosing values such as my width and height, I knew this would be a dimension I was bound to have to fix at a later point after observing how the design looks when I put it into CAD. However, for the moment I chose the initial values and went with it. I utilized the max deflection formula to solve for the length for the given width, height and max deflection of the box beam. I initially observed that the calculated length was way too small for a practical use. I then figured I forgot to change my young's modulus to be in terms of psi rather than pascals. After my second attempt, I got a length of 29.39in which was way too long after I imagined the print itself. I knew at this point I needed to start messing around with some of my values. 

<img width="2589" height="3114" alt="IMG_3001" src="https://github.com/user-attachments/assets/9240205e-2e35-49b3-a789-f0286b772f21" />

After looking at my values for a minute, I concluded that my max deflection was a lot larger than I would like it to be. I altered it to be 0.060 inches as I knew the height of my lip was to be smaller than the deflection to prevent permanent deformation. When I recalculated for the length, I got a value of 19.68 inches, which was a better alternative to the 29.39 inches I had before. The next course of action was to manually calculate for whether the stresses caused by the loads of the beams were anywhere near failure given a safety factor of 3.5. I concluded that all of the calculated stresses were well within the safety ranges and were nowhere near reaching failure. 

## Parametric Design

Now that a rough list of my values were solved for, it was time to start actually designing the beam in Solidworks. But before we could start sketching, we were to use parametric modeling to dimension the beam rather than concluded dimensions. This is useful as changing one value or equation in the equation manager will change the rest of the build and allow for more room to adjust the dimensions. I began by adding all the values and equations I calculated for into the equations manager;

<img width="900" height="321" alt="Screenshot 2026-09-21 213448" src="https://github.com/user-attachments/assets/eacc7240-c6aa-47ae-b0b9-ca09ca42a058" />

After my dimensions were assigned parametrically, it was time to start designing the geometry of the bar/beam and observe how the dimensions suit the design. I sketched out the right face of the beam and put in the variables for the length and height.

<img width="957" height="392" alt="Screenshot 2026-09-21 214219" src="https://github.com/user-attachments/assets/e2e93e5e-6a1c-41b0-93d9-7e697c9b5d31" />
<img width="815" height="280" alt="Screenshot 2026-09-21 214600" src="https://github.com/user-attachments/assets/a0740fb7-c488-40c5-86d2-b9d4af36e057" />

Just looking at these initial sketches, I already decided that the length was too long in comparison to the height and that the dimensions need to be a lot more proportional to one another. I decided to recalculate for length by changing the values of the max deflection, height of the lip and overall height of the flexure beam. 

<img width="842" height="261" alt="Screenshot 2026-09-21 215433" src="https://github.com/user-attachments/assets/133556fa-88e1-469e-a07d-f6ed95607d0f" />

The proportionality of these dimensions were a lot more visually sound and resulted in a length of 3.010 inches. This amount was smaller than I would have liked but I was heading in the right direction.

<img width="2850" height="692" alt="IMG_3003" src="https://github.com/user-attachments/assets/3de1ab00-d8fc-4658-912f-d792e34ef52c" />

<img width="875" height="558" alt="Screenshot 2026-09-21 220116" src="https://github.com/user-attachments/assets/706d4371-9856-46e2-b4c2-9a9723d8c696" />

## Holes and Pins of Beam 

While the rough design was heading in the right direction, I discerned that the width of the flexure beam was still way too large and did not look as visually appealing as I would have liked. This is also where I began to plan for the holes and pins that would serve as the conjoining points for the two parts. I added some parametric dimensions for the holes and pins;

<img width="785" height="222" alt="Screenshot 2026-09-21 222251" src="https://github.com/user-attachments/assets/cacdef1f-c578-4ee6-bfd4-fffe1c959748" />

When creating the dimensions for the holes and pins, it was important to not let the holes take up the entire height of the face, and remain as concentric as possible. I decided that for extra support I want to create both holes and pins on both faces that connect into each other like dowels when building furniture. 

<img width="1486" height="695" alt="Screenshot 2026-09-22 000221" src="https://github.com/user-attachments/assets/14167b50-e98d-406d-86c4-d892f77b2f26" />

<img width="992" height="605" alt="Screenshot 2026-09-22 000728" src="https://github.com/user-attachments/assets/72a370cf-b6ee-42ac-bf41-305888ec622f" />

It took me some time to discover how to make the pins mirror evenly on both sides of the hole in the center. I utilized the mirror tool under the linear pattern button to mirror the pins evenly across a plane that divided the beam in half like observed below;

<img width="990" height="520" alt="Screenshot 2026-09-22 001706" src="https://github.com/user-attachments/assets/cfde8f75-42af-4998-8fcf-be97e0321c8a" />

## Adjoining Piece

The next step was to design and sketch the piece that the flexure beam was to affix itself to. The relieving aspect of this part is the limits and restrictions on this part are much less than on the flexure beam. This could be observed by the FBD of the adjoining part in my on-paper calculations. Nonetheless, the parametric modeling of the piece was much shorter than that of the flexure beam.

<img width="782" height="212" alt="image" src="https://github.com/user-attachments/assets/78f37dcf-5d4b-4fba-b69c-5482d8a797a0" />

I then started sketching and messing around with the correct design of the adjoining piece. I gathered that the adjoining area has to be large enough so the pins of the flexure beam could slide in without any unnecessary angling. 

<img width="1067" height="578" alt="Screenshot 2026-09-22 004952" src="https://github.com/user-attachments/assets/fe96d7cc-b421-4a86-bd42-d4f88dca45ec" />

Similarly to the flexure beam, I needed to ensure each of the pins and holes were at an equal distance away to ensure that they will adjoin perfectly to each other without any miscalculations. 

<img width="706" height="663" alt="Screenshot 2026-09-22 094041" src="https://github.com/user-attachments/assets/848fd340-c377-4bf4-a575-53f35652151f" />

<img width="922" height="522" alt="Screenshot 2026-09-22 094756" src="https://github.com/user-attachments/assets/9251e71c-d52b-4cdc-a2c7-703034f1fbd4" />

Since the center pin was exactly in the middle of the face at 0.375 inches across, I ensured the length between the pins and holes for both parts were 0.255 inches. Now that I had parts that fit together in theory, it was time to print the pieces and see if they adjoin as they are intended to. 

## Research

Source - Protolabs Network([https://www.hubs.com/knowledge-base/how-does-part-orientation-affect-3d-print/](url))

The source above describes how the orientation of a part effects several factors of the overall print of the part. The part orientation does not only effect the aspects of the print itself such as build time, but it effects how the overall print of the object turns out. One factor of this impact is described in the article, being the strength of the object. When considering a part under constant load for FDM parts, tensions can create delamination and fractures. This is why it is imperative to create proper part orientation and ensure the dimensions prevent any way that the part could fail. I made sure that my part followed this criteria. 

## Printing

When it was time to print my parts through Prusa Slicer, I knew I would need supports as there were a lot of overhanging areas on both adjoining pieces. A main aspect of a snap fit design is the elasticity of the material so it was important to not over support the print and prevent the parts from maintaining their elastic qualities. 

<img width="866" height="490" alt="Screenshot 2026-09-22 122646" src="https://github.com/user-attachments/assets/f70de6a1-0b81-4f2c-9c86-abe4ab838253" />

<img width="717" height="275" alt="Screenshot 2026-09-22 122655" src="https://github.com/user-attachments/assets/c116e105-a065-4da2-a3bc-6cfa1553f9aa" />

<img width="1305" height="682" alt="Screenshot 2026-09-22 122726" src="https://github.com/user-attachments/assets/bcd54487-eb67-4a2a-b231-0a1427849bd5" />

I decided to add a perimeter of four and to increase the infill density to 20% to increase the overall structural integrity of the part and prevent any part from failing unexpectedly. The supports seemed to be more than satisfactory to prevent any warping with either object.  

It was now time to actually print both objects. When I went to print originally I wasted some time as the printed I attempted to use was not properly loaded with filament so the printer was going through the motions with filament that was not actually there. I went back after this and chose another printer and it printed out just fine. This was my first experience with using supports and peeling them off of the print, so I was very nervous and cautious about messing up the print itself, however it turned out just fine. 

https://github.com/user-attachments/assets/affaa007-b8c7-489d-a7b8-36a70e0e61a4

<img width="3024" height="4032" alt="IMG_3005" src="https://github.com/user-attachments/assets/a355026f-5d4b-4cea-9662-2b1959242d75" />

<img width="3024" height="4032" alt="IMG_3006" src="https://github.com/user-attachments/assets/b2933e8c-330d-4a83-925c-b8953baf8774" />

## Reflection

My build overall printed out just as expected. However, there is many things that I would change about it. For one, the pins were still too large for the holes so they did not go all the way in them. While this was not a huge problem, it hindered the purpose of the pieces to adjoin completely together. Additionally, I would try to find a way that I could increase the size of the build. While it served its purpose, it was a smaller build and could have been made larger. Another thing I could have done differently was incorporate a larger elasticity component within my build that really differentiated my part into a snap fit rather than a normal fit. I was able to bend the pins to fit into the holes, but did not use more more of the elastic component of the PLA material. Overall, this whole process took me about 6-8 hours to complete and was very valuable with learning how snap fits and the designs of them work. 
