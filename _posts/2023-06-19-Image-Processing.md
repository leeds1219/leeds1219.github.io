---
layout: post
title:  "Image Processing"
---

1. Preprocessing

Slice timing: time shift

Motion correction: rigid transformation

Coregistration: Converts the images into the spatial coordinates using unique property of an image as the landmark

Normalization: normalize into a common spatial reference space

Spatial Smoothing: such as Gaussian filter

2. Statistical analysis

The General Linear Model

2.1 Simple Linear Regression

Y = β0 + X1β1 + ϵ

The indepdent variable, X1 = [x1, x2,⋯, xn]T represent the presence or absence of a particular experimental condition

The dependent variable, Y = [y1, y2,⋯, yn]T represent mesured fMRI siganl at series of time points

β0 is the difference in average value between the two vectors

ϵ is the variation in reaction time that is not captured by the beta parameters

2.2 Multiple Linear Regression

Y = β0 + Xβ + ϵ

X = [X1, X2,⋯, Xp] 
Xp = [x1p, x2p,⋯, xnp]T
p is the number of independent variables 

2.3 General Linear Model

The multiple regression model applied to fMRI data is typically referred to as the general linear model (GLM)

Y is the fMRI signal
X is the design matrix with independent variables
β is the parameters
ϵ is the residual s

GLM is applied to the individual voxels

2.4 Data Cleaning prior to GLM

High-pass filtering 

2.5 Correlation btw predictors

2.6 T-Contrast

t-test 

3. Statistical inference


