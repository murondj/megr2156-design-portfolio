# A6 – Bracket Drawings

## Objective

1.) Create an accurate and comprehensive model of the previous assignment Bracket Design.

2.) Construct drawings from model and adhere to engineering standards. Identify tolerancing and other important features to the model.

3.) Reflect on design and lessons learned from this topic

## Analyze

This assignment is a follow-up to the previous assignment done in A5. Using the measurements acquired from the failure due to stress, a CAD model  using parametric equations will be constructed and then a drawing of the design will be made from this model. Here are the parameters used for constructing the bracket.

### CAD Model
<img width="2374" height="1242" alt="image" src="https://github.com/user-attachments/assets/7f4ea777-1c16-4a59-9c21-8cb7cb2fff2c" />

Starting with feature A, the design will be built in part order. 

<img width="2874" height="1328" alt="image" src="https://github.com/user-attachments/assets/1e0cea0c-3ead-4431-a8f3-df0c9c44aab2" />

Feature B is added using the parametric equations.

<img width="2870" height="1314" alt="image" src="https://github.com/user-attachments/assets/9764f321-ee97-4acc-9ba2-8bb768db5042" />

Feature C is added next to the part using the parametric equations

<img width="2868" height="1326" alt="image" src="https://github.com/user-attachments/assets/06f40b96-14f5-4fe3-8877-dc0c894ecf08" />

Feature D and E are added and now it is time to use the mirror tool to mirror to the opposite side.

<img width="2876" height="1322" alt="image" src="https://github.com/user-attachments/assets/c3a0ec0c-367e-414d-bc54-37254fffd127" />

Once that is done, the bracket is finished. This is the final result.

<img width="2872" height="1312" alt="image" src="https://github.com/user-attachments/assets/43a63f05-f63d-41b8-a260-ce908643ff0c" />

Checking with the measurements from assignment 5, they are all nearly identical except for the length of part E. Noticing that the original one inch measurement closes the gap too much, the measurement is reconstructed to 0.767 inches. Reworking the math, the new thickness can actually be smaller, down to 0.26 inch thickness for Feature E. The updated part and parameters are shown below.

<img width="2880" height="1314" alt="image" src="https://github.com/user-attachments/assets/2cd80dfd-9d50-4b9b-97d9-89aef7f6e808" />


<img width="2352" height="1138" alt="Screenshot 2026-09-30 220439" src="https://github.com/user-attachments/assets/e41fff9b-358b-4420-9d1e-db8efb1d0264" />

### CAD Drawing

This is the final drawing for the bracket. All the measurements of the design were based on the stress failure of the material since it was the weaker and more likely to fail sizes. All the measurements were expressed in the parametric equation, meaning if a measurement needed to be changed, it had to be changed directly in the parameters window. This is what happened when the error was caught about the sizing of the gap between the rails at the top being too small. Once it was changed in the parametric formula, it was applied across the whole model and since the mirror tool was used, it applied to the other side of the model as well.




<img width="1516" height="1182" alt="image" src="https://github.com/user-attachments/assets/6abd6411-c453-4e03-a835-2da9aecad7e3" />


## Decide
Tolerancing on the 1.50 inch measurement is tighter due to the significance of the clutch on the beam. If this measurement has a loose fit, the bracket will not grab as hard and could slide off too easily. It is a tolerance down to the thousandth of an inch and it can only be 1.499 inches. This gives maximum clutch power while also still being able to slide. For feature B, this measurement has been allowed a standard tolerance, as it being slightly smaller or larger does not have a huge effect on the design, since the part was already sized up to begin with. 

### Link Fit

#### CAD Model

This is the design for the link fit. Using the measurements calculated in the previous assignment, the link is created with two holes. Since the first hole is running an R4 fit, it is sized up to 0.626 inches to allow for a sliding fit. The bottom hole stays the same since it is a press fit. The corners of the link are filleted so that it allows for a more sleek design while not compromising the structural integrity. The hole locations are on center and 1 inch away from the top and from the bottom, giving the max amount of contact material for the holes to have. 

<img width="2380" height="1254" alt="image" src="https://github.com/user-attachments/assets/d31ff93d-8d8f-4a9f-a514-8ba763e1f027" />

<img width="2872" height="1326" alt="image" src="https://github.com/user-attachments/assets/a9346d2a-0237-4fd7-aa17-f255ad33a46d" />

#### CAD Drawing

The drawing on the CAD model has two hole callouts with ASME Y14.5 standards. These show the position of the object, that it is a diameter cut, the tolerance of the hole, the class fit of the hole, and the datum point. On the top hole the tolerance is minus 0.001 because the hole was sized up and if it was made larger, the fit would be too loose. The larger hole is an FN class fit, so the tolerancing was plus 0.0005 .

<img width="1578" height="1220" alt="image" src="https://github.com/user-attachments/assets/516f1a0b-078e-4e06-b122-a54f609ccdbf" />




## CAD FILES 
## Communicate

### Reflections and Insight

This assignment shows how to take a design on paper and model it to create a product. It is important to understand how to correctly model something, but also identify where it is most efficient to cut down on something to save costs, or pay very close attention to a feature so that the design does not fail. Tolerancing and fitting is very important on how a design operates, and modeling the design allows for mistakes to be caught and for modifications before the product is manufactured. Tolerancing is also important to how the design interacts with other features. Being able to identify when a tolerance needs to be strict or loose is very important to the functionality of the design. 


This assignment took 3 hours over the course of one day.
