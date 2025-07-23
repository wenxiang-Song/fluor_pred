# Fluorescent Dye Retrieval and Prediction Tool —— Fluor-predictor
## The main framework of this work.
![image](https://github.com/wenxiang-Song/fluor_pred/blob/main/figures/2.png?raw=true)

## File Description:
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
## We provide an updated web prediction tool for free use: 
https://lmmd.ecust.edu.cn/Fluor-tools/

Please follow these steps to create the working environment.  
* conda install pytorch torchvision torchaudio pytorch-cuda
* conda install xlsxwriter
* conda install scikit-learn
* pip install pandas
* pip install dgllife
* pip install rdkit-pypi
* pip install dgl
* pip install packaging
  
  
## The software interface is shown as follows:
for specific usage, please refer to the User Guide.pdf.
![image](https://github.com/wenxiang-Song/fluor_pred/blob/main/figures/1.png?raw=true)

## Data Usage Distribution:
![image](https://github.com/wenxiang-Song/fluor_pred/blob/main/figures/3.png?raw=true)

## Atom Weight Visualization:
In the MTATFP folder, we have retained visualization code for all scripts, allowing users to display visualized weights and also to regenerate training files for new data visualization.
![image](https://github.com/wenxiang-Song/fluor_pred/blob/main/figures/4.png?raw=true)

## Usage Statement:
Fluor-predictor is a freely available dye database and dye prediction tool. You have the right to install and run the software on your personal computer, as well as to copy and modify the software to meet your personal learning and research needs. However, you are not allowed to use the software for any commercial activities, including but not limited to selling, renting, lending the software or any derivative products of the software, or using the software in any commercial services or products.
