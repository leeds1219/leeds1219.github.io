---
layout: post
title:  "Z-Transform"
---

# Z-Transform

**Contents**
1. Definition, properties, convolution of z-Transfrom.
2. z-Domain versus frequency domain.
3. Filter design in z-Domain: Zeros and Poles of H(z).

Definition   

finite x[n] to z-transform X(z)   
x[n] -> X(z) into z domain   
X(z) -> x[n] back to time domain   
   
for a finite signal x[n] = b[0]d[n-0] + b[1]d[n-1]+ ... + b[L-1]d[n-L+1]   
   
Z-transform of x[n], System function   
X(z) = x[0]z^(-0) + x[1]z^(-1) + ... + x[L-1]z^(-L+1)   

z is a complex num, d is dirac delta function, b is the impulse response 
    
Properties   
   
1. Linearity   
   
2. Time-Delay   
   x[n[] = { 1 2 3 4 5 }
   let Y(z) = 0 z^0 + 1 z^(-1) + 2 z^(-2) + 3 z^(-3) + 4 z^(-4) + 5 z^(-5)
   Y(z) = z^(-1)X(z)
   x[n-1] <=> z^(-1)X(z)   

Convolution, z-transform of FIR filters   

FIR difference equation   
y[n] = b[0]x[n-0] + b[1]x[n-1] + ... + b[M]x[n-M]

x[n-k] = z^(-k)X(z)
H(z) = sum(b[k]z^(-k))

y[n] = sum(b[k]x[n-k])
Y(z) = H(z)X(z)   
   
Cascade system, LTI system

H(z) = H1(z)H2(z)   
   



