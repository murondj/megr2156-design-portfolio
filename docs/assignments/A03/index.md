# A3 – Parametric and Finite Element Analysis

## Objective
1.) Using the axial deflection formula, model an aluminum bar and generate dimensions of the bar.

2.) Use parametric design to determine length of the bar  

3.) Introduce an understanding to the concepts of Finite Element Analysis (FEA)

4.) Link dimensions to certain parameters using CAD software

5.) Compare and Contrast the different analysis types

## Analyze
The photo below is the prompt given for this assignment.

<img width="1348" height="578" alt="image" src="https://github.com/user-attachments/assets/71642269-ac81-49e2-8968-692d96772f13" />


The parameters state a force between **300-500 lbf** is chosen, the max axial deflection in the bar should be **0.009 inches**. The aluminum chosen for the bar should have a Young's Modulus in the range of **8.5 - 11.5 Mpsi** (10^6). 

## Decide

### Parametric Parameters

The chosen force load for the Parametric analysis was **400 lbf**. The chosen diameter of the rod is **0.75 inches**. Since the rod is circular, there is no need for a height or width dimension, just the diameter of the bar. The chosen Aluminum is **Aluminum 6061 T6** with a Young's Modulus of **10,000 ksi or 68.9 GPa**. These will be used to calculate the max length of the bar.

Using Hooke's Law, the stress, and the strain equations, the length of the bar can be determined. Rearranging Hooke's Law where the Young's Modulus is equal to the Stress over the Strain. Substituting the Stress formula (F/A) and the Strain Formula (Delta L /L),  The new formula is E = F(Delta L)/LA. Solving for the change in length, or the deformation, the new formula is Delta = FL/EA. This equation can be used to solve for the length. To get the length the formula becomes L = Delta(EA)/F. Using the numbers given the calculated length becomes **L = 99.4 inches.**


### Creo Parametric Solving  

The variable calculated above needs to be verified with CAD software. Using the relations tool and parameters tool in Creo Parametric, The values of the 6061 T6 Aluminum can be entered to solve for the length of the bar. First, the material properties are entered into the material property file.

<img width="2328" height="1698" alt="Screenshot 2026-09-08 215218" src="https://github.com/user-attachments/assets/06445964-2eda-476c-b60b-8495d1210351" />


Once the file has been loaded into Creo, a dimension is needed to set the relations for the bar. The chosen diameter is inserted and the circle is sketch with a temporary extrusion.

<img width="2880" height="1254" alt="image" src="https://github.com/user-attachments/assets/0259419e-3b02-46ba-841c-f5abf8620f97" />

Now that there is a temporary place holder, the parameters can be defined for the bar. Going to the relations tool and switching dimension modes, the variable names for the diameter and length can be found. After this, the deformation formula is coded into the software as well as the variables used. Since the Aluminum 6061 T6 material property is already loaded into the software, some of the data can be pulled from that file.

<img width="2872" height="1488" alt="image" src="https://github.com/user-attachments/assets/c9279727-a922-4c4e-be22-67006267d8ad" />


After verifying that the relations will work and there are no errors in the coding, it is time to test the result.

<img width="2880" height="1482" alt="image" src="https://github.com/user-attachments/assets/29414a09-12a4-44fd-88ec-ec47327e840c" />


Immediately off the bat, something is wrong. The length becomes 38,000 inches long. Checking the material file, there was an error when loading the properties.

<img width="1254" height="1556" alt="image" src="https://github.com/user-attachments/assets/e5557dc9-b0ba-4ca7-b5e7-c42eb13f75e5" />




For some reason, Creo decided that it was going to convert the properties in a way that cannot even be calculated. Fixing this will hopefully scale our model to the correct length. Reverting all the measurements back to the original values, this was the result.

<img width="2880" height="1494" alt="image" src="https://github.com/user-attachments/assets/1b70264c-a2b0-4e56-bbae-6c0f0f89f79b" />


This matches perfectly with the predicted length of 99.4 inches. Since the diameter variable is arbitrary, it can be changed later on when calculating a new diameter and new force. Unfortunately, the Creo Simulate software license for students does not exist, so moving over to Fusion, the parameters will be translated over there. 




### Fusion FEA
The bar has been parametrically constrained now into Fusion. Applying a fixed end and a load of 400 lbf on the opposite end of the bar will give this configuration.

<img width="2880" height="1428" alt="image" src="https://github.com/user-attachments/assets/22f11284-6619-475d-ae1e-1a7c6b80ba59" />



#### Deflection
The mesh is added to the beam and the solver is ready to run. From the beam solver, there is a max displacement of 0.017 inches. This is bad, extremely out of range. After an hour of troubleshooting, those are the correct results. Researching the topic further and looking at Fusion software, this is also accounting for gravity and weight of the bar. Since the bar is acting like a column, the slenderness to smallest radius of gyration is too large, causing a moment. This is causing the bar mainly to deform and bend in the z direction, but also affecting the other measurements.
<img width="2858" height="1272" alt="image" src="https://github.com/user-attachments/assets/c6bea89a-7173-4431-8291-f858ccb3b775" />

#### Von Mises Analysis
The Von Mises is well below the max allowable stress of 40 ksi at 2.389 ksi. This gives a safety factor of **16.74**. This means the bar is extremely strong and can withstand high loads.


<img width="2860" height="1290" alt="image" src="https://github.com/user-attachments/assets/fa2f81d6-bfd1-4065-9150-ec022b1c46fc" />


From The percent difference, there was an **88.89%** difference in the actual vs. the calculated delta. As stated above, this is due to the length of the bar and what the software is calculating. The simulation adds gravity and other factors, and the bar is subjected to these forces. The simulation is more accurate than the hand calculation due to the individual calculations it runs on the bar. Practically speaking as well, an aluminum bar that is a quarter of an inch thick and eight feet long is going to be subjected to some deformation due to the geometry of slenderness to thickness. Depending on the use of the bar, it still does have the practical applications of having a high yield stress, and can be used in an application where that is useful.

## Communicate

