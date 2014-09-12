# CUBLAS implementation progress

The following sections list the CUBLAS functions shown on the CUBLAS
documentation page:

http://docs.nvidia.com/cuda/cublas/index.html

## Level 1 (13 functions)

CUBLAS functions:

* [x] amax
* [x] amin
* [x] asum
* [x] axpy
* [x] copy
* [x] dot, dotc, dotu
* [x] nrm2
* [ ] rot (not implemented in julia blas.jl)
* [ ] rotg (not implemented in julia blas.jl)
* [ ] rotm (not implemented in julia blas.jl)
* [ ] rotmg (not implemented in julia blas.jl)
* [x] scal
* [ ] swap (not implemented in julia blas.jl)

## Level 2

Key:
* `ge`: general
* `gb`: general banded
* `sy`: symmetric
* `sb`: symmetric banded
* `sp`: symmetric packed
* `tr`: triangular
* `tb`: triangular banded
* `tp`: triangular packed
* `he`: hermitian
* `hb`: hermitian banded
* `hp`: hermitian packed

CUBLAS functions:

* [x] gbmv (in julia/blas.jl)
* [x] gemv (in julia/blas.jl)
* [ ] ger (in julia/blas.jl)
* [x] sbmv (in julia/blas.jl)
* [ ] spmv
* [ ] spr
* [ ] spr2
* [x] symv (in julia/blas.jl)
* [ ] syr (in julia/blas.jl)
* [ ] syr2
* [ ] tbmv
* [ ] tbsv
* [ ] tpmv
* [ ] tpsv
* [ ] trmv (in julia/blas.jl)
* [ ] trsv (in julia/blas.jl)
* [*] hemv (in julia/blas.jl)
* [ ] hbmv
* [ ] hpmv
* [ ] her (in julia/blas.jl)
* [ ] her2
* [ ] hpr
* [ ] hpr2

## Level 3

CUBLAS functions:

* [ ] gemm (in julia/blas.jl)
* [ ] gemmBatched
* [ ] symm (in julia/blas.jl)
* [ ] syrk (in julia/blas.jl)
* [ ] syr2k (in julia/blas.jl)
* [ ] syrkx
* [ ] trmm (in julia/blas.jl)
* [ ] trsm (in julia/blas.jl)
* [ ] trsmBatched
* [ ] hemm
* [ ] herk (in julia/blas.jl)
* [ ] her2k (in julia/blas.jl)
* [ ] herkx

## BLAS-like extensions

* [ ] geam
* [ ] dgmm
* [ ] getrfBatched
* [ ] getriBatched
* [ ] geqrfBatched
* [ ] gelsBatched
* [ ] tpttr
* [ ] trttp