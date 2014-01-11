FArrayMod.jl
============

provides the ability to use arbitrary starting indices for arrays in Julia programming language.

```jlcon
julia> import FArrayMod

julia> using FArrayMod

julia> y = FArray(Float64, -1:1, -7:7, -128:512, -5:5, -1:1, -3:3, -2:2, -1:1);

julia> y[-1,-7,-128,-5,-1,-3,-2,-1] = 14
14

julia> y[-1,-7,-128,-5,-1,-3,-2,-1] += 5
19.0
```
