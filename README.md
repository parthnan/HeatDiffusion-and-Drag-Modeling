# Heat Diffusion and Air Drag Modeling

Download the software at https://freefem.org/ and run the .edp files to see the animated simulation.

1.  About "wind_around_sphere.edp" : Modeling the airflow around a spherical aerofoil. Based on the Non stationary Navier-Stokes equation. Boundary conditions are such that airflow only enters from the left, and exits to the right. Each Simulation frame lasts 0.05 seconds(Δ𝑡=0.05).

Initial condition:	 𝑢=−𝑦(𝑦−5), 𝑣=0  , where Velocity; 𝒖=(𝑢,𝑣), Pressure=p

Boundary conditions:

𝑢_1=0, 𝑢_2=0 on Γ_top

𝑢_1=0, 𝑢_2=0, on Γ_bottom

𝑢_1=−𝑦(𝑦−5), 𝑢_2=0 on Γ_in  ,  meaning wind is the strongest at the center of the left boundary(windspeed follows parabolic curve)

(𝑝𝒏−1/Re(𝛻𝒖^𝐓)𝒏)"=0"　on Γ_out

𝑢_1=0, 𝑢_2=0 on Γ_sphere

Velocity increases in the Wind vector field from color Red(Lowest) to color Blue to color Purple/Pink(Highest).

![alt text](https://raw.githubusercontent.com/parthnan/HeatDiffusion-and-Drag-Modeling/master/winddiffusion.png)

2.  About "heat_inside_cuboid.edp" : Modeling the diffusion of heat(temperature) when heat is input through the bottom of a cuboid full of a material. Based on the Diffusion Equation. Boundary conditions are such that heat only enters from the bottom, and can exit from all other surfaces. Each Simulation frame lasts 0.05 seconds(Δ𝑡=0.05). Press Enter for simulation start.

Red is the Highest Temperature, Green the lowest.

![alt text](https://raw.githubusercontent.com/parthnan/HeatDiffusion-and-Drag-Modeling/master/heatdiffusion.png)
