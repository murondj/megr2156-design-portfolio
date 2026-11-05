# A9 – Pulley Assembly

## Objectives

1.) Design a pulley system with listed constraints and conditions

2.) Find the diameter and circumference of pulley band, and choose a best fit for assembly

3.) Choose material of pulleys and determine the minimum diameter of the pulley shafts with a safety factor of 3.

4.) Design journal bearings that will best fit the assembly






## Analyze
The following assignment was given:

<img width="1692" height="1240" alt="image" src="https://github.com/user-attachments/assets/278433e8-7841-4241-af18-6bf5a82072c5" />

There are a few assumptions in the design that must be taken. Assume that the pulley operates at optimum speed and that there is no slip. This will allow for a calculation of the force. Also assume there is no thermal changes due to friction on the belt that causes warping or power loss. This allows for a smoother calculation on the belt size and choosing a belt.
## Decide

For this assignment, **[1060 AISI Steel](https://www.matweb.com/search/DataSheet.aspx?MatGUID=5fb9954cde754e709944d64233e50d3b)** was chosen as the material for the pulley wheels and the shafts of the pulley wheels. Journal bearing length was also chosen to be **1.5 inches**. This size was chosen because an assumption was made that the shafts and pulley are used in a belt driver for a heavy duty conveyor belt. These machines use large motors with high torque, so the bearings need to be able to handle the stresses from the higher torque.

The belt tension under static load was decided to be **5 lbf**, The operational speed of the pulley is at **2000 RPM**, and the center distance between the two pulleys is **5 inches**.

### Selecting a Pulley Band
To determine the pulley band that will need to be used, the minimum diameter and circumference of the belt need to be calculated. Algebraically solving for the force on the bands under static tension yields two forces.  The top belt is under **9.59 lbf** load while the bottom belt is under **0.41 lbf** load. Finding the area of the belt using the force, yield strength, and safety factor allows for a minimum diameter to be calculated to be **0.279 in**. The circumference then can be calculated to be **26.886 inches**. Based on these results, a **5/16 inch and 27 inch diameter and circumference band were chosen**.

<img width="748" height="1024" alt="image" src="https://github.com/user-attachments/assets/e226a91e-b36a-4195-b89b-4a1f62102d91" />


<img width="1852" height="744" alt="image" src="https://github.com/user-attachments/assets/6d203d2c-2c7a-4272-a0eb-21cc6c61177a" />

### Selecting a Shaft Diameter
Determining the minimum shaft diameter and minimum area where torque is applied is next. The shafts minimum diameter is determined based on the power the system delivers and the torque on the pulleys. Finding power of the pulleys allows for the torque the pulleys generate to be calculated. This value was **13.77 lb-ft**. Finding allowable shear stress in the shafts also leads to the calculation of the diameter. The calculated diameter yielded from the two values was **0.133 in**. This diameter calculation gave a minimum area of torque application of **0.0139 inches^2**.

<img width="794" height="988" alt="image" src="https://github.com/user-attachments/assets/77f1e4e6-d70d-4111-a8d3-9c63b3ad679b" />


### Determining Journal Bearings 

The bearings need to be chosen based on their PV rating. Below is the calculations to determine the PV rating. The calculations use the toque of the journal bearing, the bearing stress and the velocity of the bearing. The bearing stress was calculated to be **25.063 psi**. This gives a torque on the bearing of **0.133 ft-lb**. The velocity of the bearing is **898.5 ft/min**. This gives a PV rating of **22,519 psi ft**. Using the chart below, the best bearings to use based on this criteria is **porous bronze**. 


<img width="1304" height="978" alt="image" src="https://github.com/user-attachments/assets/1ccd7ad0-52e8-46b0-ad11-af236c7255e5" />

The diameter of the bearings is calculated to be **0.409 inches**.

<img width="772" height="1028" alt="image" src="https://github.com/user-attachments/assets/58483415-79fd-45d4-8eb2-d01272e174b0" />


### Frame Design - Drive Belt Housing for Conveyor Belt

For the frame design the pulleys will be on a frame of one bar. This bar is then connected to a triangular base. The triangular base can be connected at an angle or straight on to the base. This allows for different orientation of the pulleys depending on which way the conveyor belt is being intended to run. The mount also allows for the two pulleys to be rotated vertically on the triangular base for a vertical drive on the pulley.
<img width="2872" height="1336" alt="image" src="https://github.com/user-attachments/assets/f2ccc422-6b7b-4821-91b1-dfa8d04ed5ee" />

<img width="2876" height="1316" alt="image" src="https://github.com/user-attachments/assets/ee8caa95-cc06-437b-b379-ad7fdc445aea" />

## Communicate

I learned a lot about pulleys and their different applications in engineering. Pulleys can be used to reduce the weight of a load, or, like in this assignment, transfer power. The many applications of pulleys allow for more versatile and complex machinery. Understanding how pulleys work can allow for a more simplified design of a machine, saving time and money. 

This assignment took 4 hours over 1 day
