# geomodels
Representative models of geologic settings

## Why 

Having representative models of geologic settings that can be populated with physical properties is essential for developing an understanding of geophysical responses, how we might image these systems and where challenges may arise. Having a standard, accessible set of models is valueable for validating simulation software. The purpose of this repository is to be a resource that contains such models.

## Scope

- Representations of simple geologic models that can be populated with physical properties by unit and can be mapped to a mesh for simulations. 
- Can include surfaces and functions or mappings that describe physical property distributions in 3D space

## Not Goals

- performing numerical simulations and data analysis are outside of the scope of this repo

## Similar 

- SEG SEAM Models (http://seg.org/News-Resources/Research-Programs/SEAM) 

## A sketch of an idea 

```python
from geomodels import geothermal
import discretize

mesh = discretize.TensorMesh()
model = geothermal.CanonicalModel()
sigma = model.tomesh(mesh)
```
