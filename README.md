# Dataset of A Transfer Learning Hyper-heuristic Approach for Automatic Tailoring of Unfolded Population-based Metaheuristics
This repository contains the resulting dataset of A Transfer Learning Hyper-heuristic Approach for Automatic Tailoring of Unfolded Population-based Metaheuristics presented in CEC22. We also included the main python file to plot the figures thereby presented.

## Requirements
- Python v3.7+
- [CUSTOMHyS framework](https://github.com/jcrvz/customhys.git)
- Standard modules: os, matplotlib, seaborn, numpy, pandas, scipy.stats

## Files
- Main script: 
- Results for population size of 30 agents: 
- Results for population size of 50 agents: 
- Results for population size of 100 agents: 
- Results for basic metaheuristics: 
- Collection of basic metaheuristics:
- Collection of default heuristics: 

## Structure of datasets

The experiments were saved in JSON files. [Further information can be found here](https://www.sciencedirect.com/science/article/pii/S2352711020303411). The data structure of saved files follows the particular scheme described below.

<details>
<summary> Expand structure </summary>
<p>

```
|-- {dict: 3}
|  |-- problem = {list: 428}
|  |  |-- 0 = {str}
:  :  :  
|  |-- dimensions = {list: 428}
|  |  |-- 0 = {int}
:  :  :  
|  |-- results = {list: 428}
|  |  |-- 0 = {dict: 5}
|  |  |  |-- step = {list: 12}
|  |  |  |  |-- 0 = {int}
:  :  :  :  :  
|  |  |  |-- performance = {list: 12}
|  |  |  |  |-- 0 = {float}
:  :  :  :  :  
|  |  |  |-- statistics = {list: 12}
|  |  |  |  |-- 0 = {dict: 10}
|  |  |  |  |  |-- nob = {int}
|  |  |  |  |  |-- Min = {float}
|  |  |  |  |  |-- Max = {float}
|  |  |  |  |  |-- Avg = {float}
|  |  |  |  |  |-- Std = {float}
|  |  |  |  |  |-- Skw = {float}
|  |  |  |  |  |-- Kur = {float}
|  |  |  |  |  |-- IQR = {float}
|  |  |  |  |  |-- Med = {float}
|  |  |  |  |  |-- MAD = {float}
:  :  :  :  :  
|  |  |  |-- encoded_solution = {list: 12}
|  |  |  |  |-- 0 = {list: 50}
|  |  |  |  |  |-- 0 = {int}
:  :  :  :  :  :  
:  :  :  :  :  
|  |  |  |-- hist_fitness = {list: 50}
|  |  |  |  |-- 0 = {list: 98}
|  |  |  |  |  |-- 0 = {float}
:  :  :  :  :  :  
:  :  :  :  :  
:  :  :  
```
</p>
</details>

## Contact information

Jorge M. Cruz-Duarte - [jcrvz.co](https://jcrvz.co), [jorge.cruz@tec.mx](mailto:jorge.cruz@tec.mx)

Distributed under the MIT license. See [LICENSE](./LICENSE) for more information.
