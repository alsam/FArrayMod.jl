This directory contains at the moment a translation of explicit upwind finite difference scheme for scalar law advection equation from
the book _Numerical Solution of Hyperbolic Partial Differential Equations_ by prof. John A. Trangenstein.


+ ./scalar_law/PROGRAM0/main.jl
    The original Fortran arrays  `u(-2:ncells+1), x(0:ncells), flux(0:ncells)` transformed to 1-based Julia arrays by shifting index expressions
```julia
    u    = Array(Float64, ncells+4)
    x    = Array(Float64, ncells+1)
    flux = Array(Float64, ncells+1)
```

+ ./scalar_law/PROGRAM0/main_farray.jl
    Exemplary usage of this package
```julia
    u    = FArray(Float64, -2:ncells+1)
    x    = FArray(Float64,  0:ncells)
    flux = FArray(Float64,  0:ncells)
```
