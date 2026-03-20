# March 6th: Intial Sketches and Concepts
The overall idea is a high performance cartesian gantry that can replace voron gantries. 
Primarily intended for large builds where corexy belt lengths become determimental compared to x axis weight (>350mm). 

Heres the basic idea:
- Boxcart gantry means static y motors, and x motors mounted to the carriage
- Compatible with Voron frame sizes/extrusion lengths
- 2 * Nema 23 Y motors
- 2 * Nema 17 2504 X motors
- 9mm belts
- Future compatability with AWD Nema 17 Y

Also heres where I'll be taking inspiration from:
- General Concept: [CT300](https://www.printables.com/model/1112221-ct-300-3d-printer), it gets great IS results for a simple gantry
- Design practices / some belt spacing: [Monolith](https://github.com/Monolith3D/Monolith_Gantry)
- Belt tensioning: [Annex K3](https://github.com/Annex-Engineering/Gasherbrum-K3/tree/main)
- More design ideas: [Splendacross](https://github.com/Kizime123/Splendacross)

A couple of design constraints as a result:
- Y belt needs to be aligned with y carriage and com(Center of mass) of x assembly
- X belt is aligned with the center of MGN12 carraige for the toolhead
- Minimize idler count and belt length
- X tube length, hole spacing and mounting are standardized based on [voron](https://vorondesign.com/voron_trident)/monolith gantry

My main goal was to plan out where the y motors would be located and where everthing on the x joint would be layed out.

For the y motors it was pretty obvious, if I want compatiblity with flying gantries(V2.4), I needed to have spacing from the y extrusions. 
I basically just used where monolith's motors mounted to figure out where the y belts would meet at the xy joint.

The xy joints were a lot more difficult to work out. Based on the design constraints and a lot of messing around in CAD I came up with:

<img width="927" height="1040" alt="Screenshot 2026-03-06 235037" src="https://github.com/user-attachments/assets/04904476-e863-40d7-8886-340b7acc5468" />

So It looks complicated because I sketched out both the y belts and the x belts, which will be on stacked on top of each other.
The X belts will be inline with the X-tube, and wrap around the motor and a live idler. There is no tensioner since it adds complexity and is pretty simple to integrate into the toolhead.

The y belts will be above the x belts because the motors pull the center of mass about 10mm above the center of the x extrusion.
It has a tensioner integerated at the rear, and the front will have a static belt clamp.

**Total time spent: 7h**

# March 14th: XY Joint
I focused on getting all of the features of the xy joint done. 

<img width="824" height="644" alt="image" src="https://github.com/user-attachments/assets/2e395aac-8ef5-44b6-b6b2-5a2a9b234902" />
<img width="720" height="609" alt="image" src="https://github.com/user-attachments/assets/05f2e90e-bd14-45a2-a306-66f679dccdea" />
<img width="875" height="573" alt="image" src="https://github.com/user-attachments/assets/f6331657-4b53-4642-927b-d768419a5759" />

The y belt clearance, clamping and tensioning was the hardest part to integrate into the part. 

I'll just need to finish the part by adding chamfers and fillets, and I can move onto the y motor mounts.

**Total time spent: 8h**
