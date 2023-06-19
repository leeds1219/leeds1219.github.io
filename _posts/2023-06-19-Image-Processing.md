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

figure 1. (add image)

example
A block design of 15s, three continuous time series, 
each condition presented in 4 times/blocks

the other six colums per run show the nuisance regressors and the motion correction parameters from the alignment of fMRI data

the last three columns in the design matrix model shows the potential differences in the signal btw runs

2.6 Significance test & Interpretation
2.6.1 Parametric tests

t-test: ratio of beta to error in a voxel
F-ratio :
ANOVA : 

2.6.2 Non-parametric tests

null hypothesis significance testing(NHST)
Bayesian statistics

2.7 Multiple comparisons problem
p-value: probability that the H0 is true
type-1 error: H0 is true but rejected 

2.7.1 Bonferroni correction
type 1 error/number of voxels
FWE correction: family of voxels

2.7.2 Faulse discovery rate
FDR less conservative than FWE

2.7.3 Uncorrected threshold

Second-Level Whole-Brain Analyses

Region of Interest(ROI) Analyses
avoids the problem of inter‑individual variability in anatomy but only provide a very local view of the data

Double Dipping & Circular Analyses

Double dipping: refers to a situation where data is used multiple times in the same analysis or for multiple analyses, leading to potential biases or inflated statistical significance.

Circular analysis: also known as circular reasoning or circularity, refers to a logical fallacy in which the conclusion of an argument is assumed or presupposed in one or more of the premises.

3. Statistical inference
Forward inference: If process X is manipulated, then
region R is activated; thus, the activation of region R is related to process X

Reverse inference: Results show an activation of region R, among other activations. Other studies in the literature have activated region R when they manipulated process X. Thus, the activation of region R in the current study is related to process X


Summary 
Data analysis starts with image processing, including slice timing, motion correction, coregistration, normalization, and spatial smoothing.
During all steps, it is important to perform quality control and consider whether the appropriate parameter settings are being used.
Each step can influence the end result, necessitating transparency about which parameters have been used and why
Statistics are typically based on a regression model referred to as the general linear model.
Correction for multiple comparisons is needed when determining the significance of the results.
One should avoid performing circular analyses in which knowledge about the results
of initial analyses influences how later analyses are performed.
Statistical inference is preferably based on forward inference, and proper caution
should be used in the case of reverse inference.

