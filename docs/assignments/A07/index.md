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
The second design, the walls of the bracket will all be the same width for a more uniform structure, while adding ribs to the plate connecting the bracket and shaft. This will keep the plate from bending. The third design will help solve the stress in the shaft. The end of the rod will be connected to the sliding part of the bracket.

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


### Design 2 - Increased Width of Fixture and Ribs
Running the initial stress test shows a lot of area for improvement. Below shows the FOS, max stress, and max location on the part:

#### FOS Design 2:

Iteration 1:


Iteration 2:




Iteration 3:




#### Stress Design 2:

Iteration 1:



Iteration 2: 




Iteration 3:



### Deflection Design 2: 

Iteration 1:




Iteration 2:



Iteration 3:






Table: 

### Design 3 - Supporting connection on end of Fixture
Running the initial stress test shows a lot of area for improvement. Below shows the FOS, max stress, and max location on the part:

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

