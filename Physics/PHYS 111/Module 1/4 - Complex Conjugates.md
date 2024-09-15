**Note: Uses desmos-generated graphs.

Notation for conjugates:
$$
z*=\bar{z}=x-iy
$$
Note that
$$
Re(z) = Re(z*), \,\,\, Im(z)=-Im(z)
$$
Because of this, a complex conjugate (on the plane) is a reflection of the original complex number along the x-axis:
```desmos-graph
	y=x|blue|dashed|0<=y<=2
	(2,2)|blue|label:`z`

	y=-x|blue|dashed|0<=x<=2
	(2,-2)|blue|label:`z*`
```

Because of the stated properties of the real and imaginary parts, if $z$ is real (meaning $Im(z)=0$, then $z*=z$.