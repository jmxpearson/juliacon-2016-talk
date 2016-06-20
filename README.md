# VinDsl.jl: Fast and furious statistical modeling
(Slides and code for my talk at JuliaCon 2016)

## Abstract
Variational inference is a fast, scalable method for fitting complex statistical models to large and high-dimensional datasets. The repertoire of available algorithms and techniques is expanding rapidly, but most models are still coded by hand. The few automated implementations (e.g., in Stan) face a dual-language problem, and so are less suited to rapid development of new ideas. [VinDsl.jl](https://github.com/jmxpearson/VinDsl.jl) aims to provide a variational inference domain-specific language -- a set of data structures and macros for defining models -- in pure Julia. As a result, existing methods can be mixed and matched and new ones prototyped quickly, creating a thoroughly hackable toolbox for machine learning researchers. In this talk, I'll give an introduction to variational inference and sketch the philosophy and features of VinDsl, ending with applications to some problems in neuroscience.

## Following along
VinDsl currently makes use of some features of Distributions.jl that are not yet available on master, as well as the latest release of PDMats.jl. You will need to checkout the `jp/autodiff` branch of Distributions:
```julia
Pkg.clone("https://github.com/jmxpearson/VinDsl.jl")
Pkg.update()
Pkg.checkout("Distributions", "jp/autodiff")
```
