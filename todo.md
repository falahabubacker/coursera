1. First create a folder
2. Open cmd, open vscode with `code .`
3. Create environment inside vscode terminal – `python3.11 -m venv proj_venv` – To contain all libraries inside a single folder
4. Activate above created virtual environment – `source proj_venv/bin/activate` – So that the packages are installed inside venv folder
5. Create python files as requried for project

### To install any python library use PIP, Eg – `pip install pandas`, numpy is installed automatically
### Instead of Jupyter we can create .ipynb file inside vscode

### To open vscode integrated terminal press `Command + J`

# Code:

`pd.read_csv('file.csv')` function – read the csv file data and returns a pandas Dataframe object
`mydata.head()` or `mydata[:5]` – Returns first 5 records of Dataframe
`mydata.loc[0:8]` # To get a slice of dataset or a single record at the given index
`len(mydata)` – To get the total no. of records or total no. of elements in an object
`mydata.describe()` – To describe numerical columns of the dataset only
`mydata[mydata.Age.isnull()]` – Returns all the records with Age as null value. This works by passing in the True/False dataset of Age column
`mydata.dtypes` – Returns the datatype of each column