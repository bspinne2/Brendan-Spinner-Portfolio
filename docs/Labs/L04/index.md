# Lab 04) Benchmark a Parameter

For this week, our objective is to utilize different 3D printing tests in order to test the limits to which a product fails once being printed. It was our goal to basically test how manufacturable our designs really are. 

## Pick a Parameter

I decided to observe the Overhang Angle Test as my parameter. I utilized the below image as an inspiration for my design.

![Screenshot](./Screenshot%202026-09-15%20115948.png)

The main objective of this test is to see how material overhanging at different angles fails and when it succeeds. It can be taken from this image that the larger the angle between the height dimension of the object and the hypotenuse of the overhang, the more likely the object is to fail. My initial prediction is that the limit will be at the 45 degree angle mark similar to the design above. 

## Design Documentation

When building the design, I wanted it to be unique and original from the inspiration image above. However, one aspect I aimed to replicate was the varying overhang angles showing the progression of the failure. I began by creating a rectangular extrude and began to sketch overhanging ramps on one side of the long face of the block. I noticed quickly that this would be a very bulky block if I simply had the ramps extruding on just one side. It was here I had the idea to create the overhangs on both sides of the block to create a symmetry of the block as well as keeping the printing time to a minimum. 

![Screenshot](./Screenshot%202026-09-10%20135159.png)

This was my rough design of the block. While I was certain I could make it work, I felt as though making the differing angles so close together could make the discrepancies a lot more difficult to recognize. It was here I had the idea to add some spacing between each of the overhangs.

![Screenshot](./Screenshot%202026-09-10%20140231.png)

![Screenshot](./Screenshot%202026-09-10%20140500.png)

After messing around with the spacing and dimensions, I finalized my design of the block. To add a more distinguished factor of my block, I delegated a different thickness for each of the overhangs to conclude how the thickness contributes to the test. 

## Preprocessor 

The next course of action was exporting the design onto PrusaSlicer;

![Screenshot](./Screenshot%202026-09-10%20140728.png)

![Screenshot](./Screenshot%202026-09-10%20140844.png)

I knew that the selected conditions that I chose on PrusaSlicer were incredibly crucial for the outcome of the test. However, I was unsure on whether choosing certain conditions such as brim or higher infill would make the block more secure, and ultimately prevent the blocks ability to fail. It was for this reason that I opted to add only a small perimeter around the block and keep the infill as it is. Little did I know this decision would later bite me in the butt. 

## Printing

It was then time to print my artifact and see if it failed as I expected it to. 
