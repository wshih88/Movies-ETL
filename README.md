# Movies-ETL Assumptions
##1. Exactly three files are uploaded.
##2. Files must be in .json, .csv, and .csv order.
##3. Database column names must be identified.
##4. All finance data to remain under billions of dollars.
##5. Datetime format is in text and not serial date number.
### The code accepts exactly three files in assumption that they are from the same data source, and the same format. Current code only allows to process one .json and two .csv files. The column names must remain static to allow formatting changes to ensure proper merging of the dataframes. While the regex code allows for some spelling errors and variations to define box office earnings and film budget, should either categories go to and beyond $1 trillion, the function would fail, therefore dollar figures must be below $1 trillion.  While serial date numbers are manageble, the current code assumes that serial date numbers are not used.