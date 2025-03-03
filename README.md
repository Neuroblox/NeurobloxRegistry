# NeurobloxRegistry

### Adding the Neuroblox Registry

This is the [registry](https://pkgdocs.julialang.org/v1/registries/) that allows you to easily install [Neuroblox.jl](https://github.com/Neuroblox/Neuroblox.jl) in Julia.

To add the NeurobloxRegistry simply open julia and execute

``` julia
using Pkg
pkg"registry add https://github.com/Neuroblox/NeurobloxRegistry"
```
and then the NeurobloxRegistry will be installed and active on your machine. 

If this is the first time you have used Julia on your current machine, you *may* also need to add the [General Registry](https://github.com/JuliaRegistries/General) which can be done with

``` julia
pkg"registry add General"
```

Once this is done, you'll be able to add Neuroblox.jl just like any other julia package, e.g.

``` julia
using Pkg
Pkg.add("Neuroblox")
```
or
``` julia
using Pkg
pkg"add Neuroblox"
```
or from the package-manager REPL mode (entered by hitting `]` in the regular Julia REPL)
``` julia
pkg> add Neuroblox
```




### Removing the Neuroblox registry

If you need to remove the NeurobloxRegistry for whatever reason, you can run

``` julia
using Pkg
pkg"registry remove NeurobloxRegistry"
```

If for some reason that does not work, you can remove the file `NeurobloxRegistry` from your `.julia/registries` folder manually (see https://docs.julialang.org/en/v1/base/constants/#Base.DEPOT_PATH for more info on the `.julia` folder).
