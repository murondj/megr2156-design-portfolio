# A8 – Gears

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

From the input torque and the input speed, the stress limit and the minimum diameter can be calculated. The major results calculated was a stress limit of **448.5 psi** and a minimum shaft diameter of **0.06 inches**. This is smaller than the diameter of the shaft, so the power transmission shaft diameter of **0.125** in is applicable and does not need to be changed.


#### Output Shaft

The output shaft is a short shaft that is connected to the input shaft via the reduction gear and pinion gear. It drives the desired lower speed and torque to the machine assembly. 

Since the output torque and speed is already known, the minimum diameter and stress limit can be calculated directly. Note that the formula for diameter is different for a short shaft compared to a power transmission shaft. The calculated value of the stress limit is **407.4 psi** and the calculated minimum diameter is **0.09 inches**. The shaft diameter of **0.25 inches** is well above this, so this is a valid shaft for the output shaft.


### Journal Bearings

Journal bearings allow the shafts to freely spin while also guiding the shafts and anchoring them to a design. For the gearbox assembly, the journal bearings will hold the shaft into the assembly and allow them to freely rotate while also keeping them in place in the assembly. 

For this part of the design, the material and bearing thickness need to be determined. The length of the bearing needs to be assumed for these calculations. A 1:1 ratio of each shaft diameter to journal bearing should yield desired results. If not, it can be changed after calculation. 

#### Input Shaft Bearing

The diameter of the shaft is 0.125 inches. To have a press fit with the gearbox housing, the tolerance for the hole to house the journal bearing is an FN 6 fit. The fit to the journal bearing to the shaft is an RC5 fit. Below are the calculations to solve for PV and material selection:



Using the pitch diameter of the pinion, the calculated PV due to radial force over the bearing area is **5913.81 psi ft/min**. The calculated thickness due to allowable hoop stress to diameter ratio calculated a thickness of **0.125 in** Originally, graphite was chosen as the bearing material, but the website did not offer a bearing of this thickness and length in that option, so bronze was chosen instead for this [bearing](https://www.mcmaster.com/products/journal-bearings/sleeve-bearings-3~/shaft-diameter~1-8/length~1-8-1/od~0-252/). Note the size is also 0.252 inches instead 0.250 inches.

#### Output Shaft Bearing

The same process was done for this bearing as well. Instead of the pinion pitch, the gear pitch was used instead. This gave a calculated PV of **1114.98 psi ft/min**. A calculated thickness of **0.38 inches** was calculated as the thickness. For consistency, this bearing was also switched to bronze. This was the [bearing](https://www.mcmaster.com/products/journal-bearings/shaft-diameter~1-4-1/length~1-4-2/) chosen.
## Decide

Now to design the assembly. The assembly will be in two parts with a snap-fit together. The material of the assembly will be 
## Communicate

