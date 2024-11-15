## Data preparation

1. Min-cost flow instances:
    - Download the GOTO min-cost flow instances from [here](http://lime.cs.elte.hu/~kpeter/data/mcf/goto/) to folder `data/goto`. 
The instances are in the format of `*.min`. Transfer them to the format of `*.mcf` by running `scripts/min2mcf.py`.
    - Download the benchmark problems from [here](https://plato.asu.edu/ftp/lptestset/network/) to folder `data/mcf`.

2. Optimal transport instances:
   - Download the MNIST dataset from [here](http://yann.lecun.com/exdb/mnist/) to folder `data/mnist`.
Create folder `data/ot_mnist` and run `scripts/mnist2ot.py` to generate the optimal transport instances.

3. LP instances:
   - Download the LP instances from [here](https://plato.asu.edu/ftp/lpopt.html) to folder `data/lp`.
Then use `file_handler.FileHandler.write_presolved_models` to generate the presolved instances.
