# billboard tidy-data excercise

## requirements
  - all the necessary files are included in requirements.txt

## modifications
  - names of the artist was uninverted if "," occured
  - multiple weeks were melted into columns "week" and "rank"
  - rows containing NaN were deleted
  - previous week strings were converted into numbers
  - column "rank" data type was set to int64
  - long names were shorten to 20 chars by adding "..."
  - date column was created from "date.entered" and "week"
  - columns "date.entered" and "date.peaked" were deleted from main file and saved into billboard_dates.csv
  - all the values were sorted by year > artist > track > week > rank
  - final data was saved to billboard_clean.csv



## structure
  - files structure

### original_data/
  - billboard.csv (necessary)
#### metadata/
  - metadata_guide.md
### documents/
  - data_appendix.md
  - README.md
### command_files/
  - lab2.ipynb (necessary)
### analysis_data/
  - billboard_clean.csv
  - billboard_dates.csv