# project-template

This repository serves as a template for data science projects within the WAIT community. It is structured to ensure consistency and efficiency in the development process. By using this template, members can adhere to best practices and streamline collaboration.

## Recommended Project's structure

```
📦data                  <-- Directory for storing data
 ┣ 📂01_Raw             <-- The original, immutable data dump.
 ┣ 📂02_Interim         <-- Intermediate data that has been transformed.
 ┗ 📂03_Processed       <-- The final data sets for modeling.
📦docs                  <-- Documentation files (eg. markdown files linked with README.md)
📦figures               <-- Generated graphics and figures to be used in reporting.
📦models                <-- Trained and serialized models.
📦notebooks             <-- Jupyter notebooks named in the following convention e.g. `01_RawDataLoad.ipynb`
📜.gitignore            <-- Specifies intentionally untracked files to ignore.
📜 Reamde.md            <-- The top-level README for developers using this project.

```

## Recommended files naming convention

- To properly navigate through the project pipeline, notebooks should be executed in the order specified by their names, ensuring each step builds on the previous one.
- Generated files are stored in `data`, `figures`, and `models` folders, with names prefixed by numbers that correspond to the generating notebook for easy traceability.

```
📦data
 ┣ 📂01_Raw
 ┃ ┗ 📜01_DataCompetencySurvey.csv    # The number in the prefix of the filename indicates the notebook
 ┣ 📂02_Interim                       # where file has been generated.
 ┃ ┗ 📜01_SelectedFeutures.csv          
 ┗ 📂03_Processed
 ┃ ┗ 📜02_ProcessedData.csv     <---- # File generated in the 02_FeatureEngineering.ipynb         
📦docs                   
📦figures
 ┗ 📜03_TargetDistribution.png  <---- # File generated in the 03_ExploratoryDataAnalysis.ipynb
📦models                
📦notebooks
 ┣ 📜.gitkeep
 ┣ 📜01_DataPreprocessing.ipynb       # The numbering of files suggests the order of execution,
 ┣ 📜02_FeatureEngineering.ipynb      # while descriptive naming provides clear insights       
 ┣ 📜03_ExploratoryDataAnalysis.ipynb # into the content and purpose of each file
 ┣ 📜04_Modeling.ipynb                # facilitating an organized and logical workflow.
 ┗ 📜05_ModelsEvaluation.ipynb
📜.gitignore            
📜 README.md            
```
