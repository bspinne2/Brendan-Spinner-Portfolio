# Lab #9) Laser Cutter

Brendan Spinner & Ethan Minton

## Objective

Our objective was to measure, record, design, laser cut, assemble, and document a parametric construction kit using Taguchi’s Robust Design principles. We were to utilize repeatable joint connections that account for measured kerf and material thickness variation across an entire sheet.

## Analysis

### Determining Sheet Thickness

Ethan and I recognized that we had to utilize a 1in by 1 in square to measure the recorded kerf, so we decided to take a shortcut and use the cut out square to measure the sheet thickness as well. We used a digital caliper rather than a mechanical one to avoid any human error or inaccuracies that may have come with it. 

<img width="851" height="637" alt="Screenshot 2026-11-02 141532" src="https://github.com/user-attachments/assets/b045e530-85a1-42e4-9bb5-7821b403eacf" />

However, we did decided to switch to do the final measurements on the sheet itself to reduce any changes that a cut could make to the sheet and its thickness.

<img width="323" height="392" alt="Screenshot 2026-11-02 141735" src="https://github.com/user-attachments/assets/0e9bee26-3ddc-428c-8bee-6401c39354f9" />

To find the average, we add these measured values and divide by 5. This gives us a thickness of 0.1072 inches, which we will use when creating our CAD model and determining certain constraints.

### Finding the Kerf

Kerf is the measured value that is erased or cut out during the process of laser cutting. The best way to evaluate this value is measure the before and after dimensions of a block to analyze how much was really taken away. This is the process that Ethan and I did to begin to determine what fit we would use for our design. We began by creating a quick 1 inch by 1 inch sketch in Inkscape that would be able to laser cut the print and grab our measurements with the true sides.

<img width="850" height="503" alt="Screenshot 2026-11-02 142156" src="https://github.com/user-attachments/assets/13bb9457-e280-4993-ae9f-f4ca63aa205f" />

When getting to the actual cutting process of the square block, we needed the help of a couple of the lab assistances to help with connecting to the print. Setting up the print itself was a lot more challenging and difficult than the print itself. I was definitely shocked with how quickly it cut out the piece. 

<img width="860" height="484" alt="image" src="https://github.com/user-attachments/assets/957f4ce7-c252-4fb0-af8a-abe9a5a5db71" />
https://github.com/user-attachments/assets/85034c2d-c6f7-4c07-b778-f15f9fbc84d0

The measured values for the nominal 1 inch by 1 inch square were 0.9965 inches for the x-axis and 0.9950 inches for the y-axis. Subtracting these from the nominal values and averaging them gives us a calculated Kerf of roughly 0.00425 inches. This value will be utilized when designing the tolerance and our clearance test.

<img width="857" height="637" alt="Screenshot 2026-11-02 143034" src="https://github.com/user-attachments/assets/9fd20a95-7026-48c6-982c-451c0081291c" />

<img width="853" height="637" alt="Screenshot 2026-11-02 143043" src="https://github.com/user-attachments/assets/40f3b575-cbf3-4406-aff8-e3cb86d22260" />

<img width="691" height="226" alt="Screenshot 2026-11-02 143121" src="https://github.com/user-attachments/assets/1062555f-0157-419e-95ee-f272ecd3b206" />

As noted by the table, our mean kerf was about 0.00425in.

### Determining Clearance

When designing the clearance test, We were told by a lab volunteer it would be best to use Fusion 360 over SolidWorks as the CAD software as it has minimal issues with sending DXF files over to Inkscape, which I was nervous about as I am not super familiar with Fusion360. Luckily, my partner Ethan was a little more used to using it.

We began by creating a simple sketch on the front surface. Next we created 5 equally spaced slits between each of the protrusions that were each set to be 0.30 inches wide, with them all being equalized with the equal constraint. They were also set to a height of 0.70 inches to allow for proper grip ability and easy insertion. I started with the middle constraint, setting it just to our thickness value of 0.1072 inches.

<img width="1911" height="961" alt="image" src="https://github.com/user-attachments/assets/f56eafe5-0a0c-436a-a4d6-2d7c2fc143ba" />

We then went to the right of the center and added a single increment of the kerf measured value.

<img width="1911" height="963" alt="image" src="https://github.com/user-attachments/assets/881b5166-2141-46ed-bd11-e05d1bee72d8" />

Then at the edge we then added the thickness to be 2 times the kerf value. This was specifically to ensure a better base line to check if I need smoother or longer values for my tolerances. These 2 tabs represent the loose fits.

<img width="1912" height="962" alt="image" src="https://github.com/user-attachments/assets/8449cd63-bc42-4749-b296-61bc0c1dd736" />

We did the same process on the left side, but instead of adding increments of the kerf value, we decided to subtract increments on this side to represent the tighter fits. This results in the completed Tolerance Test Model below.

<img width="1911" height="962" alt="image" src="https://github.com/user-attachments/assets/e32d9d84-9714-4b03-b0ea-7ff4c8047740" />

Before we uploaded the file to Inkscape, some of our peers told us to make the fits to test a slot fit. We did this by adding a rectangular sketch to the top of the design, as you can see below. All other dimensions remained the same.

<img width="1917" height="966" alt="image" src="https://github.com/user-attachments/assets/4c2ecc47-4ee9-4cdb-937d-dac94c5d068c" />

Below is the parametric table we used for this process with the kerf having a measurement of 0.00425 inches, and the thickness being set to 0.1072 inches.

<img width="1498" height="592" alt="image" src="https://github.com/user-attachments/assets/4a1f644a-e64e-4976-9de2-1418051d3394" />

We then uploaded the file with a DXF file into Inkscape so that the file could be cut.

<img width="1917" height="1137" alt="image" src="https://github.com/user-attachments/assets/dd6c8ed4-ecd2-4ad1-9d0b-555f54284e0d" />

Below is a video of the cutting for the clearance test;

<img width="860" height="484" alt="image" src="https://github.com/user-attachments/assets/44470206-ac91-47ca-a72a-0872a42bf40b" />
https://github.com/user-attachments/assets/e8d18941-5655-46ba-84d5-ab8c84648247

After we finishing cutting and began analyzing what fit worked the best we recorded that 1 kerf was too loose of a clearance and that 2 kerf was too tight a clearance. Because of this, we picked dimenions roughly 1.5 kerfs to accomodate the needed clearance.

## Designing

When creating the inspiration for our design, we wanted to create something simplistic, practical yet efficient. 

We began by creating a sketch on the top surface and set the length to "LENGTH2," which was set to 4.50 inches and set the width to "WIDTH" which was set to 0.60 inches.

<img width="1916" height="967" alt="image" src="https://github.com/user-attachments/assets/d1fe46a7-c274-4c28-91ad-aea06bee11bd" />
<img width="1911" height="963" alt="image" src="https://github.com/user-attachments/assets/4b061e98-f9d4-45f0-9328-45172607f964" />

We then created 2 rectangles on the interior of the sketch and equalized their side lengths to each other to ensure that any change in the model will parametrically affect the other. These rectangles would be the slot fits that connect the pieces to each other.

<img width="1915" height="967" alt="image" src="https://github.com/user-attachments/assets/751a01f9-1fd9-48cf-9907-a279e13dbc5d" />

We then constrained the top of these rectangles with "(WIDTH/2) - (KERF + CLEARANCE)". We included the clearance variable so that any alterations We had to make on Monday could be easily added to the model without directly changing the "KERF" variable. This currently has resulted in a length of 0.296 inches.

<img width="1907" height="965" alt="image" src="https://github.com/user-attachments/assets/8195bc10-0538-4a65-bce7-fe49dd08a32e" />

We then constrained the height of the smaller rectangles using "THICKNESS - (KERF + CLEARANCE)" for the same reasons. This equates to a value of roughly 0.103 inches.

<img width="1916" height="952" alt="image" src="https://github.com/user-attachments/assets/ca65b222-4d87-4967-bbae-60e07728c77a" />

Next, we constrained each of their lengths from the opposing side to be "LENGTH1" or 4 inches.

<img width="1915" height="960" alt="image" src="https://github.com/user-attachments/assets/338a5cb4-9bd7-4a4e-b9f8-c43853b6a61a" />

Then we aligned the smaller rectangles to the center of the main rectangle, utilizing the collinear constraint.

<img width="1912" height="957" alt="image" src="https://github.com/user-attachments/assets/57342735-b0c5-4c16-8221-c520e43d7dd1" />

This was the end of the first shape. We began creating the second shape with a "LENGTH1" value of 4 inches.

<img width="1915" height="962" alt="image" src="https://github.com/user-attachments/assets/86fd6d38-333a-46b5-80a4-ca94c5efc043" />

Once the first shape was complete, it was very easy to build the others as we just based the dimensions of the following pieces on the first piece. We did a lot of messing around with the dimensions to ensure all the fits reached each other and fit snug. 

After finishing the design, we printed and cut it with the laser cutter just as we did with the kerf test.

<img width="1917" height="1140" alt="image" src="https://github.com/user-attachments/assets/6dc48df4-854e-4d2b-97bb-c8f341889574" />

<img width="1917" height="1130" alt="image" src="https://github.com/user-attachments/assets/d6817b6e-13b2-412d-a41b-191acac4def0" />

After laser cutting, we assembled the pieces together as best as we could.

<img width="3024" height="4032" alt="IMG_3284" src="https://github.com/user-attachments/assets/33bdb448-496b-4a02-bcb6-e22dd552aefb" />

While we accomplished our rough geometry of our design, the fits were rather lose and did not attain the practical pen holder application that we had planned. To fix this, we decided to increase the clearance by 0.001 inch, which by itself seems rather trivial, but managed to completely fix our design and its efficiency.

## Lessons Learned

### Process Log
* **Total Time:** 5.5 hours total( 1.5 hours analysis, 3 hours designing and 1 hour reflection/documentation).

### Mistakes, Troubleshooting, and Modifications
* **Initial Fit Issue:** Upon initial laser cutting and assembly, the overall 3D pen holder geometry was successfully created, but the interlocking tab-and-slot fits were overly loose, preventing the assembly from holding pens securely.
* **Troubleshooting & CAD Parametrics:** We reviewed our parametric model where slot width was governed by `THICKNESS - (KERF + CLEARANCE)`. With a measured kerf of 0.00425" and nominal thickness of 0.1072", the clearance was producing excess play.
* **Design Modification:** We adjusted the CAD model by increasing the clearance parameter by 0.001", effectively tightening the interlocking slots. This small change eliminated wobble and restored full structural stability and functional efficiency.

### Resources Used
* **Material:** 1 sheet of 1/8 inch laser-cut plywood
* **Tools & Consumables:** CO2 laser cutter and digital calipers for parametric tolerance measurements

### Reflection Prompts

1. **Measured vs. Assumed Values:** Real sheet thickness varied from nominal values, and our baseline kerf assumption initially allowed too much play in the slots. If we had strictly relied on unadjusted assumed values without modifying clearance, the structure would remain too loose to function as a stable pen holder.
2. **Taguchi's Quality Loss Function Analysis:** While the current interlocking joints work, they deviate slightly from an ideal friction-fit target. Under Taguchi's model, any deviation from target quality incurs a financial loss; produced at scale, this variance would cause inconsistent customer assembly quality, higher return rates, and lower product reliability.
3. **Real-World Product Example:** Flat-pack furniture and sheet metal enclosures use similar tab-and-slot joints. For customers, kerf or thickness errors show up as joints that are either impossible to assemble without damaging parts (too tight) or structurally weak and prone to rattling (too loose).
4. **Future Design Iterations:** If granted one additional test cut, we would micro-adjust the slot clearance down by another 0.0005" to achieve a perfect, tool-free press fit that firmly locks the frame together without needing glue.




