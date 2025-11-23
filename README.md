# Weight-Adjusting Binary Transformation (WABT)

We provide our WABT model, and necessary utilities in this repository. Containerization will be available in the future. 

Our experiments, shown in our accompanying paper, were conducted on a computer with the processor AMD Ryzen 7 4800H, 2.90 GHz, with 16.0 GB RAM, Windows 11 operating system. 

### Contents

 - wabt.py: Our entire model
 - main.ipynb: Contains a method for running a model on a dataset, which the user can modify accordingly. Also contains some example runs of WABT, and conducting the nemenyi test.
 - nemenyi.py: Method used for nemenyi analysis. It also contains a copy of the graph related methods from the [Orange](https://pypi.org/project/Orange3/) library, since those methods are now deprecated.
 - utils.py: Methods for loading libraries and evaluation metrics. For fairness in comparisons, the accuracy metric implementations are the same as in the [PBT codebase](https://github.com/o-yildirim/PBT/tree/main).
 - results folder: Contains our results as .csv files, also some additional test run results in .txt files, plots, critical distance graphs. Plots and test results generated from the model WABT are automatically added here, so make sure that results folder is inside the root directory while running, if you want to save results.
 - datasets folder: Contains the datasets used in the experiments.

### Version info
requirements.txt contains all the libraries we installed at one point in the project. These specific ones are the most important, as **different versions can create different test results**:

 - river==0.19.0
 - scikit-learn==1.3.2 
 - scikit-multilearn==0.2.0
 - scipy==1.10.1

