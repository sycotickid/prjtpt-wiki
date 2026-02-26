A tool for building / placing bodies of water (lakes and rivers) using beziar curves and basic shapes to define where water is placed and simple parameters like width to define the size of rivers around the curves and the size of lakes around their shape. Including a system that connects the curves to the shapes and a shader that displays water seamlessly from rivers to lakes etc. potentially include an area system that allows for these shapes to define depth and additional behavior modifiers like gravity, blurring or rippling, and setting additional flags for character behavior. 

![Attachment.png](blob:capacitor://localhost/558e3d20-5987-4bf9-bcb4-3271898e0b97)

Points on the Bézier curve can denote where the center of the river is with a radius parameter controlling how far each vertex should be placed away from the curve point. At least two points will be needed to generate vertices so that the cross product of the line can be used to set the direction of the radius.

Whether or not 2D shapes as bodies of water can connect to the bezier rivers, a shader should be built to seamlessly display stylized water across rivers and lakes (and show ripples when the water mesh intersects with land)

Can be used to create various rivers and lakes in [[Journal]]