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
The second design, the walls of the bracket will all be the same width for a more uniform structure, while adding more rigid support to the plate connecting the bracket and shaft. This will keep the plate from bending. The third design will help improve on the second design by becoming a more applicable model adding extra support fixture closer to the end.

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


### Design 3 - Supporting connection for end of Fixture
For this design the added material is thinned down and there is an extra bar to support the end of the link by adding extra support closer to the end.


<img width="2874" height="1554" alt="image" src="https://github.com/user-attachments/assets/4458b19a-80b3-4b66-aea5-5800a3d528fd" />


#### FOS Design 3:

Iteration 1:
<img width="2880" height="1280" alt="image" src="https://github.com/user-attachments/assets/122f1fac-3b3e-46a7-a990-ac4a9dd5920a" />

Iteration 2:
<img width="2879" height="1389" alt="image" src="https://github.com/user-attachments/assets/e08a1e43-ecb0-402a-b03b-dca980dde168" />

Iteration 3:
<img width="2851" height="1391" alt="image" src="https://github.com/user-attachments/assets/46f3b769-ca8d-4383-9373-bb5d4400b1c0" />

#### Stress Design 3:

Iteration 1:
<img width="2876" height="1264" alt="image" src="https://github.com/user-attachments/assets/99f60dc7-a03a-42a6-8db3-8562252151bb" />

Iteration 2: 
<img width="2873" height="1642" alt="image" src="https://github.com/user-attachments/assets/72e543c4-5d9f-4cea-96d7-5cd61e8c3712" />

Iteration 3:
<img width="2873" height="1391" alt="image" src="https://github.com/user-attachments/assets/ae16fc3f-3c0f-4d09-bd1e-795db8e4406c" />

### Deflection Design 3: 

Iteration 1:
<img width="2880" height="1312" alt="image" src="https://github.com/user-attachments/assets/e6e616e6-6c68-4afe-9dbb-fb7085170e54" />

Iteration 2:
<img width="2879" height="1649" alt="image" src="https://github.com/user-attachments/assets/22c90c0e-a192-4834-95d6-bc03fb8951f4" />

Iteration 3:


<img width="2874" height="1533" alt="image" src="https://github.com/user-attachments/assets/358e54a6-d389-49e5-a2c4-ae7e380842a9" />

Table: 

<img width="1909" height="203" alt="image" src="https://github.com/user-attachments/assets/f4983b9a-5718-4385-82a0-f250c440b091" />


### Linkage FEA
Running the same three tests on the linkage shows that 

#### Safety Factor
Iteration 1:
<img width="2875" height="1256" alt="image" src="https://github.com/user-attachments/assets/eddc13d9-9031-4f11-acd3-cf99d0f6a351" />

Iteration 2:

<img width="2879" height="1308" alt="image" src="https://github.com/user-attachments/assets/4cb4aeb1-50b8-4aed-9280-eb374be9195f" />

Iteration 3:
<img width="2846" height="1288" alt="image" src="https://github.com/user-attachments/assets/889ff330-688b-49d4-9c36-4a241cb2b5a0" />

#### Stresses

Iteration 1:
<img width="2874" height="1298" alt="image" src="https://github.com/user-attachments/assets/2bbc3536-3d67-4405-8762-f01264c437ec" />

Iteration 2:
<img width="2871" height="1440" alt="image" src="https://github.com/user-attachments/assets/3ec12e87-1120-41f7-9f38-f7bb17ab681b" />

Iteration 3:
<img width="2879" height="1422" alt="image" src="https://github.com/user-attachments/assets/1de8db41-ce32-448c-84d0-d2c57eb9b9e5" />

#### Stiffness
Iteration 1:

<img width="2874" height="1426" alt="image" src="https://github.com/user-attachments/assets/8d2b5598-ab3f-45a4-a821-30b6af861357" />

Iteration 2:

<img width="2849" height="1260" alt="image" src="https://github.com/user-attachments/assets/192c02df-83e0-4d73-a65c-dfdd804ab5e5" />

Iteration 3:
<img width="2879" height="1424" alt="image" src="https://github.com/user-attachments/assets/35bd51df-a58a-4e14-89a4-80d1ddfd5340" />


Table:
<img width="2076" height="312" alt="image" src="https://github.com/user-attachments/assets/649b8614-097f-424f-b045-6b2880b112e9" />

Due to time constraint, rerunning the test with modifications was not possible, but it can be described. Changing the amount of material around the hole or making it thicker will allow for the stress and stiffness to be increased.
## Communicate

Since the analysis did not have convergence on all features for any iteration, there has to be a choice made based on what options are available. The first design gives an extremely light design, at the cost of relatively no safety factor. The second design gives the lowest stress and highest safety factor, but is extremely bulky and weighed down. The last design has the max stiffness and better balance between all variables, but it is also more complex design and still has weight. Based on the criteria, design 2 is the best choice because it has the lowest stress and highest safety factor. The governing failure mode for this design was stress, so it would be best to pick the design that has the least amount of stress on the system.

This is a prime example of an engineering defense. Since there was no perfect outcome, there had to be a compromise on the parameter of the design. Based on the needs of what the bracket was used for, the more expensive, safer option was chosen over the riskier option. This assignment was also a great exercise on how to iterate over a design to find the best outcome, and keep tweaking the design using computer simulation. This allows an engineer to risk asses and also be firm in the choices made for a design.

### CAD UPDATED FILEs : [Updated Bracket](UpdatedBracketDesign.f3d) and [Linkage](BracketLink(2).f3d)



This project took 8 hours over the course of 2 days.
