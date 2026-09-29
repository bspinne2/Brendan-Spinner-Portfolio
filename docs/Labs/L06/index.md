# A6 – Design Fits for an Artifact

For this week's assignment, I was tasked with designing a snap fit part that affixes itself to an object chosen from a bag of objects used in engineering. The instructions for the assignment is listed as follows;

<img width="1355" height="831" alt="Screenshot 2026-09-28 103953" src="https://github.com/user-attachments/assets/7e67234f-16a3-4f73-9578-df864fbf40bf" />

## Planning/Recording Dimensions

Before I can begin to design my design fit for my chosen artifact, I need to firstly analyze what my artifact is and what dimensions it inhibits. I chose a small, red PCB(Printed Circuit Board) as my artifact. The PCB has two holes on either side of it, inferably intended for mechanical fastening. The board also has 7 solder joints on one side of the board and their pin ends exposed on the flatter side of the PCB.

<img width="3024" height="4032" alt="IMG_3048" src="https://github.com/user-attachments/assets/1fd2fea2-2a1d-4c74-9bcc-a0ec6538f803" />

The next step was to begin dimensioning the PCB using a caliper provided in class. Measuring using a caliper allows for an enhanced precision of each of the dimensions that hopefully leads to minimal room for error when it comes to designing in the CAD software. Below are dimensions of the PCB recorded by the caliper.

<img width="2882" height="1776" alt="IMG_3049" src="https://github.com/user-attachments/assets/339d4602-cfad-4a17-b686-d7a702ed3b50" />

## Research

Now that I measured some basic information about the circuit board, the next step was planning the snap fit itself and how it would affix itself to the PCB. I had some rough ideas in my head, however I wanted some visual inspiration for the design fits. I found one that to go off of on printables;

<img width="1491" height="596" alt="Screenshot 2026-09-28 102649" src="https://github.com/user-attachments/assets/6dca0415-9ac1-48ad-9614-d356eddaf6f7" />

I really liked the idea of making the snap fit into a PCB mount as it adds a practical purpose the fit that extends outside of the assignment criteria. One thing that can be observed from the inspiration design is that claw clips are utilized to snap into the underneath of the board which holds it together. Instead of using triangular clips, I really liked the idea of having cylindrical clips that connect to the holes of the PCB board. I believe this will make my design overall look clean, deliberate and unique. 

## Parametric Design

As critical as planning and research is to the design process, I am aware how valuable trial and error can be when it comes to designing an object. In many cases, just because something looks to be viable on paper does not translate to it printing without failures. I implemented this trial and error process a lot over the course of this assignment. Parametric modeling was immensely beneficial to making sure that dimensions were neatly assigned so that way when I come across one of these mistakes, I was able to fix a few components and not have to scrap the entire design. My initial parametric model was as shown:

<img width="766" height="175" alt="Screenshot 2026-09-28 225521" src="https://github.com/user-attachments/assets/9b23eaad-6182-4020-9425-b26ca9c352fc" />
### Creating Base
It is with these dimensions that I started to create a rough base for my PCB mount. 

<img width="968" height="618" alt="Screenshot 2026-09-28 230113" src="https://github.com/user-attachments/assets/3a7acb4c-ac61-4063-8061-6a4cc41c442b" />

<img width="1461" height="648" alt="Screenshot 2026-09-28 230132" src="https://github.com/user-attachments/assets/0a9946bb-7cb5-44b5-b180-bba6b3971556" />

It was here where I encountered my first obstacle. Each of the solder joints have metal node-looking stubs on the under side of the PCB preventing me from simply having a flat base. My initial idea was to create a cutout for the stubs to go into. My concern with this idea was that it would reduce the material thickness which significantly effects the integrity of the mount.

<img width="1492" height="727" alt="Screenshot 2026-09-28 232439" src="https://github.com/user-attachments/assets/1904d89c-81bf-4675-b8dc-cfcfd9637525" />
### Creating Standoffs

It was here where I had the idea to create two standoffs where each of the holes are located on the PCB that keep the base as a flat surface that is not effected by the underneath stubs of the solder joints. I updated my parametric modeling and continued with my design including the standoffs. 

<img width="761" height="230" alt="Screenshot 2026-09-28 232610" src="https://github.com/user-attachments/assets/53b66248-5282-488d-9607-a90de7f5eeea" />

<img width="1346" height="601" alt="Screenshot 2026-09-28 233248" src="https://github.com/user-attachments/assets/4f6d38dd-de61-4a54-91b7-6cc802ebe220" />

<img width="1071" height="666" alt="Screenshot 2026-09-28 233406" src="https://github.com/user-attachments/assets/a4e9030f-101a-4c24-8a0a-7be36eadf3d0" />

<img width="1217" height="448" alt="Screenshot 2026-09-28 233442" src="https://github.com/user-attachments/assets/c8e33e40-0274-4cbf-a99a-60f9ab278c27" />

### Creating Pins

Now that I solved the problem of the stub interference, the next step was to figure out how exactly this design was going to snap fit into the PCB. I already decided that i wanted to try something different than clips on the edges, so I figured why not create pins that snap directly into the holes already present on the PCB? I decided to go forward with this idea.

<img width="1431" height="651" alt="Screenshot 2026-09-28 234926" src="https://github.com/user-attachments/assets/95ccf552-72d9-441c-9668-dc30d0dc2886" />

<img width="1386" height="417" alt="Screenshot 2026-09-28 235004" src="https://github.com/user-attachments/assets/947c4f82-0458-4597-bead-180f609177ea" />

### Creating Overhang/lip

Now that I have the pins at a good set of dimensions, the next step is to create some sort of lip that prevents the pin from slipping out from the hole. I figured that some sort of lip or overhang with a chamfer was the best course of action forward. 

<img width="1246" height="600" alt="Screenshot 2026-09-28 235729" src="https://github.com/user-attachments/assets/f486e7d9-9088-4df8-b5d0-9c9566b8016e" />

<img width="1403" height="608" alt="Screenshot 2026-09-28 235804" src="https://github.com/user-attachments/assets/742a1786-091f-4b7f-816a-6d98a39c00b2" />

<img width="1083" height="620" alt="Screenshot 2026-09-29 000120" src="https://github.com/user-attachments/assets/2416cba4-1242-4ad4-9a59-3ad17160ea43" />

### Creating Cutout

After I applied the chamfer to the lip, the initial design for the snap fit system was pretty much complete. The final step was to give the pin room to elastically deform to fit into the hole. With the solid structure of the pin and lip as it is, the material would not be able to bend enough to fit and would not function as a snap fit. To fix this, I created a rectangular cut on each pin to give it this flexibility. 

<img width="765" height="67" alt="Screenshot 2026-09-29 000348" src="https://github.com/user-attachments/assets/36b7eaf2-1943-4478-bb8a-6341ee777320" />

<img width="1446" height="537" alt="Screenshot 2026-09-29 001150" src="https://github.com/user-attachments/assets/3a2ee47b-ac46-4787-805e-693eaeab693f" />

<img width="1052" height="740" alt="Screenshot 2026-09-29 001924" src="https://github.com/user-attachments/assets/81ce60b2-3db6-426c-b016-b1046d64dec0" />

### Creating Mounting Holes

Now that the snap fit mechanism was fully functional in theory, it was time to add a unique and practical purpose to my design. I wanted to create mounting holes on either side of the PCB where somebody could affix it to something else. 

<img width="767" height="122" alt="Screenshot 2026-09-29 165259" src="https://github.com/user-attachments/assets/fc52b1ed-f9a7-47f6-854c-2313e6193427" />

<img width="1107" height="562" alt="Screenshot 2026-09-29 002817" src="https://github.com/user-attachments/assets/610617bb-e3c6-4b7c-99ba-70dbd9b5b4a0" />

<img width="1182" height="477" alt="Screenshot 2026-09-29 003707" src="https://github.com/user-attachments/assets/560f60a5-5847-4bce-83f7-9bdbee8cf568" />

<img width="1026" height="667" alt="Screenshot 2026-09-29 004450" src="https://github.com/user-attachments/assets/3a07c106-541d-4eed-9998-a759d150baff" />

## First Print

Now that I had my completed design, it was time to start adding some parameters and get ready to print. I decided to increase the perimeters to 4 to ensure the vertical prongs were 100% solid wall loops to maximize the tensile strength, ensuring the clips spring back instead of breaking. I also decided have 4 top layers and 4 bottom layers to ensure that the base plate and the top of the standoffs were completely sealed. I did not want to over constrain with parameters, so that was the extent of parameters I used. 

<img width="857" height="498" alt="Screenshot 2026-09-29 123353" src="https://github.com/user-attachments/assets/68999b3d-8705-4b1b-8908-cdd7b264c8ec" />

<img width="1901" height="707" alt="Screenshot 2026-09-29 130431" src="https://github.com/user-attachments/assets/cab8197a-411f-42ea-96ef-4e1b89ed93c9" />

