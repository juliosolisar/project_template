# Project Template

![project_template-1](https://github.com/user-attachments/assets/3d568646-a9fa-449a-a0a5-731e2cdb033c)

Standard architecture for code and project management (based on David Yang's lab manual)

Two folders
- `build`
  - `temp`: Folder contains .Rmds for data cleaning and wrangling from raw datasets. .Rmds are `child` doing subtasks put together by code on `output`
    -  Raw datasets are taken from `~Dropbox/.../06_data/input/`
    -  Code stores processed data in `~Dropbox/.../06_data/temp/`
  - `output`: calls `child` .Rmds and puts together the final dataset for analysis
    - Whenever code is not `child` it is included here
    - Code stores final data prior to analyis in `~Dropbox/.../06_data/output/`

- `analysis`
  - Code analysing clean data from stored in `~Dropbox/.../06_data/output/`
  - Can generate output which is also saved on `~Dropbox/.../06_data/output/`
  
To make code reproducible:

1. Create an Rproject at the top of the repo folder (i.e., at the same level of this README file)

2. Modify the .Renviron file to point into the Dropbox or other folder containing the data
