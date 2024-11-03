# Fluorescent Dye Database and Prediction Tool —— Flour-predictor
## The main framework of this work.
![image](https://github.com/17855461143/flour_pred/blob/main/figures/2.png?raw=true)

## File Description
* Data aggregation  
  The directory contains our compiled dye data as well as the collected xanthene  and cyanine datasets.
* MTATFP  
  The main code for this project, including training data and code for three types of predictive models.
* GUI  
  The user interaction code for Flour-predictor. Once the environment is set up, simply run GUI.py to execute it, and the output data will be saved in the Results folder.
* Single-task_and_ML_models  
  Single-task models and machine learning code for comparison with the MTATFP model.


## Creation of the GUI Usage Environment:
* conda create -n dye37 python=3.7
* conda install pytorch==1.13.1 torchvision==0.14.1 torchaudio==0.13.1 pytorch-cuda=11.7 -c pytorch -c nvidia
* conda install xlsxwriter
* conda install -c anaconda scikit-learn
* pip install pandas==1.3.0
* pip install dgllife==0.2.8
* pip install rdkit-pypi
* pip install dgl==1.1.2+cu117 -f https://data.dgl.ai/wheels/cu117/repo.html
* pip install packaging  
___In GUI.py, jump to the code in attentivefp.py through AttentiveFPGNN, rename copy_edge to copy_e; rename src_mul_edge to u_mul_e. After the installation is complete, you can run it directly___
![image](https://github.com/17855461143/test/blob/main/1.png?raw=true)

## Data Usage Distribution
![image]([https://github.com/17855461143/test/blob/main/Figure1.png?raw=true](https://github.com/17855461143/flour_pred/blob/main/figures/3.png?raw=true))

## Atom Weight Visualization
In the MTATFP folder, we have retained visualization code for all scripts, allowing users to display visualized weights and also to regenerate training files for new data visualization.
![image]([https://github.com/17855461143/test/blob/main/Figure1.png?raw=true](https://github.com/17855461143/flour_pred/blob/main/figures/4.png?raw=true))
