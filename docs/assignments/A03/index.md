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




## Communicate

