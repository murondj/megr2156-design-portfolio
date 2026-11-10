# A10 – Lead Screw Translating System

## Objectives


## Analyze
This week's assignment is a group assignment. The goal is to design and build a mechanically driven tester that is capable of applying **2 KN** of axial tensile load, and be able to have a controllable crosshead speed of **1 to 50 mm/min**. 

## Decide

### Leadscrew Diameter: Greyson Boatright
#### Lead screw diameter using axial stress
I found the minimum lead screw diameter with the assumption that we were going to analyze the screw under axial stress only. In this analysis I used the given parameters of a safety factor of four and a total force of 2kn in the resulting equation. Since the two lead screws were identical and the force was distributed evenly between the two, this meant I could divide the total force by two and analyze only one lead screw. The material from the catalog online only gave options for steel and stainless steel which meant I had to make an assumption for the yield strength I was going to use to effectively calculate the allowable stress. Using steel set the yield strength to 250MPa, I solved the equation for the minimum diameter to be 4.5297mm. Lastly I went through the catalog with the number that had to achieve the minor(root) diameter for the lead screw, I chose a 3/8-16 right handed steel screw temporarily as there was still more analysis to be done.

<img src="gb-4.png" alt="initial design" width="400">

#### Range of rotational speed
The next step was to calculate the range of rotational speed we could achieve with a given range of linear speed. The linear speed that was given was a range of 1 to 50 mm/min. We needed to convert this linear speed to rotational speed, to do this we could divide the speed over the lead. Luckily I was able to easily figure out the lead size as it was given to me through the manufacture of the temporary lead screw. After drawing the free body diagram, identifying knowns and unknowns, I was able to write equations for both the minimum and maximum RPMs, those came out to be 0.625-31.246 and I found that to be a reasonable rotational speed range for what we are trying to achieve.

<img src="gb-5.png" alt="initial design" width="400">

#### Lead screw based on max torque
The last analysis of the lead screw diameter was to find out what the maximum torque would be. I drew a free body diagram of the lead screw and the only unknown in this problem was the torque. With the help of my machineries handbook on page 2647 in the lead screw section there is a formula that goes over how to calculate torque in a lead screw. The formula was T=(PxL)/2pi*e, the formula from the book gave e in English standard and I found e to be 0.25 because I knew we were going to be using a bronze nut. I did have to convert my values into English standard so I could numerically solve and convert back to metric units. The result after algebraically solving and plugging in the values and converting back came out to be 1,018.72 N*mm and I was satisfied with the reult.

<img src="gb-1.png" alt="initial design" width="400">
<img src="gb-6.png" alt="initial design" width="400">

#### Lead screw selection
Overall the analysis of the temporarily chosen lead screw was sufficient and I decided to further continue with my initially chosen lead screw. I eventually went back to where I determined the diameter based upon axial stress and wrote down some key information about the dimensions and part number from the website. In addition to that I took a screenshot of the lead screw straight from the website and embedded it below for visual aid.

<img src="gb-2.png" alt="initial design" width="400">

### Selecting a Nut & Flange: Greyson Boatright

#### Selecting the nut/flange based upon thread bending stress analysis
A key part of this assignment is to ensure that the nut and flange we chose for the given lead screw is able to withstand the conditions in which it is put under. For this portion I analyzed the internal threads of the nut due to bending stress. For the knowns of this problem we continued using a safety factor of 4, we only analyze one nut since it is symmetric and that gives us a force of 1kn compared to 2kn. I also knew the minimum diameter of the nut which I based on the major diameter of the lead screw. For the rest of the unknowns I had to gather this information from the nut that mates with the lead screw from the McMaster-Carr website. Doing so I found the length to be 15.875mm, The material was bronze 673 and so I approximated the yield strength to be 140MPa. For this problem there were two unknowns with one being the pitch and the other being the number of threads in contact. I drew a free body diagram of the nut and lead screw, I was able to find a formula from the lecture that went over calculating the stress due to bending. The pitch was found by dividing 1 by the number of threads per inch which gave use 1.5875mm/thread. Once I found the pitch I was able to find the number of threads in contact by dividing the length of the nut by the pitch which gave us 10. According to the saftey factor of 4 and the yield strength the resulting allowable stress was 35MPa. The formula for stress due to bending was equal to (6F)/(n*pi*d*p), plugging in all over our known values this gave us a result of 13.003MPa which was significantly lower than the allowable stress and met the requirements. I went with the nut I initially selected, wrote down the part number and included additional information below. Also, there were three different flanges that were avalible that all had the same dimensions, just different types of steel. I decided to go with the 1015 carbon steel as it is cost effective and the tester will not be subjected to excessive moisture, thus causing rust. For more information about the flange and nut see below.

<img src="gb-7.png" alt="initial design" width="400">
<img src="gb-8.png" alt="initial design" width="400">
<img src="gb-9.png" alt="initial design" width="400">
<img src="gb-10.png" alt="initial design" width="400">
<img src="gb-11.png" alt="initial design" width="400">
<img src="gb-12.png" alt="initial design" width="400">
<img src="gb-13.png" alt="initial design" width="400">
<img src="gb-14.png" alt="initial design" width="400">
<img src="gb-15.png" alt="initial design" width="400">

### Cross Head

### Cost of Material: J.V. Muron

Below is the total cost of all the material and the assembly parts as well.
| Item Number | Quantity | Name | Cost | Purchase Link |
|-------------|----------|------|------|---------------|
| 60750       | 2        | ACME Lead Screw 3/16 RH Steel | 13.26 per foot | https://www.roton.com/family/acme-right-screws-and-nuts-7060750/ |
||----------|------|------|---------------|
|

### CAD Modeling and FEA
_Reference your concept selection (Pugh matrix) here. How does this design follow from that decision?_

## Communicate

