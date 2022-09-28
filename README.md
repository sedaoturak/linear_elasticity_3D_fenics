# Linear Elasticity Problem in 3D by FEniCS

This repository shows how to model a **three dimensional (3D)** part and simulate for a **linear elasticity** problem. [**FEniCS**](https://fenicsproject.org), Python based open-source partial differential equation software, is used to simulate the part, while 3D cylindrical part is modeled by [**pygmsh**](https://pygmsh.readthedocs.io/en/latest/) library -python package for gmsh software.

The code is written in Google Colab. The dependencies or installation details may change dor local machines or other platforms.

This example is expected to be helpful to students, researchers or anyone who starts to use FEniCS.

Any contribution is more than welcome!

## Geometry
The part is a cylinder with radius of 20 mm and height of 20 mm. It was created by using [**pygmsh**](https://pygmsh.readthedocs.io/en/latest/) library which is the Python interface of Gmsh mesh generator software.

<p float="center">
  <img src="https://user-images.githubusercontent.com/57313118/192842057-45319a3a-9365-4d12-9a99-5c180defb759.png" width="350" />
  <img src="https://user-images.githubusercontent.com/57313118/192843579-f42248b9-3209-414b-8030-ebf1d7077733.png" width="350" /> 
</p>

## Material
Material is chosen as aluminum to show the linear elasticity behaviour. 

## Problem Definition
The part is simulated under applied displacement in compression mode. There is also a mode for applying force application in the problem definition.

As boundary conditions, the bottom surface of the part is fixed in x, y and z directions, while on top, the surface is free in z direction and fixed in x and y directions.

<img width="400" alt="def" src="https://user-images.githubusercontent.com/57313118/192845321-bbd8183f-a096-4dcc-83a0-e9d18469f232.png">

## Visualizations
[**Plotly**](https://plotly.com) library is used to vusalize the part, mesh and the deformed body after the simulation.
