# Create Docker

From folder `dump_numpy/` run:
```bash
docker build . -t dump_numpy
docker run -v $(pwd):/home/jovyan/src/ -p 8888:8888  dump_numpy
```

# Summary
For a vector of size `(65000, 2048)`, `float32`, the results are:

|      	|  Pickle  	|   Numpy  	| Memmap 	|
|:----:	|:--------:	|:--------:	|:------:	|
| Save 	|  ~9 sec  	|  ~9 sec  	| ~9 sec 	|
| Load 	| ~3.5 sec 	| ~3.5 sec 	| ~11 ms 	|
| Size 	|  0.66 G  	|  0.66 G  	|  0.5 G 	|

Thus, in this case, it is more optimal to use `np.memmap` to save the vector and read it from disk. 


