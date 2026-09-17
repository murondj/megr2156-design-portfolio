# A4 – Motor Mount

## Objective
1.) Design and solve a Motor Mount to the required specifications of the assignment. Use bending moment and deflection equations to solve for each unique feature.

2.) Design Motor Mount in CAD and create a Drawing for the Design

## Analyze
This assignment task is given below.

<img width="1400" height="744" alt="image" src="https://github.com/user-attachments/assets/fbf41493-ccb2-481b-8cd4-5f6a152538e1" />




## Decide
Using these specifications, a motor mount will be designed. After some research online, most motor mounts use an L-shape bracket to hold the motor. This allows for ease of installment, distribution of mechanical stresses, and allows for compact storage of the motor in a design. After researching the materials, the best material for this design is **PLA**. While the filament is not very heat resistant, ABS can warp while being printed causing mechanical failure immediately, and while PETG is strong and durable, it is moisture sensitive and can cause printing problems while being assembled. Since this is a prototype, PLA fits the requirements the best. The final design should be made out of a metal that can be researched later.

PLA (PolyLactic Acid) has an Elastic Modulus of around 3,500 MPa, assuming a solid fill for the design, which is what will be assumed from here. The yield strength of PLA can range anywhere from 35-60 MPa depending on printing orientation, molding, and infill of the parts. To simplify, it will be assumed middle range of 47.5 MPa for the tensile yield strength. 

### Feature 1: Motor Housing

Feature 1 will have where the motor will sit on the plate. There will be a slight indentation to hold the motor in place. From earlier assumptions, this plate will be treated as a cantilever beam. The cross-sectional area needs to be calculated from the max strength and stiffness. To get these measurements, the length and width of the plate must be determined. Using the 24mm diameter, the motor should have some clearance from feature 2. With this in mind, a design that should be implemented is a filleted corner intersect between 1 and 2, so a 50mm plate length and width will be enough to account for bolts and wall clearance from Feature 2. On Feature 1 the force of the motor is 300 N. Giving 13mm of clearance from the wall of feature 2 will allow the motor to have enough clearance to run.

To find the height for the beam, a comparison for the stress allowed and the deflection will give a height of the beam that will fit the parameters. For allowable stress, the formula is equal to the Bending moment of the beam times the distance from neutral axis, divided by the moment of inertia. To solve for the height of the beam, I can be substituted with bh^3/12, M can be substituted with PL, and y can be substituted with h/2. Rearranging and algebraically solving for height, the new formula becomes h = square root of 6PL/b(allowed stress). With a safety factor of 3, the allowed stress becomes 15.83 MPa. Solving for h using allowed stress, it is calculated to be the minimum height needed to support the load under stress is **5.44 mm**.

For solving the minimum height with deflection, start with the deflection formula of a beam with delta equal to PL^3/3EI. Substituting I with bh^3/12 again, the formula can be algebraically simplified to 4PL^3/Ebh^3. To solve for h, the formula becomes the cubed root of 4PL^3/Ebdelta. The calculated value for this is **3.69 mm**.

From these calculations, the allowable stress will fail before the beam reaches a max deformation of 0.3mm. Therefore, the chosen minimum height requirement will be 5.44 mm. This is within the tolerance of the motor driver that has a 6mm tolerance. For a little wiggle room, the height will be moved up to **5.50 mm.**

Notice how 13mm length is not a lot of room for clearance with the motor having an 11mm diameter. This only gives us a wall that can be about 10mm thick max.
### Feature 2

Much like Feature 1, the minimum height needs to be calculated for the mount part. Since the end is free to bend on this part, there is a much larger bending moment on feature 2. To mitigate this, the height will be dropped from 50mm to 25.5mm. Note this includes the 5.5mm from feature 1 at the bottom. Using the same formulas from earlier, with the new calculated bending moment of 300*25.5, the calculated minimum height (or thickness rather) for stress becomes **7.62 mm** and 7.24 mm. Since the stress failure is a larger thickness, 7.62mm will be used. Giving some more wiggle room, the number goes up to 7.7mm.

### Fusion Model of Mount

Using Fusion 360 software a general sketch using the lengths and thicknesses from Feature 1 and Feature 2 are conducted. For the sketch, Feature 1 is 50mm long, 50mm wide and 5.5 mm thick from the top view.

<img width="2866" height="1340" alt="image" src="https://github.com/user-attachments/assets/87e47b91-ef88-410b-99f2-482ea8d227c6" />

Adding these dimensions to the parametric equation sheet as well for ease of changing later. Next Feature 2 is added to Feature 1. Since the thickness is already at 5.5mm, adding 20mm will be good for the height. This is also added in the parametric equations. 

<img width="2868" height="1302" alt="image" src="https://github.com/user-attachments/assets/5ce79cb3-3874-4de6-9cd3-8aca18524202" />


The next step is to add the hole where the motor mount will come through. This is 13mm away from the inside facing wall. The radius circle outside of that which will hold the motor in place. Finally, the fastener M3 holes will be added into this circle. All of this can be parametrically combined into one part. adding a sinking rest allows the motor to also be more secure in the mount. A fillet just under the clearance of 3.3 set at 2.5mm will be enough for the inside while the outside fillet will be 3mm. This gives the design extra deflection and also spreads the area of the part out larger, allowing for a larger bending moment. 


<img width="2874" height="1324" alt="image" src="https://github.com/user-attachments/assets/132b1d35-d15f-47f5-97b3-b208f950e741" />

To finalize the design, the fastener holes to attach the mount need to be added in. This will also be parametrically determined. The edge of the holes needs to be 5mm from each corner. 

<img width="2880" height="1440" alt="image" src="https://github.com/user-attachments/assets/1860fae9-c5e9-4a05-8d51-5c9972757a92" />

Here are the parametric equations used.


<img width="2370" height="962" alt="image" src="https://github.com/user-attachments/assets/452cd8c5-2528-4143-b0ee-c7a7679a2e0a" />



### CAD Drawing
<img width="1676" height="1200" alt="image" src="https://github.com/user-attachments/assets/4b4fe76b-8dad-4498-9caa-976049f1cb1e" />

### Files For CAD Work
Here are the files for the CAD work completed.

[Motor Mount CAD File](Motor Mount.f3d) 


[MotorMount.pdf](https://github.com/user-attachments/files/32318567/MotorMount.pdf)


