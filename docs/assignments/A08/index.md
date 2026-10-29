# A8 – Gearbox Assembly

## Objective

1.) Design a gearbox and gear assembly that can be assembled and disassembled with appropriate assumptions

2.) Size the input and output shafts and analyze to find strength

3.) Create gearbox housing with proper clearance and fastening

4.) Parametrically model and design gearbox in CAD

5.) Render drawings for all parts 

## Analyze
For this assignment, the task is listed below:

<img width="1431" height="722" alt="image" src="https://github.com/user-attachments/assets/f69d240e-fc57-48b9-ae24-a41b01e999dc" />

Important information to pay attention to are the fits of the gears, the type of gears, clearance of gears and gearbox, and the assumptions about the gear system. This will allow for a valid design for the gearbox. Another assumption that will drive the design of the gearbox needs to be made, which is the intended purpose. Looking at different gearbox housings, each shape is assumed based on the function of what the gears are intending to drive. For example, a car gearbox is very different looking than a gearbox that drives a 3D printer. Judging by the size of the gears and the output, this is more likely to be in a 3D printer. Because of this, the housing for the gears do not need to have a specific geometry or special requirements to fit in an allotted area. With this assumption, this allows the gearbox to be a basic design that will accomplish the task of housing the gears.


### Evaluation of Shafts

Before construction of the gearbox, the strength and geometry of the shafts needs to be assessed before continuing. This will make sure that they are able to operate under the load required and not fail due to torsion or cannot fit into the gears with the required fits.

#### Input Shaft

The input shaft is a power transmission shaft that is driven directly from the motor. It holds the pinion gear and drives the reduction gear and output shft.

To solve the stress limit and diameter required, multiple calculations need to be performed. First, Finding the input torque and speed is required to find the stress and diameter. To solve this, assume 100 percent efficiency in transmission from input to output. The following ratio of output torque over the gear ratio can be used with this assumption, giving a calculated value of **0.172 in-lbf**. The speed of the input shaft is calculated by multiplying the gear ratio by the output speed of the shaft. This gives an input speed of **7975 RPM**. 

<img width="848" height="1130" alt="image" src="https://github.com/user-attachments/assets/20d38075-5e53-4fb1-b99a-4829f0a475e7" />


From the input torque and the input speed, the stress limit and the minimum diameter can be calculated. The major results calculated was a stress limit of **448.5 psi** and a minimum shaft diameter of **0.06 inches**. This is smaller than the diameter of the shaft, so the power transmission shaft diameter of **0.125** in is applicable and does not need to be changed.


#### Output Shaft

The output shaft is a short shaft that is connected to the input shaft via the reduction gear and pinion gear. It drives the desired lower speed and torque to the machine assembly. 

<img width="836" height="1118" alt="image" src="https://github.com/user-attachments/assets/ae7dc54f-a39b-4e42-801c-f36d3859fd6a" />


Since the output torque and speed is already known, the minimum diameter and stress limit can be calculated directly. Note that the formula for diameter is different for a short shaft compared to a power transmission shaft. The calculated value of the stress limit is **407.4 psi** and the calculated minimum diameter is **0.09 inches**. The shaft diameter of **0.25 inches** is well above this, so this is a valid shaft for the output shaft.


### Journal Bearings

Journal bearings allow the shafts to freely spin while also guiding the shafts and anchoring them to a design. For the gearbox assembly, the journal bearings will hold the shaft into the assembly and allow them to freely rotate while also keeping them in place in the assembly. 

For this part of the design, the material and bearing thickness need to be determined. The length of the bearing needs to be assumed for these calculations. A 1:1 ratio of each shaft diameter to journal bearing should yield desired results. If not, it can be changed after calculation. 

#### Input Shaft Bearing

The diameter of the shaft is 0.125 inches. To have a press fit with the gearbox housing, the tolerance for the hole to house the journal bearing is an FN 6 fit. The fit to the journal bearing to the shaft is an RC5 fit. Below are the calculations to solve for PV and material selection:

<img width="764" height="1068" alt="image" src="https://github.com/user-attachments/assets/a6bafa23-eae2-4f00-8e32-3f705c23429b" />

Using the pitch diameter of the pinion, the calculated PV due to radial force over the bearing area is **5913.81 psi ft/min**. The calculated thickness due to allowable hoop stress to diameter ratio calculated a thickness of **0.125 in** Originally, graphite was chosen as the bearing material, but the website did not offer a bearing of this thickness and length in that option, so bronze was chosen instead for this [bearing](https://www.mcmaster.com/products/journal-bearings/sleeve-bearings-3~/shaft-diameter~1-8/length~1-8-1/od~0-252/) (9368T95). Note the size is also 0.252 inches instead 0.250 inches.

#### Output Shaft Bearing

The same process was done for this bearing as well. Instead of the pinion pitch, the gear pitch was used instead. This gave a calculated PV of **1114.98 psi ft/min**. A calculated thickness of **0.38 inches** was calculated as the thickness. For consistency, this bearing was also switched to bronze. This was the [bearing](https://www.mcmaster.com/products/journal-bearings/shaft-diameter~1-4-1/length~1-4-2/) (S391K126) chosen.

<img width="810" height="1126" alt="image" src="https://github.com/user-attachments/assets/e5dc23c6-5650-49a0-a0f4-c5c4ec95701e" />


All parts will be listed at the end of the document as well for further research.
## Decide

### Assembly of Gearbox
Now to design the assembly. The assembly will be in two parts with a snap-fit together. The dimensions of the box need to be larger than both gears combined side by side. The pinion gear has a diameter of **0.402 inches** and the reduction gear has a diameter of **1.027 inches**. A **2.5 inch by 2 inch box** will fit both gears with clearance. The depth of the box needs to be calculated. Given the journal bearings, the wall needs to be **0.25 inches** thick. The shafts need to stick out for input and output connection. The gear's depths are **0.308 inches** for the power gear and **0.368 inches** for the reduction gear. The gears need to rotate freely and not rub against the inner wall. This gives a depth of **1 inch**, which gives clearance for the gears to not rub the walls. Note the cover will be included in that thickness.

<img width="832" height="1078" alt="image" src="https://github.com/user-attachments/assets/685a3612-3c8c-45e5-923a-725d98809ebf" />

### CAD Modeling of Gearbox
These are the parametric equations for the box itself

<img width="2374" height="1120" alt="image" src="https://github.com/user-attachments/assets/8562cf80-2cc1-41e2-a171-ef2bfce4bc32" />


The first part before full assembly is the gearbox. Using parametric equations, the box is constructed below.

<img width="2876" height="1326" alt="image" src="https://github.com/user-attachments/assets/73784890-7ab5-4bf4-9c8c-eb3106b92251" />

Next, the box is shelled down to 0.25 inches:

<img width="2880" height="1322" alt="image" src="https://github.com/user-attachments/assets/84e86d2d-a104-40c6-a6aa-7ab481b7aeb6" />

The holes that hold affix the pegs from the front plate need to be added. Assuming a 3D printed model, the clearance should run an 8 thou clearance for a press fit that can be pulled apart for maintenance. Peg size will be 1/8 of an inch in diameter and will go a depth of 0.30 inches. These holes are part of a pattern that can be adjusted.

<img width="2870" height="1330" alt="image" src="https://github.com/user-attachments/assets/8ab8173b-9024-4178-b318-971818085cab" />

Now the holes for the journal bearings are made. Note, to get a press fit, you would need a diameter of around 0.2514 inches for the press fit of the first hole. the modeling would not work unless the part was as large as the hole. There is probably a technique in CAD software to mark a press fit, but it is not known. The drawings of the model will have the correct tolerance on the hole.

<img width="2870" height="1314" alt="image" src="https://github.com/user-attachments/assets/b7b51980-2b40-46e8-a269-a89136b599be" />

Next, the other hole is determined in placement. To prevent overheating and allowing gears to rotate freely, a backlash of 10 thou is added to allotted. By combining the pitch diameters of the gears and dividing by 2, this gives a shaft distance of 0.6771 inches. Adding backlash gives a distance of 0.6871 inches.

<img width="2872" height="1338" alt="image" src="https://github.com/user-attachments/assets/2af36716-d7c3-44a8-b77b-77df35ee8710" />

The front covering of the gearbox is made using the same steps but with pegs added instead of holes and no shelling of the model. 

<img width="2876" height="1312" alt="image" src="https://github.com/user-attachments/assets/a5f1e7dd-9de3-4eef-addc-5567a6d14815" />


### CAD Modelling of Shafts

The shafts are 0.125 inches by 1 inch and 0.25 inches by 1 inch respectively. A chamfer was added to allow for easier press fit to gears.

<img width="2874" height="1316" alt="image" src="https://github.com/user-attachments/assets/80d15974-0324-41c3-a3ff-7717ecbd0540" />


<img width="2874" height="1324" alt="image" src="https://github.com/user-attachments/assets/be44620d-421b-4e4d-9734-7c1e7add9c78" />

### Full Assembly

Now for the full assembly. All the parts are added into one assembly. Realizing that one of the journals was smaller than the other, the hole originally cut is modified to fit the journal while also leaving a recess for the shaft to fit through with enough clearance to rotate. 

<img width="2876" height="1318" alt="image" src="https://github.com/user-attachments/assets/f21cf57a-e43b-4dea-b1a8-677fe7493cba" />


<img width="2858" height="1330" alt="image" src="https://github.com/user-attachments/assets/f7869e07-5783-4823-bf8f-bfc376df227b" />

<img width="2866" height="1326" alt="image" src="https://github.com/user-attachments/assets/0bff5708-2c85-4062-94db-d3b31a386033" />



### CAD Drawings of Gearbox Assembly
Here are listed drawings completed for the 2 shafts, 2 plain bearings, and 2 housing pieces.

<img width="1896" height="1230" alt="image" src="https://github.com/user-attachments/assets/368be6ec-35ad-4d14-9c9a-feffd5fa09ac" />

<img width="1904" height="1226" alt="image" src="https://github.com/user-attachments/assets/0853a8cc-32d0-415a-b351-d3039bfae5f3" />

<img width="1744" height="1126" alt="image" src="https://github.com/user-attachments/assets/618bd910-d74b-43f5-b07d-24cfb4fd61ba" />

<img width="1824" height="1174" alt="image" src="https://github.com/user-attachments/assets/e69a4ad0-8170-4a11-914c-4073610968b5" />

<img width="1710" height="1110" alt="image" src="https://github.com/user-attachments/assets/483bf62e-4fc0-425f-ada2-76e0deba21e9" />

<img width="1868" height="1206" alt="image" src="https://github.com/user-attachments/assets/4e29b0b9-fe4c-4252-8164-331c22361267" />

## Communicate

This project used a lot of CAD. I learned a lot about assemblies and how to put everything together into one cohesive design. It was really satisfying being able to put everything together and watch a working product, even if it is just a design and not a full product. Being able to see how everything interacts allows for changes to be made to the design, which I ended up doing. There was also a lesson in the design phase is never really over. The initial design is never the final product because you will always find something to tweak or design something more practically.

This assignment took 8 hours over 2 days. 

## Appendix

### Files for CAD

#### Assembly
[Full Assembly](Gear_Box_Assembly.f3z)

#### Parts Made from Scratch

[Housing](Gearbox_Housing.f3d)

[Housing Lid](Gearbox_Housing_Lid.f3d)

[Input Shaft](Pin_for_pinion.f3d)

[Output Shaft](Shaft_GearReduction.f3d)

#### MCMaster-Carr Parts

Bronze sleeve Bearing: 6391K126 and 6391K611 

[Pinion Gear](https://www.mcmaster.com/catalog/129/1330/7880K19)

[Gear](https://www.mcmaster.com/catalog/129/1330/7880K24)

