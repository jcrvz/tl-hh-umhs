<<<<<<< HEAD:README.md
# Unfolded Metaheuristics - Results
=======
<<<<<<< HEAD
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
=======
# customhys
>>>>>>> origin/main:README-customhys.md

This repository contains the resulting datasets of the **A Transfer Learning Hyper-heuristic Approach for Automatic Tailoring of Unfolded Population-based Metaheuristics** presented in *CEC-22*. We also included the main python file to plot the figures thereby presented. 

## Requirements
- Python v3.7+
- [CUSTOMHyS framework](https://github.com/jcrvz/customhys.git)
- Standard modules: os, matplotlib, seaborn, numpy, pandas, scipy.stats

## Files
- **Main notebook**: [paper_transferlearning_exp1.ipynb](./paper_transferlearning_exp1.ipynb)
- Code for generating weight matrices: [paper_transferlearning_part1.py](./paper_transferlearning_part1.py)
- Visualization of transfer learning matrices: [data_files/transfer_learning](./data_files/transfer_learning) 
- Results from the proposed approaches: [data_files/exp_output](./data_files/exp_output)
- Raw figures generated from the main notebook: [data_files/exp_figures](./data_files/exp_figures)
- Experimental configurations used in this work: [exconf](./exconf)
- Results for basic metaheuristics: [data_files/basic-metaheuristics-data_v2.json](./data_files/basic-metaheuristics-data_v2.json)
- Collection of basic metaheuristics: [collections/basicmetaheuristics.txt](./collections/basicmetaheuristics.txt)
- Collection of default heuristics: [collections/default.txt](./collections/default.txt)

## Contact information

Jorge M. Cruz-Duarte - [jcrvz.co](https://jcrvz.co), [jorge.cruz@tec.mx](mailto:jorge.cruz@tec.mx)

Distributed under the MIT license. See [LICENSE](./LICENSE) for more information.

<<<<<<< HEAD:README.md
=======
![Module Dependency Diagram](docfiles/dependency_diagram.png)

**NOTE:** Each module is briefly described below. If you require further information, please check the corresponding source code.

### 🤯 Problems (benchmark functions)

This module includes several benchmark functions as classes to be solved by using optimisation techniques. The class structure is based on Keita Tomochika's repository [optimization-evaluation](https://github.com/keit0222/optimization-evaluation).

Source: [``benchmark_func.py``](./benchmark_func.py)

### 👯‍♂️ Population

This module contains the class Population. A Population object corresponds to a set of agents or individuals within a problem domain. These agents themselves do not explore the function landscape, but they know when to update the position according to a selection procedure.

Source: [``population.py``](./population.py)

### 🦾 Search Operators (low-level heuristics)

This module has a collection of search operators (simple heuristics) extracted from several well-known metaheuristics in the literature. Such operators work over a population, i.e., modify the individuals' positions. 

Source: [``operators.py``](./operators.py)

### 🤖 Metaheuristic (mid-level heuristic)

This module contains the Metaheuristic class. A metaheuristic object implements a set of search operators to guide a population in a search procedure within an optimisation problem.

Source: [``metaheuristic.py``](./metaheuristic.py)

### 👽 Hyper-heuristic (high-level heuristic)

This module contains the Hyperheuristic class. Similar to the Metaheuristic class, but in this case, a collection of search operators is required. A hyper-heuristic object searches within the heuristic space to find the sequence that builds the best metaheuristic for a specific problem.

Source: [``hyperheuristic.py``](./hyperheuristic.py)

### 🏭 Experiment

This module contains the Experiment class.  An experiment object can run several hyper-heuristic procedures for a list of optimisation problems.

Source: [``experiment.py``](./experiment.py)

### 🗜️ Tools

This module contains several functions and methods utilised by many modules in this package.

Source: [``tools.py``](./tools.py)

### 💾 Data Structure

The experiments are saved in JSON files. The data structure of a saved file follows a particular scheme described below.
>>>>>>> tl-hh-umhs

<details>
<summary> Expand structure </summary>
<p>

```
<<<<<<< HEAD
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
=======
data_frame = {dict: N}
|-- 'problem' = {list: N}
|  |-- 0 = {str}
:  :
|-- 'dimensions' = {list: N}
|  |-- 0 = {int}
:  :
|-- 'results' = {list: N}
|  |-- 0 = {dict: 6}
|  |  |-- 'iteration' = {list: M}   
|  |  |  |-- 0 = {int}
:  :  :  :
|  |  |-- 'time' = {list: M}
|  |  |  |-- 0 = {float}
:  :  :  :
|  |  |-- 'performance' = {list: M}
|  |  |  |-- 0 = {float}
:  :  :  :
|  |  |-- 'encoded_solution' = {list: M}
|  |  |  |-- 0 = {int}
:  :  :  :
|  |  |-- 'solution' = {list: M}
|  |  |  |-- 0 = {list: C}
|  |  |  |  |-- 0 = {list: 3}
|  |  |  |  |  |-- search_operator_structure
:  :  :  :  :  :
|  |  |-- 'details' = {list: M}
|  |  |  |-- 0 = {dict: 4}
|  |  |  |  |-- 'fitness' = {list: R}
|  |  |  |  |  |-- 0 = {float}
:  :  :  :  :  :
|  |  |  |  |-- 'positions' = {list: R}
|  |  |  |  |  |-- 0 = {list: D}
|  |  |  |  |  |  |-- 0 = {float}
:  :  :  :  :  :  :
|  |  |  |  |-- 'historical' = {list: R}
|  |  |  |  |  |-- 0 = {dict: 5}
|  |  |  |  |  |  |-- 'fitness' = {list: I}
|  |  |  |  |  |  |  |-- 0 = {float}
:  :  :  :  :  :  :  :
|  |  |  |  |  |  |-- 'positions' = {list: I}
|  |  |  |  |  |  |  |-- 0 = {list: D}
|  |  |  |  |  |  |  |  |-- 0 = {float}
:  :  :  :  :  :  :  :  :
|  |  |  |  |  |  |-- 'centroid' = {list: I}
|  |  |  |  |  |  |  |-- 0 = {list: D}
|  |  |  |  |  |  |  |  |-- 0 = {float}
:  :  :  :  :  :  :  :  :
|  |  |  |  |  |  |-- 'radius' = {list: I}
|  |  |  |  |  |  |  |-- 0 = {float}
:  :  :  :  :  :  :  :
|  |  |  |  |  |  |-- 'stagnation' = {list: I}
|  |  |  |  |  |  |  |-- 0 = {int}
:  :  :  :  :  :  :  :
|  |  |  |  |-- 'statistics' = {dict: 10}
|  |  |  |  |  |-- 'nob' = {int}
|  |  |  |  |  |-- 'Min' = {float}
|  |  |  |  |  |-- 'Max' = {float}
|  |  |  |  |  |-- 'Avg' = {float}
|  |  |  |  |  |-- 'Std' = {float}
|  |  |  |  |  |-- 'Skw' = {float}
|  |  |  |  |  |-- 'Kur' = {float}
|  |  |  |  |  |-- 'IQR' = {float}
|  |  |  |  |  |-- 'Med' = {float}
|  |  |  |  |  |-- 'MAD' = {float}
:  :  :  :  :  :
```
where:
- ```N``` is the number of files within data_files folder
- ```M``` is the number of hyper-heuristic iterations (metaheuristic candidates)
- ```C``` is the number of search operators in the metaheuristic (cardinality)
- ```P``` is the number of control parameters for each search operator
- ```R``` is the number of repetitions performed for each metaheuristic candidate
- ```D``` is the dimensionality of the problem tackled by the metaheuristic candidate
- ```I``` is the number of iterations performed by the metaheuristic candidate
- ```search_operator_structure``` corresponds to ```[operator_name = {str}, control_parameters = {dict: P}, selector = {str}]```
</p>
</details>

## 🏗️ Work-in-Progress

The following modules are available, but they may do not work. They are currently under developing.

### 🌡️ Characterisation

This module intends to provide metrics for characterising the benchmark functions.

Source: [``characterisation.py``](./characterisation.py)

### 📊 Visualisation

This module intends to provide several tools for plotting results from the experiments.

Source: [``visualisation.py``](./visualisation.py)

## Sponsors

<a href="https://tec.mx/en" target="_blank"><img src="./docfiles/logoTEC_full.png" width="250"></a>
<a href="http://www.cas.cn/" target="_blank"><img src="./docfiles/cas_logo.png" width="250"></a>
<a href="https://www.gob.mx/conacyt" target="_blank"><img src="./docfiles/conacyt-logo.png" width="250"></a>

## References

1. [Cruz-Duarte, J.M., Amaya, I., Ortiz-Bayliss, J.C., Connat-Pablos, S.E., and Terashima-Marín, H., A Primary Study on Hyper-Heuristics to Customise Metaheuristics for Continuous Optimisation. CEC'2020. Accepted.](./docfiles/SearchOperators_CEC.pdf)
1. Cruz-Duarte, J.M., Amaya, I., Ortiz-Bayliss, J.C., Connat-Pablos, S.E., Terashima-Marín, H., and Shi, Y., Hyper-Heuristics to Customise Metaheuristics for Continuous Optimisation. Submitted to SWEVO.
>>>>>>> tl-hh-umhs
>>>>>>> origin/main:README-customhys.md
