# Steady state seepage validation

## Summary

We tested Gofer’s **steady state seepage** (SSS) features by modelling a homogenous and isotropic material earth dam placed on top of an assumed horizontal impervious layer. The model contains set boundary conditions and a drain at the downstream toe of the proposed structure.

This example is used to validate a comparison of results from **Gofer**, **Oasys Slope** and **Plaxis**.

Our example model geometry is taken from Milton E. Harr’s [_Groundwater and Seepage._](https://www.worldcat.org/title/groundwater-and-seepage/oclc/489956), Milton E. Harr (1962; rev. 1990).

A summary of the geometry and key parameters is presented below:

<<<<<<< HEAD
![cross-section-dam](https://b2c-templates-arup.s3-eu-west-1.amazonaws.com/gofer/validationImages/Smaller-slide-1-original-sss-validation-model.png)

_The graph shows a cross-section of a dam_
_Fig 2: A table showing silt sand permeability_

![parameters](https://b2c-templates-arup.s3-eu-west-1.amazonaws.com/gofer/validationImages/sand-permeability-table.png)

> > > > > > > 53180c2e211a03032b0de41dc04bd0a28958087d

## What is it?

The modelling of boundary conditions such as injection, sink points and lines, and constant head/flow boundaries, etc. enables engineers to estimate the water free surface.

In turn, this information is used to derive credible porewater pressures in a ground model system; to estimate ground pressures accurately, or produce meaningful slope stability analyses.

Gofer creates plots of various magnitudes including: _porewater pressures, head, hydraulic gradient, and seepage velocities._

## Steady state seepage in Gofer

- Gofer’s steady state seepage capabilities are found in the **Configure stages** mode, under **Stage settings**.

- The user controls the mesh element size by selecting and setting neighbouring element sizes (in m) at relevant nodes.

- Steady state seepage calculations can be activated at any stage if they are set as **Staged construction**.

- **C-phi analysis** stages do not run a steady state seepage calculation. These can inherit the results of generated porewater pressures from previously run steady state seepage stages.

- To activate the steady state seepage calculations, users must switch on the relevant boundary conditions within **Configure stages**. The selected boundary conditions then visually change from dashed to solid lines.
- Gofer’s SSS capabilities are found in the **Configure stages** mode, under **Stage settings**.

- The user controls the mesh element size by selecting and setting neighbouring element sizes (in m) at relevant nodes.

- SSS calculations can be activated at any stage if they are set as **Staged construction**.

- **C-phi analysis** stages do not run a SSS calculation. These can inherit the results of generated porewater pressures from previously run SSS stages.

- To activate the SSS calculations, users must switch on the relevant boundary conditions within **Configure stages**. The selected boundary conditions then visually change from dashed to solid lines.

- In the **Results** mode, users can generate a variety of plots to display magnitudes such as piezometric head, porewater pressures, seepage velocity and hydraulic gradient.

## How it compares: Analytical solution

In _Groundwater and Seepage_, Harr presents the case of an earth dam, with no low permeability core. The dam is composed of a single material with isotropic hydraulic conductivity, on top of an impervious base. A toe filter is installed at the downstream toe.

The computed analytical solution for this problem is a match like-for-like with Oasys Slope and Plaxis. We have visualised an approximation of the coefficients provided in Figure 8-11 (Harr, 1990, p.222), which accounts for some slight discrepencies.

These images below show the computed analytical solution plotted on top of the Gofer and Oasys Slope and Plaxis output.

![gofer-case](https://b2c-templates-arup.s3-eu-west-1.amazonaws.com/gofer/validationImages/Smaller-slide-2-Gofer-case-sss.png)

_Analysis results in Gofer_

![slope-case](https://b2c-templates-arup.s3-eu-west-1.amazonaws.com/gofer/validationImages/Smaller-slide-3-Slope-case-sss.png)

_Analysis results in Oasys Slope_

![plaxis-case](https://b2c-templates-arup.s3-eu-west-1.amazonaws.com/gofer/validationImages/Smaller-slide-4-Plaxis-case-sss.png)

_Analysis results in Plaxis_
The computed analytical solution for this problem is a match like-for-like with Gofer, Oasys Slope and Plaxis. We have visualised an approximation of the coefficients provided in Figure 8-11 (Harr, 1990, p.222), which accounts for some slight discrepencies.

These figures show the computed analytical solution plotted on top of the Gofer and Oasys Slope output.

_Fig 3: Analysis results in Gofer_

![gofer-case](https://b2c-templates-arup.s3-eu-west-1.amazonaws.com/gofer/validationImages/Slide-2-Gofer-case-sss.png)

_Fig 4: Analysis results in Oasys Slope_

![slope-case](https://b2c-templates-arup.s3-eu-west-1.amazonaws.com/gofer/validationImages/Slide-3-Slope-case-sss.png)

_Fig 5: Analysis results in Plaxis_

![plaxis-case](https://b2c-templates-arup.s3-eu-west-1.amazonaws.com/gofer/validationImages/Slide-4-Plaxis-case-sss.png)

## How it compares: Oasys Slope and Plaxis

The porewater pressure results attained from Oasys Slope and Plaxis were a match for both the analytical solution and Gofer.

![gofer-slope](https://b2c-templates-arup.s3-eu-west-1.amazonaws.com/gofer/validationImages/Smaller-slide-5-Gofer-slope-sss.png)

_Gofer and Oasys Slope comparison_

![gofer-plaxis](https://b2c-templates-arup.s3-eu-west-1.amazonaws.com/gofer/validationImages/Smaller-slide-6-Gofer-plaxis-sss.png)

_Gofer and Plaxis comparison_
_Fig 6: Gofer and Oasys Slope comparison_

![gofer-slope](https://b2c-templates-arup.s3-eu-west-1.amazonaws.com/gofer/validationImages/Slide-5-Gofer-slope-sss.png)

_Fig 7: Gofer and Plaxis comparison_

![gofer-plaxis](https://b2c-templates-arup.s3-eu-west-1.amazonaws.com/gofer/validationImages/Slide-6-Gofer-plaxis-sss.png)
