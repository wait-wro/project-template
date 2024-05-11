# project-template

This repository serves as a template for data science projects within the WAIT community. It is structured to ensure consistency and efficiency in the development process. By using this template, members can adhere to best practices and streamline collaboration.

## Project structure

### Blah!

```
/data                # Directory for storing raw data and processed datasets.
/docs                # Documentation files for the project.
/models              # Serialized models, model predictions, and model summaries.
/notebooks           # Jupyter notebooks for explorations and presentations.
/reports             # Generated analysis as HTML, PDF, LaTeX, etc.
/src                 # Source code for use in this project.
.gitignore           # Specifies intentionally untracked files to ignore.
requirements.txt     # Project dependencies for reproducibility.
README.md            # The top-level README for developers using this project.
```

```
📦data                  <-- Directory for storing data
 ┣ 📂01_Raw             <-- The original, immutable data dump.
 ┣ 📂02_Interim         <-- Intermediate data that has been transformed.
 ┗ 📂03_Processed       <-- The final data sets for modeling.
📦figures               <-- Generated graphics and figures to be used in reporting. 
                            Naming convention is a number (for ordering)
📦models
📦notebooks             <-- Jupyter notebooks. Naming convention is a number (for ordering) e.g. `01_RawDataPreprocessing.ipynb`
📜.gitignore            <-- Specifies intentionally untracked files to ignore.
📜 Reamde.md            <-- The top-level README for developers using this project.


```