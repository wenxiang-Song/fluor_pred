# Fluorescent Dye Retrieval and Prediction Tool —— Fluor-predictor
## The main framework of this work.
![image](https://github.com/17855461143/fluor_pred/blob/main/figures/2.png?raw=true)

## File Description
* Data aggregation [folder]  
  The directory contains our compiled dye data as well as the collected xanthene  and cyanine datasets.  
    
* MTATFP [folder]  
  The main code for this project, including training data and code for three types of predictive models.  
    
* GUI [folder]  
  The user interaction code for Fluor-predictor. Once the environment is set up, simply run GUI.py to execute it, and the output data will be saved in the Results folder.  
    
* Single-task_and_ML_models [folder]  
  Single-task models and machine learning code for comparison with the MTATFP model.  
    
* User Guide.pdf  
  The specific usage method of Fluor-predictor is based on the runtime environment.
  
* demo_video.mp4  
  The usage demonstration of Fluor-predictor: users simply need to replace the target molecules and solvents.

## Creation of the GUI Usage Environment:  
Please follow these steps to create the working environment.  
* conda create -n dye37 python=3.7
* conda install pytorch==1.13.1 torchvision==0.14.1 torchaudio==0.13.1 pytorch-cuda=11.7 -c pytorch -c nvidia
* conda install xlsxwriter
* conda install -c anaconda scikit-learn
* pip install pandas==1.3.0
* pip install dgllife==0.2.8
* pip install rdkit-pypi
* pip install dgl==1.1.2+cu117 -f https://data.dgl.ai/wheels/cu117/repo.html
* pip install packaging
  
There is an error in the AttentiveFP library that needs to be corrected. Here are the steps for the modification: ___In GUI.py, jump to the code in attentivefp.py through AttentiveFPGNN, rename copy_edge to copy_e; rename src_mul_edge to u_mul_e. After the installation is complete, you can run it directly___  
  
## The software interface is shown as follows
for specific usage, please refer to the User Guide.pdf.
![image](https://github.com/17855461143/fluor_pred/blob/main/figures/1.png?raw=true)

## Data Usage Distribution
![image](https://github.com/17855461143/fluor_pred/blob/main/figures/3.png?raw=true)

## Atom Weight Visualization
In the MTATFP folder, we have retained visualization code for all scripts, allowing users to display visualized weights and also to regenerate training files for new data visualization.
![image](https://github.com/17855461143/fluor_pred/blob/main/figures/4.png?raw=true)

## Usage Statement
Fluor-predictor is a freely available dye database and dye prediction tool. You have the right to install and run the software on your personal computer, as well as to copy and modify the software to meet your personal learning and research needs. However, you are not allowed to use the software for any commercial activities, including but not limited to selling, renting, lending the software or any derivative products of the software, or using the software in any commercial services or products.
