## Split Large Data Files
This is a simple script I wrote out of necessity. Often times I'm asked to take a large files and split these files into smaller chunks so that teams can begin working with them.

The use case here is that some files are very large with 1M+ rows. I've worked on files with 4M, 6M, and even up to 10M records, and not every person has access to tools like PowerBI or Tableau to be able to access such large files.

This simple script takes a filename and maxRowLength and spits out xlsx files.

### Example
Steam Reviews dataset on Kaggle has over 6 million rows. 
https://www.kaggle.com/andrewmvd/steam-reviews

The expected result with *maxRowLength = 500000* will be x files.

![Alt text](/../main/output.png?raw=true "Optional Title")
