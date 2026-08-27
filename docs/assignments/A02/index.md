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

The first step in analyzing and designing a truss is to research the types of trusses already available. There is no need to reinvent the wheel if someone has already optimized a design choice. Judging by the two load points C and D, a triangular point truss will not work. This narrows the choices down to a [Warren](https://en.wikipedia.org/wiki/Warren_truss), [Howe](https://en.wikipedia.org/wiki/Howe_truss), or [Pratt](https://en.wikipedia.org/wiki/Truss_bridge#Pratt_truss) truss. Using a trapezoidal shape and the least amount of material possible, A Warren truss variation is the best option.

The frame of the truss is assembled first. To find the length of the beams used, trigonometric operations are needed to find BC and AD connections. These operations are carried out below. Once one is solved, symmetrical properties can be used to calculate the other. The opportunity to calculate interior angles will also be used to confirm geometry and member and pin calculations. This will also help with determining placement of inner members.

the member BC is found to be 0.5m in length using the 3-4-5 trigonometric rule. It can be double-checked using Pythagoras Theorem. Our truss geometry becomes **AB = 1.2m, BC = 0.5m, CD = 0.4m, and DA = 0.5m**.

Now that the frame structure has been constructed, the inner member placement and static determinacy will be calculated. Two additional members will be added to the interior of the frame. Adding a joint at the midpoint of the truss will connect the two members. This brings our total members to 7 due to the splitting of the top beam. We now have a statically determinant truss since there are 
## Decide
_Which geometry did you select, and why? This is your first open design choice in the course — defend it._

## Communicate

