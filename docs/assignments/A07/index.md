# A7 – Finite Element Analysis on Bracket

## Objectives
1.) Conduct Finite Element Analysis on bracket design to optimize strength, stiffness, and weight of the bracket

2.) Improve design from results of analysis from running stress analysis, constraint, loading, and mesh selection

3.) Reconduct the Finite Element Analysis and compare results with percent difference for the max stress, max displacement, and factor of safety to be within 7 percent of each other. IF failure to converge at 7 percent, use the finest mesh 

4.) Iterate this loop for three different design choices

## Analyze
The directions for this assignment are stated below:

<img width="1486" height="284" alt="image" src="https://github.com/user-attachments/assets/ec86a9b7-58e3-45ed-a34c-d45e635e3857" />

Laying out the groundwork, the first design will be the initial design from Assignment 6. The material will be **Aluminum 6061 T6**. The structure will have the same parameters that were decided last time. For the analysis, the part should have a fixed constraint on the slider and the force will be acting along the cylindrical shaft. The force decided was **600 lbf**, and it will be split in half over the cylinder. To properly distribute this force as a strap force, a bearing load will be used in Fusion 360. Splitting the cylinder allows us to apply the strap load evenly across both sides of the cylinder while also using the assumed 0.75 inches of space for the strap from the previous assignment. 

Fixed Constraint:

<img width="2880" height="1360" alt="image" src="https://github.com/user-attachments/assets/9980f8de-b5a0-4fca-9264-550aca2a8d03" />

Force and Mesh Applied:

<img width="2864" height="1422" alt="image" src="https://github.com/user-attachments/assets/9eb14265-8ff0-4054-9f74-eda9bf7c7718" />




Percent difference and all measurements will be put into Excel and calculated. An evaluation will appear after discussing the results.

## Decide
The second design, the walls of the bracket will all be the same width for a more uniform structure, while adding more rigid support to the plate connecting the bracket and shaft. This will keep the plate from bending. The third design will help solve the stress in the shaft. The end of the rod will be connected to the sliding part of the bracket.

### Design 1 - Initial Design of Bracket
Running the initial stress test shows a lot of area for improvement. Below shows the FOS, max stress, and max location on the part:

#### FOS Design 1:

Iteration 1:
<img width="2880" height="1370" alt="image" src="https://github.com/user-attachments/assets/8375fe6f-71fe-4eaa-a7d5-b347ca9c3a10" />

Iteration 2:
<img width="2868" height="1420" alt="image" src="https://github.com/user-attachments/assets/3ae9f68e-6913-4415-b9d1-97b8ac784814" />

Iteration 3:
<img width="2272" height="1270" alt="image" src="https://github.com/user-attachments/assets/87d9d3b8-87d3-40f6-8fb6-0c93c6114d40" />

#### Stress Design 1:

Iteration 1:
<img width="2852" height="1378" alt="image" src="https://github.com/user-attachments/assets/a9937acb-2898-45b0-82c7-0c7d2c61ce32" />

Iteration 2: 
<img width="2860" height="1398" alt="image" src="https://github.com/user-attachments/assets/3bdedc41-474c-475a-b287-a4e56f245ede" />

Iteration 3:
<img width="2866" height="1250" alt="image" src="https://github.com/user-attachments/assets/6a57df50-616f-4a6d-a072-f2f0a8c3d86f" />

### Deflection Design 1: 

Iteration 1:
<img width="2858" height="1408" alt="image" src="https://github.com/user-attachments/assets/b4299add-3c27-494b-8212-d5cb0a20ae47" />

Iteration 2:
<img width="2854" height="1372" alt="image" src="https://github.com/user-attachments/assets/ed5af1b6-2025-433a-af29-d7ee11ca5a7d" />

Iteration 3:
<img width="2880" height="1254" alt="image" src="https://github.com/user-attachments/assets/bb796aae-3403-458b-b861-777385debe8f" />


Table: 
<img width="1912" height="258" alt="image" src="https://github.com/user-attachments/assets/66703caa-dc71-47e7-9f76-0e16cf2a6638" />

From the results, this design is unreliable due to the lack of convergence. While it converges on deflection, it is invalid and design needs to be redefined. Seeing the highest points of variability are the flange and the shaft.

### Design 2 - Increased Width of Fixture and Extra plating
This design will increase the strength on the flange. Increasing the width allows for a more uniform and stable strength around the bracket.

<img width="2874" height="1316" alt="image" src="https://github.com/user-attachments/assets/96f35a3e-e546-458d-97c8-1a7ab0cec408" />

#### FOS Design 2:

Iteration 1:
<img width="2880" height="1388" alt="image" src="https://github.com/user-attachments/assets/1e3280b4-1996-41df-a3d8-7891634c69fd" />


Iteration 2:
<img width="2876" height="1294" alt="image" src="https://github.com/user-attachments/assets/21960bdd-5b87-4ebd-b2aa-9ebaab28b0f0" />

Iteration 3:
<img width="2840" height="1242" alt="image" src="https://github.com/user-attachments/assets/5bfa4baa-dcc5-4b6f-8380-362d4ac64893" />

#### Stress Design 2:

Iteration 1:
<img width="2856" height="1244" alt="image" src="https://github.com/user-attachments/assets/8f9d8ef9-d235-4788-83bd-250a300ac589" />


Iteration 2: 
<img width="2880" height="1270" alt="image" src="https://github.com/user-attachments/assets/16f681cc-6f86-49c0-aab4-50b094d915ec" />

Iteration 3:
<img width="2856" height="1278" alt="image" src="https://github.com/user-attachments/assets/f63139f5-ab3c-48c9-8f03-47f5700f8653" />

### Deflection Design 2: 

Iteration 1:
<img width="2876" height="1294" alt="image" src="https://github.com/user-attachments/assets/e0ed1ff2-047d-4a9f-9c67-242d7ee5746b" />

Iteration 2:
<img width="2878" height="1324" alt="image" src="https://github.com/user-attachments/assets/ed0ee2d9-a562-4717-9a52-19796cd9a70f" />

Iteration 3:
<img width="2880" height="1316" alt="image" src="https://github.com/user-attachments/assets/f0b9362b-6f03-4eb7-9aaa-950dae830a75" />


Table: 
<img width="1996" height="214" alt="image" src="https://github.com/user-attachments/assets/47828f09-9f07-46b2-8299-4d3e348b8093" />


The results from this iteration were very promising. The stress has gone way down as well as the deflection. While it did not converge, the results show that the iterations are getting more similar. The factor of safety and stress are both very close in percent difference. This means the design is becoming more uniform. Issues with this design are the weight being too high and too much material. For the next design, the material added will be thinned out and also a fixture at the end of the shaft will be added for the end of the bar 


### Design 3 - Supporting connection on end of Fixture
For this 

#### FOS Design 3:

Iteration 1:


Iteration 2:




Iteration 3:




#### Stress Design 3:

Iteration 1:



Iteration 2: 




Iteration 3:



### Deflection Design 3: 

Iteration 1:




Iteration 2:



Iteration 3:






Table: 

## Communicate

