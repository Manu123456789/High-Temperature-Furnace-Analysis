# 3D Heat Conduction Simulation

This project simulates the heat conduction in a three-dimensional object using the explicit central difference method in space for steady-state and transient analysis, employing the forward Euler method for time integration. It is developed in MATLAB and designed to offer insights into temperature distribution within materials under various boundary conditions.

## Features

- Simulates heat conduction in 3D using explicit central differences.
- Supports steady-state and transient time analysis with the forward Euler method.
- Allows configuration of material properties, domain size, and boundary conditions.
- Generates 3D visualizations of the temperature distribution within the object.
- Optional video recording of the simulation process.

## Material Properties

Currently, the script supports simulation for two materials:
- **Water**: A poor conductor of heat.
- **Copper**: An excellent conductor of heat.

The properties (thermal conductivity, specific heat, and density) for these materials are predefined, but you can easily modify the script to simulate heat conduction in other materials.

## Domain Configuration

The simulation domain dimensions, mesh resolution, and time step are configurable. The script includes an example of a 14 x 14 inch plate with a 3/4 inch depth, converted into meters for the simulation.

## Boundary Conditions

- **Dirichlet (1st type)**: Temperature is specified on the boundaries.
- **Neumann (2nd type)**: Heat flux is specified on some boundaries, demonstrating how to simulate insulated surfaces or apply specific heat fluxes.

## Visualization

The `plot3D_conduction.m` function is provided to visualize the temperature distribution within the 3D domain. It generates a 3D plot with isosurfaces corresponding to different temperature levels, providing a clear visual representation of the heat conduction process.

## Usage

1. Ensure MATLAB is installed on your system.
2. Place `conduction.m` and `plot3D_conduction.m` in your MATLAB workspace or a directory of your choice.
3. Open `conduction.m` in MATLAB and run the script. Modify the material properties, domain size, and boundary conditions as needed.
4. The simulation and visualization will start automatically. If enabled, a video file of the simulation will be saved in the same directory.

## Customization

You can customize the simulation by editing `conduction.m`:
- Change the material by editing the `material` variable.
- Adjust the domain size and mesh resolution according to your needs.
- Modify the boundary conditions to simulate different scenarios.

The `plot3D_conduction.m` function can also be customized to change the visualization appearance, such as the number of isosurfaces, color schemes, and camera angle.




