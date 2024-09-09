# newproject

The file structure is organized as such:

``` text
newproject
  ├── data
  |     ├── raw
  |     ├── out
  |     ├── metadata
  |     └── README.md
  ├── scripts
  |     ├── processing
  |     ├── analysis
  |     ├── utils
  |     └── README.md
  ├── results
  |     ├── figures
  |     ├── tables
  |     └── README.md
  ├── report
  |     ├── README.md
  |     ├── main.docx
  |     ├── figures
  |     ├── tables
  |     └── supplementary
  ├── submission
  |     ├── journal1
  |     └── README.md
  ├── .gitignore
  ├── LICENSE
  ├── README.md
  ├── lab-book.md
  └── newproject.Rproj
```

## Directory organisation

- `data`:
    - `data/raw`: All original files needed for the analysis that were not produced in the project in hand. These files should be protected against any change after the first storage. These files should be added to `.gitignore` as to not be tracked by git.
    - `data/out`: All data generated for the project. These files should be added to `.gitignore` as to not be tracked by git.
    - `data/metadata`: Metadata for the raw data and possible dependencies.
- `scripts`: This folder contains all code used to process the data and perform the analysis.
    - `scripts/processing`: Data wrangling of data originally from `data/raw`. Processing of data to create data objects.
    - `scripts/analysis`: Where the majority of the analysis will be stored. Preferably, scripts should not be extensively large. Name of documents should be clear.
    - `scripts/utils`: All the R scripts and peran one file.sonal functions that are used in more th Access them through the `source()` function.
- `results`: All code used to process the data.
    - `results/figures`: Output figures. These files should be added to `.gitignore` as to not be tracked by git.
    - `results/tables`: Output tables. These files should be added to `.gitignore` as to not be tracked by git.
- `report`: Any presentation or notes related to the project's discussion should be stored in this folder.
    - `report/main.docx`: Word document where the initial draft should be prepared.
    - `report/figures`: Finalised figures to be included in the `main.docx` document.
    - `report/tables`: Finalised tables to be included in the `main.docx` document.
    - `report/supplementary`: Supplementary material referenced in the text, be it figures or tables.
- `submission`: Files specific to journal submissions, such as cover letters or distinct submitted versions.
    - `journal1`: Example of folder relative to first submission. Other sub-folders ma y created here, such as `first` or `revisions`, depending on the submission path.

This is a personalised structure based on a reproducible workflow as described by (FellowsFreiesWissen/computational_notebooks)[https://github.com/FellowsFreiesWissen/computational_notebooks.git] (thank you guys!)
