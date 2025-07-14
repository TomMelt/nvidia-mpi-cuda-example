# nvidia-mpi-cuda-example

This example was taken from NVIDIA's [multi-gpu-programming-models](https://github.com/NVIDIA/multi-gpu-programming-models) example.

I had to make a few minor changes so that we can debug the kernel code.

I have included the original [LICENSE.md](./LICENSE.md).

To build this code:

```
$ make
```

To run the code:

```
$ mpirun -n 2 ./jacobi
```

To debug this code with [mdb](https://github.com/TomMelt/mdb) us the following command

```
mdb launch -n 2 -b cuda-gdb -t ./jacobi
```
