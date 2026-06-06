1. First create a folder
2. Open cmd, open vscode with `code .`
3. Create environment inside vscode terminal – `python3.11 -m venv proj_venv` – To contain all libraries inside a single folder
4. Activate above created virtual environment – `source proj_venv/bin/activate` – So that the packages are installed inside venv folder
5. Create python files as requried for project

### To install any python library use PIP, Eg – `pip install pandas`, numpy is installed automatically
### Install matplotlib with command – `pip install matplotlib`
### Instead of Jupyter we can create .ipynb file inside vscode
### Inside the .ipynb file Select Kernel and select the newly created venv

### To open vscode integrated terminal press `Command + J`

# Code:

Import matplotlib – `import matplotlib.pyplot as plt`
`pd.read_csv('file.csv')` function – read the csv file data and returns a pandas Dataframe object. If the csv file has a different seperator other that comma, then mention the seperator using the sep attribute – `pd.read_csv('file.csv', sep=";")`
`mydata.head()` or `mydata[:5]` – Returns first 5 records of Dataframe
`mydata.loc[0:8]` # To get a slice of dataset or a single record at the given index
`len(mydata)` – To get the total no. of records or total no. of elements in an object
`mydata.describe()` – To describe numerical columns of the dataset only
`mydata[mydata.Age.isnull()]` – Returns all the records with Age as null value. This works by passing in the True/False dataset of Age column
`mydata.dtypes` – Returns the datatype of each column
To convert datetime string to datetime data type – `vappadata.gmt = pd.to_datetime(vappadata.gmt)`
Merge function in pandas – `pd.merge(data1, data2, how=<join_type>, left_on=<left_table_column>, right_on=<right_table_column>)`
`countdf = joindf.groupby("Region").count()` – Group dataset based on Region and store in a variable `countdf`
Create plot(graph) using the function – `countdf.plot(kind="bar", figsize=(14, 5))`
To count the no. of values in a given column – `mydata.<column_name>.value_counts()`
`vappadata = vappadata.assign(weekday=weekdays)` – To add new column
`vappadata = vappadata.drop(columns=["weekdays"])` – To remove a column from a dataset

# MySQL

`a LEFT JOIN b USING (c1, c2, c3)` – Easier way to reference columns that have the same name in both tables.
`SHOW WARNING` – To display the warning message from the last run sql query
