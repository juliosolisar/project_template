# Project Template
Standard architecture for code and project management (based on David Yang's lab manual)

Two folders
- Build
  - `temp`: `child` .Rmds for data cleaning and wrangling from raw datasets (taken from `~Dropbox/.../06_data/input/`); stores processed data in `~Dropbox/.../06_data/temp/`
  - `output`: calls `child` .Rmds and puts together the final dataset for analysis (stored in `~Dropbox/.../06_data/output/`)

- Analysis
  - Code analysing clean data from stored in `~Dropbox/.../06_data/output/`
  - Can generate output which is also saved on `~Dropbox/.../06_data/output/`
