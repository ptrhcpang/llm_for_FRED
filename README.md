## A nanoGPT for FRED data
This is an adaptation of Karpathy's nanogpt project 
(https://github.com/karpathy/ng-video-lecture) 
for financial time series predictions using data 
pulled from [FRED](https://fred.stlouisfed.org/).

## Aims

The aim of this project was for me to learn 
how to code the attention mechanism. 

This was applied to prediction of the 
10 year minus 3 month US treasury yield spread.

## Contents

The contents of this project are heavily based 
on Karpathy's nanogpt project 
(https://github.com/karpathy/ng-video-lecture). 
Some tweaks for the time series data 
include: 
 1. a preamble that converts data into a vector of increments,
 2. a simplified tokeniser, 
 3. using 2nd order Runge-Kutta stepping instead of
    a standard residual connection (which is an explicit Euler scheme),
 4. commenting out some dropout layers except
    in the feed forward layer, where the dropout
    layer is between the activation function and
    a final linear layer, which seems to improve performance,
 5. modifications in the training loop for convenience,
 6. code for plotting comparison of
    predicted spread with realised spread.

## Licence

[MIT](https://opensource.org/license/mit)
