# newproject

The file structure is organized as such:

``` text
newproject
  ├── data
  |     ├── out
  |     ├── raw
  |     ├── README.md
  ├── report
  |     ├── README.md
  ├── results
  |     ├── figures
  |     ├── tables
  ├── scripts
  |     ├── processing
  |     ├── analysis
  |     ├── utils
  |     ├── README.md
  ├── submission
  |     ├── README.md
  ├── .gitignore
  ├── LICENSE
  ├── README.md
  ├── lab-book.md
  ├── newproject.Rproj
```

## Directory organisation

-   `data`:
    -   `data/raw`: All original files needed for the analysis that were not produced in the project in hand. These files should be protected against any change after the first storage. These files should be added to `.gitignore` as to not be tracked by git.
    -   `data/out`: All data generated for the project. These files should be added to `.gitignore` as to not be tracked by git.
-   `report`: Any presentation or notes related to the project's discussion should be stored in this folder.
-   `results`: All code used to process the data.
    -   `results/figures`: Output figures. These files should be added to `.gitignore` as to not be tracked by git.
    -   `results/tables`: Output tables. These files should be added to `.gitignore` as to not be tracked by git.
-   `scripts`:
    -   `scripts/processing`: Data wrangling of data originally from `data/raw`. Processing of data to create data objects.
    -   `scripts/analysis`: Where the majority of the analysis will be stored. Preferably, scripts should not be extensively large. Name of documents should be clear.
    -   `scripts/utils`: All the R scripts and personal functions that are used in more than one file. Access them through the `source()` function.
-   `submission`: Files specific to journal submissions, such as cover letters or distinct submitted versions.

This is a personalised structure based on a reproducible workflow as described by 
https://github.com/FellowsFreiesWissen/computational_notebooks.git (thank you guys!)
