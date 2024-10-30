[![INFORMS Journal on Computing Logo](https://INFORMSJoC.github.io/logos/INFORMS_Journal_on_Computing_Header.jpg)](https://pubsonline.informs.org/journal/ijoc)

# From an Interior Point to a Corner Point: Smart Crossover

This archive is distributed in association with the [INFORMS Journal on
Computing](https://pubsonline.informs.org/journal/ijoc) under the [MIT License](LICENSE).

The software and data in this repository are a snapshot of the software and data
that were used in the research reported on in the paper 
[From an Interior Point to a Corner Point: Smart Crossover](https://doi.org/10.1287/ijoc.2022.0291) by Dongdong Ge, Chengwenjian Wang, Zikai Xiong, Yinyu Ye. 


**Important: This code is being developed on an on-going basis at 
https://github.com/tkralphs/JoCTemplate. Please go there if you would like to
get a more recent version or would like support**

## Cite

To cite the contents of this repository, please cite both the paper and this repo, using their respective DOIs.

https://doi.org/10.1287/ijoc.2022.0291

https://doi.org/10.1287/ijoc.2022.0291.cd

Below is the BibTex for citing this snapshot of the repository.

```
@misc{SmartCrossover,
  author =        {Ge, Dongdong and Wang, Chengwenjian and Xiong, Zikai and Ye, Yinyu},
  publisher =     {INFORMS Journal on Computing},
  title =         {{From an Interior Point to a Corner Point: Smart Crossover}},
  year =          {2024},
  doi =           {10.1287/ijoc.2022.0291.cd},
  url =           {https://github.com/INFORMSJoC/2022.0291},
  note =          {Available for download at https://github.com/INFORMSJoC/2022.0291},
}  
```

## Description

The goal of this software is to implement the crossover algorithms proposed in the paper.


## Building

Follow these steps to set up the environment:

1. Install Miniconda

You need to have [Miniconda](https://docs.conda.io/en/latest/miniconda.html) installed to manage the environment. Download and install Miniconda by following the [official instructions](https://docs.conda.io/en/latest/miniconda.html).

2. Clone the repository:
   ```
   git clone https://github.com/INFORMSJoC/2022.0291.git
   cd smart-crossover
   ```
3. Create the environment using `environment.yml`:
   ```
   conda env create -f environment.yml -n smart_crossover
   ```
   An important remark: we use Gurobi 9.0.3, Cplex 12.9.0, and Mosek 9.3.14 in this project. To recreate the results in this paper perfectly, you should add
   
   ```
     - gurobi=9.0.3
   ```
   to file `environment.yml` below `-dependencies:` and add
   ```
     - cplex=12.9.0
     - mosek=9.3.14
   ```
   below `-pip:`
   
4. Activate the environment:
   ```
   conda activate smart_crossover
   ```

To use the environment with Jupyter Notebook, install the environment as a Jupyter kernel when the environment is activated:

Install the Jupyter kernel:
  ```
  python -m ipykernel install --user --name=smart_crossover  
  ```


## Usage example

Open `/notebooks/example.ipynb`, activate the environment, and run the notebook to test the algorithm.

## Ongoing Development

This code is being developed on an on-going basis at the author's
[Github site](https://github.com/wcwj0147/smart-crossover).
