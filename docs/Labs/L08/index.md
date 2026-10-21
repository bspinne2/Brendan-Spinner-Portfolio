# Lab 8) Design and Print Something Useful

## Reading & Writing

Given the article, asking smarter questions is essential for optimal communication and understanding between human beings. Specifically in design processes, asking investigative questions that truly question the why of the design process are very important to the greater understanding of what the design is intended for. While asking questions can seem to be a hindrance for designers as they may waste time, the time spent on asking such questions is rather well spent as a lack of information about the design process can lead to resources and even more time to be squandered in the process. Utilizing smart questions so that they empower both the design asking the questions as well as the ones being asked are the most effective as they allow for a deeper analysis into what can create success for both parties rather than hyper focusing on the failures that one or the other may have created. This not only builds team chemistry but allows for greater success with making a design to be satisfactory for all parties involved. 

## Purpose of Design

This projects prompts me to solve a problem with a design that is exclusive to me. I first read this prompt in the car on the way to class, and immediately I located something I could fix. My father had recently got me a dashcam for my brand new car, and to prevent the cord from getting in the way of the windshield, I taped the cord to the edges of the windshield. The tape made it look low effort and unappealing, so I decided to change this. 

<img width="3024" height="4032" alt="IMG_3196" src="https://github.com/user-attachments/assets/1cfc53bc-9a13-4913-a418-420ce5c54b1a" />

The rough idea of the design would be some sort of snap fit or clip that would hold the wire itself, and then a blade that would tuck into between the fabric and glass of the windshield and be held together by the compressive forces of the two materials. If designed correctly, this could be used for any person with a car and has a dash cam cord or LED cord that gets in the way of their vision when driving. This was my very rough sketch for my design:

<img width="3024" height="4032" alt="IMG_3208" src="https://github.com/user-attachments/assets/df71c411-cb94-484f-b21d-de5f04931f82" />

The design itself is rather basic as there is not many components at all to it. The hardest part of the design itself I imagine would be the geometry itself.

## Designing in CAD

Now that I had developed a rough idea of what I wanted to create, the next step was to build the geometry in SolidWorks. I began by parametrically designing dimensions so that the geometry was easier to adjust if any dimensional errors arise. 

<img width="925" height="411" alt="Screenshot 2026-10-19 231848" src="https://github.com/user-attachments/assets/0a2a526d-0767-433f-b6d9-9b3b0d96157e" />

After I attributed dimensions, I began constructing the geometry for the clip. I had to ensure that the clip was big enough to hold the wire and fit into the seam, but also that it was small enough to make it appealing to look at. The parametric dimensions were educated guesses of what would be good dimensions with guidance from Artificial intelligence. I decided to add some clearance for the diameter of the clip so that the wire would comfortably sit inside of it and fit in nicely and with little effort. 

<img width="667" height="482" alt="Screenshot 2026-10-19 230706" src="https://github.com/user-attachments/assets/e516ab1b-1dad-4988-8b81-8cca20a13775" />

<img width="1082" height="512" alt="Screenshot 2026-10-20 000923" src="https://github.com/user-attachments/assets/f8ebb3df-4a03-4960-ba71-398bbc0cc7a9" />

<img width="940" height="357" alt="Screenshot 2026-10-20 001032" src="https://github.com/user-attachments/assets/647dfbfa-641d-4b54-ae1d-04164ec8c1b2" />

I began by trying to offset the line geometry in order to create the thickness of the blade. I began by creating two separate sketches, one for the clip and one for the tuck-in blade. The issue I encountered with this was that the two sketches would not merge. The worry was that they would not adjoin or merge together like I had hoped. To fix this, I decided to make one sketch geometry that I could extrude to ensure that they were one solid geometry. I trimmed the merging arc of the clip that connects to the blade so that the two components merge together. 

<img width="800" height="447" alt="Screenshot 2026-10-20 004516" src="https://github.com/user-attachments/assets/56ae40b0-3ea7-4951-b39b-373ea78f1fee" />

<img width="637" height="565" alt="Screenshot 2026-10-20 005121" src="https://github.com/user-attachments/assets/1eba4b0c-0997-44da-8e73-c46ae4fd63c0" />

<img width="1007" height="532" alt="Screenshot 2026-10-20 005502" src="https://github.com/user-attachments/assets/31fc6b2a-f8da-46bc-bcb4-18637a2685f4" />

<img width="911" height="377" alt="Screenshot 2026-10-20 005844" src="https://github.com/user-attachments/assets/ac97ebfb-40ab-40a9-b825-66b69e8bd653" />

<img width="891" height="483" alt="Screenshot 2026-10-20 010033" src="https://github.com/user-attachments/assets/57f7c99c-46db-4353-bcdc-ec422bf4fd89" />

Now that the geometry was merged together, I extruded the sketch to create the final design for the clips. 

<img width="1011" height="561" alt="Screenshot 2026-10-20 121347" src="https://github.com/user-attachments/assets/7489d9cc-9b3e-4096-a09f-72ce9e9d6ec7" />

<img width="1002" height="582" alt="Screenshot 2026-10-20 121548" src="https://github.com/user-attachments/assets/b9fb307f-af7e-4925-b68c-af23a9ae1bfe" />

I created some chamfers at the sharp edges to avoid any cutting of the wires as well as any unwanted stress points. 

<img width="912" height="588" alt="Screenshot 2026-10-20 121634" src="https://github.com/user-attachments/assets/b5e5addb-dcac-47a9-98da-32a0344c47aa" />

## Printing

Overall, given how small and simplistic my design was, I did not need a lot of printing settings when I added the design into Prusa Slicer. I did add 3 to 4 perimeters to make the build solid rather than hollow. I also made sure to make the printing material to PETG as it does not melt under the sun and deform like PLA does. 

<img width="1122" height="297" alt="Screenshot 2026-10-20 122054" src="https://github.com/user-attachments/assets/5ed35df3-12ac-4e47-ad18-f119e5a8928c" />

<img width="1731" height="711" alt="Screenshot 2026-10-20 122102" src="https://github.com/user-attachments/assets/e3893b4d-a9a7-4930-a7a9-69ec66845dcf" />

I sliced the design and began to print. The printing time was rather short, only 8 mins as the clips were small, even though I decided to print five of them. There were no issues with the printing itself. 

https://github.com/user-attachments/assets/3b79760f-9ec3-44b7-995e-4b656b03306a

<img width="3024" height="4032" alt="IMG_3210" src="https://github.com/user-attachments/assets/ef46dfcc-477b-4e2b-95ee-60233b8de08c" />

After the print was finished, I scraped off the print from the pad. During the process, I did break off some of the blade on two of the clips. Luckily, the purpose functioned the same and ended up serving its purpose.

<img width="4032" height="3024" alt="IMG_3211" src="https://github.com/user-attachments/assets/9d4939ca-74eb-4b50-a5e3-337dc7a2d71d" />

<img width="3024" height="4032" alt="IMG_3212" src="https://github.com/user-attachments/assets/7c1d043a-d791-4b1a-9659-440c7c4f16ee" />

## Lessons Learned

Overall, this process took about three to four hours for the design, printing, and documentation of the design. I learned a lot about fixing a problem during this process. I am very satisfied with the finakl result and am proud with how useful my design is proving to be. I additionally learned more about designing in CAD, how to separate entities, trim entities, and merge different components together. 


