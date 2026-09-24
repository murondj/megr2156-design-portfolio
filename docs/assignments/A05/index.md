# A5 – Bracket Design

## Objectives
1.) Perform a stress analysis to determine the dimensions and features of the bracket

2.) Generate FBDs of the features of the bracket.

3.) Identify the known variables and assumptions to calculate for the stress of the bracket.

4.) Perform a deflection analysis on the bracket and compare it to the stress analysis calculations to determine the minimum dimensions of the bracket.

5.) ensure structural integrity of the design by comparing analysis results to the constraints of the problem

6.) Create multiview dimensional sketches from the analysis

7.) Document and reflect on results

## Analyze
The constraints from the assignment are listed in the image below.
<img width="1378" height="1082" alt="image" src="https://github.com/user-attachments/assets/ebf833ca-bf0b-4968-8054-168ee4a6b7c4" />


## Decide
Since the range of the force is between 500 and 800 lbf, a force of **600 lbf** will be chosen for the design to support. Already familiar with the mechanical properties of **Aluminum 6061 T6**, this material will be used for the construction and the assumptions of the bracket. An assumption of how big the polyester strap is needs to be made to be able to create the design. Assuming the strap has a 0.75 inch width, the length of the first feature that holds the strap will be **1.25 inches** in length. Another assumption that the shape of the bracket will have symmetry over a vertical axis will also halve the work and the force chosen. 


### Feature A

Feature A is the cylindrical strap holder on the bottom of the bracket that is meant to hold the weight from the strap and drive the dimensions of the bracket. Assume that the feature will not fail in shear, that the average shear stress will be able to hold the strap, and that Feature A acts as a cantilever beam. Using these assumptions, the minimum diameter can be calculated. Using the Section Modulus relationship to the diameter of a cantilever beam, the formula is Z=(SF*W*l)/2*Sy. This relates the stress from the bending moment to the diameter of the beam. Solving for Z and setting it equal to the bending moment formula for a cylindrical beam, the calculated minimum diameter due to failure from bending stress is **0.576 in**.

To solve for failure of the beam due to deflection, assuming Feature A acts like a cantilever beam under uniform load, the formula to drive this calculation is delta=WL^3/8EI. Substituting the Moment of Inertia formula (I) for pid^4/64, the diameter can be calculated. Rearranging the formula to quad root of 8*W*L^3/pi*E*delta, the calculated diameter for failure from deflection is **0.416 in**

Comparing the two diameters, the feature will most likely fail due to stress before deflection. Therefore the minimum diameter of feature A is **0.576 in**. Since the design is being streamlined, the bar will be sized up to **0.625 in** or 5/8 of an inch. This is a more common bar size and does not interfere with the minimum diameter. The size may be changed later if it does not meet the required constraints. 

### Feature B

Feature B connects Feature A to the main clutch section of the bracket. It is assume to be treated as an axially loaded bar. It will also have a uniform cross-sectional area and no bending. Like Feature A, Feature B will not fail due to direct shear stress. To give the clutch of the bracket clearance from Feature A, an assumed length of **2 inches** will be used for Feature B. The width of the bar will connect Feature A to Feature B so it will carry the same length as the diameter of feature A which is **0.625 inches**.

Treating Feature B as a bar with an axial load, the formula for stress becomes sigma = F/A. Replacing A with wt will allow for the minimum thickness of the piece to be calculated. Factoring in the safety factor, the calculated result becomes **0.048 in** as a minimum diameter due to failure from stress.

Using the axial deformation formula of delta = FL/EA, and substituting A again for wt, a calculated minimum diameter becomes **0.0192 in**.

Judging the two calculated minimum diameters, Feature B must have a minimum diameter of **0.048 in**. To streamline the design, this value will also be moved to a better manufacturing variable of 1/16 of an inch or **0.0625 in**. 

### Feature C

Feature C is the bottom base of the clutch of the bracket. It is assumed to be a simply supported beam with a concentrated load at the center. The feature will also not fail due to direct shear stress. An assumed length and width of the feature will be **2 in**. 

Using the stress formula for a simply supported beam with a center load (sigma=MC/I), M can be substituted with FL/4, c can be subbed with t/2, and I can be substituted with bt^3/12. Algebraically solving for the minimum thickness yields the formula t=root1.5FL/bsigma. Accounting for the safety factor, the minimum thickness for Feature C due to stress constraints is **0.212 in**.

To get minimum thickness from the stiffness formula, delta=WL^3/48EI, substitute I for bt^3/12. Algebraically solving for minimum thickness will yield the formula tmin= cube root FL^3/4Ebdelta. This yields a result of **0.182 in** as a minimum thickness.

Failure from stress determines the driving dimensions for the feature again. To make the part easier to manufacture, the thickness will be taken up to **0.25 in** or 1/4 inch thick plate. 

### Feature D


## Communicate

