# A2 – Truss Stress Analysis

This assignment outlines the decision-making process that engineers must take to get a desired result. Design, analyze, and generate a report based on results and explain the decision-making process of the truss. 
## Objectives

1.) Design a lightweight planar truss that uses A500 steel or another steel material.  

2.) create a Free Body Diagram for the joints and critical pins.  

3.) Determine pin size from shear force and given safety factor of 3.5. Solve related equations symbolically and then numerically.  

4.) Estimate weight of truss and pins.  

5.) Create CAD model of the truss and compare the actual weight from the estimated weight.  

6.) Document learning and process.


## Analyze

The picture below shows the current constraints for designing the truss. 

The first step in analyzing and designing a truss is to research the types of trusses already available. There is no need to reinvent the wheel if someone has already optimized a design choice. Judging by the two load points C and D, a triangular point truss will not work. This narrows the choices down to a [Warren](https://en.wikipedia.org/wiki/Warren_truss), [Howe](https://en.wikipedia.org/wiki/Howe_truss), or [Pratt](https://en.wikipedia.org/wiki/Truss_bridge#Pratt_truss) truss. Using a trapezoidal shape and the least amount of material possible, A Warren truss variation is the best option. This is because when the two members are added, the shape is split into three triangles. Two of the triangles are similar, and one is different. These triangular shapes will allow the load types to be balanced and distributed through the members.


### Designing the Truss
The frame of the truss is assembled first. To find the length of the beams used, trigonometric operations are needed to find BC and AD connections. These operations are carried out below. Once one is solved, symmetrical properties can be used to calculate the other. The opportunity to calculate interior angles will also be used to confirm geometry and member and pin calculations. This will also help with determining placement of inner members.

the member BC is found to be 0.5m in length using the 3-4-5 trigonometric rule. It can be double-checked using Pythagoras Theorem. Our truss geometry becomes **AB = 1.2m, BC = 0.5m, CD = 0.4m, and DA = 0.5m**.

Now that the frame structure has been constructed, the inner member placement and static determinacy will be calculated. Two additional members will be added to the interior of the frame. Adding a joint at the midpoint of the truss will connect the two members. This brings our total members to 7 due to the splitting of the top beam. There is now a statically determinant truss since there are 7 members, 3 reaction forces, and 5 joints. Plugging this into the M+R=2J formula, it is calculated that 10=10. This means the structure is rigid and will not bend or experience torsion under a load.

With the design finalized, it is now time to solve the truss under load to determine if there are any inconsistencies with the previously calculated design. Solving each joint and member symbolically first will assist in determining symmetry. The values can be later substituted in. After solving the first two joints, the symmetry can clearly be seen as equal and opposite due to the applied loads, so only solving for the three joints on one side was necessary. Determining the zero force member where the loads were applied was also crucial in determining the members with the largest internal forces. After symbolically and numerically solving (shown below), the highest internal force members shown were the two added inner supports. These both carry a compressive and tensile load of 20.03 KN. 

Using this load of 20.03 KN, the minimum cross-sectional area of the truss can be calculated. Shown below, it can be seen that the final minimum area of the beams need to be **189.47 mm^2**. 

### Designing the Pins

Now that the truss has been assembled, the members need to be linked at pin connections. When connecting members by pins, shear force is introduced into the structure at these pins. 
## Decide
_Which geometry did you select, and why? This is your first open design choice in the course — defend it._

## Communicate

