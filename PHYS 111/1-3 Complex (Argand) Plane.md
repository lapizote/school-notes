**Note: Uses desmos-generated graphs, if you are using Obsidian make sure you have internet.**

Since a complex number $z$ can be said to have two parts $x$ and $y$ ($Re(z)$ and $Im(z)$ respectively), we can represent it in a complex number plane (also known as an Argand plane).

This plane works the same way as cartesian plane, with the only difference being that the x-axis represents the value of $Re(z)$ and the y-axis represents the value of $Im(z)$.

For example, given the complex numbers $z=3+2i$, $z=-5i$, and $z=-2+i$:
```desmos-graph
	y=(2/3)x|blue|dashed|0<=y<=2
	(3,2)|blue|label:`3+2i`

	y=(-1/2)x|blue|dashed|0<=y<=1
	(-2,1)|blue|label:`-2+i`

	x=0|blue|dashed|-5<=y<=0
	(0,-5)|blue|label:`-5i`
```

To get the magnitude (length) of a complex number from the origin, we simply use
$$
|x+iy|=\sqrt{x^2+y^2}.
$$
(Note that this is similar to how a magnitude in a [[Finding magnitudes of a vector|vector]] is found.)

#### Useful things about complex number graphs
---
1. Since addition and subtraction of complex numbers is simply the addition and subtraction of its components, they can be visualized as such:
	- For addition:
	![[vector-addition.png|400]]
	
	- For subtraction:
	![[vector-subtraction.png|400]]

2. Since [[1-4 Complex Conjugates|complex conjugates]] only differ by a negative imaginary part, we can say that it is a reflection of the original complex number along the x-axis.
