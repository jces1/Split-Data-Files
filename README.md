# Split Large Data Files

##General Info
This is a simple script I wrote out of necessity. Often times I'm asked to take a large files and split these files into smaller chunks so that teams can begin working with them.

The use case here is that some files are very large more than 1M rows which Excel has difficulty handling such files, and not every person has access to tools like PowerBI or Tableau to be able to access such large files.

This simple script takes a filename and creates multiple Excel files based on the desired maximum record count per file.

## Technologies
- Python 3.9
  - Pandas, os

## Example
Steam Reviews dataset on Kaggle has 6,417,106 rows. 

https://www.kaggle.com/andrewmvd/steam-reviews

The expected result with *maxRowLength = 500000* will be 12 files with 500,000 records, and the 13th file with the remaining 417,106 records.

![Alt text](/../main/output_example.png?raw=true "Output")
