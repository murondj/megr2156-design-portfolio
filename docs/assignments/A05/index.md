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

<img width="788" height="1070" alt="image" src="https://github.com/user-attachments/assets/02c68a79-e1ae-4074-9413-39ae63f3bf96" />

Comparing the two diameters, the feature will most likely fail due to stress before deflection. Therefore the minimum diameter of feature A is **0.576 in**. Since the design is being streamlined, the bar will be sized up to **0.625 in** or 5/8 of an inch. This is a more common bar size and does not interfere with the minimum diameter. The size may be changed later if it does not meet the required constraints. 

### Feature B

Feature B connects Feature A to the main clutch section of the bracket. It is assume to be treated as an axially loaded bar. It will also have a uniform cross-sectional area and no bending. Like Feature A, Feature B will not fail due to direct shear stress. To give the clutch of the bracket clearance from Feature A, an assumed length of **2 inches** will be used for Feature B. The width of the bar will connect Feature A to Feature B so it will carry the same length as the diameter of feature A which is **0.625 inches**.

Treating Feature B as a bar with an axial load, the formula for stress becomes sigma = F/A. Replacing A with wt will allow for the minimum thickness of the piece to be calculated. Factoring in the safety factor, the calculated result becomes **0.048 in** as a minimum diameter due to failure from stress.

Using the axial deformation formula of delta = FL/EA, and substituting A again for wt, a calculated minimum diameter becomes **0.0192 in**.

<img width="768" height="1046" alt="image" src="https://github.com/user-attachments/assets/2a6a5217-a170-470c-b39b-a09a1ccf8ee8" />

Judging the two calculated minimum diameters, Feature B must have a minimum diameter of **0.048 in**. To streamline the design, this value will also be moved to a better manufacturing variable of 1/16 of an inch or **0.0625 in**. 

### Feature C

Feature C is the bottom base of the clutch of the bracket. It is assumed to be a simply supported beam with a concentrated load at the center. The feature will also not fail due to direct shear stress. An assumed length and width of the feature will be **2 in**. 

Using the stress formula for a simply supported beam with a center load (sigma=MC/I), M can be substituted with FL/4, c can be subbed with t/2, and I can be substituted with bt^3/12. Algebraically solving for the minimum thickness yields the formula t=root1.5FL/bsigma. Accounting for the safety factor, the minimum thickness for Feature C due to stress constraints is **0.212 in**.

To get minimum thickness from the stiffness formula, delta=WL^3/48EI, substitute I for bt^3/12. Algebraically solving for minimum thickness will yield the formula tmin= cube root FL^3/4Ebdelta. This yields a result of **0.182 in** as a minimum thickness.

<img width="798" height="1072" alt="image" src="https://github.com/user-attachments/assets/604b8d1f-0ce0-49e3-a414-7e7210408d9b" />


Failure from stress determines the driving dimensions for the feature again. To make the part easier to manufacture, the thickness will be taken up to **0.25 in** or 1/4 inch thick plate. 

### Feature D
This will be the main contact clutch of the bracket. Looking at the tolerances, the minimum height is 1.499 +0.000/-0.001 for the T beam. Since the bracket needs to be detachable from the beam, a **0.150 in** height will fit. This keeps from having an interference fit that would force the parts together and gives the bracket a sliding fit. Feature D will also be assumed to not fail due to direct shear stress. 

Solving Feature D uses the same formulas as Feature B. Using this setup, the calculated minimum thickness due to stress failure is **0.015 in** while the minimum thickness of the plate from deformation failure is **0.0045 in**.

<img width="772" height="1018" alt="image" src="https://github.com/user-attachments/assets/f18b4da9-a4fb-4c4e-a218-26c7d32d623b" />


From this data, the dimension is again determined by stress failure. The chosen value of **0.015 in** is close to 1/64 inch plate so this value does not need to be changed for ease of manufacturing.

### Feature E

The last feature to calculate is the top of the clutch of the bracket. This part creates a contact force on the inner part of the T beam. This dimension will be driven by the assumption of a close fit for the T beam at 0.9992 +0/-0.0005. Allowing for clearance to allow the bracket to slide on and off is crucial to the design. For now, the design will use a **1 inch** width over part 'b' of the T beam. This will give .0008 inches of clearance, allowing just enough room to slide on. Assuming no direct shear stress failure and this 1 inch dimension are the only assumptions for this feature. Also treating this structure as a cantilever beam will also be assumed to allow the minimum thickness to be calculated. 

The stress failure calculated uses the max bending moment on a cantilever beam. This gives a **0.30 in** minimum thickness for the feature. Using the max deformation of a cantilever beam formula, the calculated minimum thickness before deformation failure was **0.23 in**. 

<img width="792" height="1034" alt="image" src="https://github.com/user-attachments/assets/88d7e794-5a79-45eb-b2c8-b591093bf824" />


From this, the minimum thickness of Feature E needs to be **0.30 in**.


### Drawings
This is the drawing of the stress dimensions

<img width="790" height="992" alt="image" src="https://github.com/user-attachments/assets/35f4f0fa-cfd6-4ed2-ba59-a4afc3cf5bb0" />


This is the drawing of deformation dimensions

<img width="800" height="1074" alt="image" src="https://github.com/user-attachments/assets/8a9585eb-622f-4486-9f47-f454c849c179" />


### Designing a Fit Link
Adding a link to Feature A that has a running/ sliding fit is done below. Assuming a 0.25 in thickness and the length is 4 inches, the calculated minimum width of the link needs to be above **1.12 inches** due to the 1 inch diameter hole needing material outside of the hole. A chosen width of **1.25** will allow for more material to surround the hole.


<img width="784" height="1026" alt="image" src="https://github.com/user-attachments/assets/f7b4ab13-252d-4b87-af53-af15abd75d6a" />

Running the stiffness calculation, the part is well under the 0.005 inch constraint set from earlier and will not deform. Using an RC 4 fit for the 0.625 inch diameter hole, the calculated tolerance can be found on page 654 in the *Machinery's Handbook*. It is an H8 hole with a +0.001 inch tolerance. This gives a range from 0.625 inches to 0.626 inches of the diameter. This hole is best reamed since it is a grade 8 fitting  (page 650)

For the 1 inch diameter hole, since it needs light assembly pressure, it is an FN 1 fit. The tolerance on this is + half a thousandth of an inch (Page 658). This is a grade 6 hole, so it can also be reamed.    

## Communicate

### Governing Failure Mode

The main failure mode of the whole design is stress failure. Aluminum 6061 T6 is an extremely stiff material and does not bend easily. Since the deformation of 0.005 is a "loose" range (depending on what the project is), it takes a lot more strength to reach the target deformation. IF the tolerance was tightened down to 0.001 inch, the failure modes would have been much closer.

### Error Propagation

Nothing calculated earlier caused a later error. For design sake, however, if the design required a uniform thickness, Feature D would need to be redesigned to fit the thickness of Feature E. Due to the calculations, Feature D could potentially be matched without calculating, but it is safe to check the calculation before actually applying the design change.

### Assumption Sensitivity

A lot of assumptions were made in this design, but the most important one was neglecting shear stress. This assumption impacts Feature B the most due to the axial loading of the part. The part would have to be thickened to help counteract the new shear stress in the piece. In a real setting, all the parts would most likely have to thicken to overcome the shear forces that act on them.

### Lessons and Insights

This project taught mainly how to make valid assumptions on a design. When designing a product, not all the information will be given, so assumptions must be made on a design. This can be done a smart way by creating criteria to assume on or disregarding criteria if it does not apply to the solution of a problem. It is important to distinguish the two and be able to produce a valid design. 

This project took 6 hours over the span of 1 day.
