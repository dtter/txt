_Table of Contents_
1. [[#Setup coding environment]]
2. [[#Load the data]]
3. [[#Examine the data]]
4. [[#Plot the data]]

ref: (https://www.kaggle.com/alexisbcook/hello-seaborn/tutorial

---
### Setup coding environment
in any notebook (i.e. Jupyter Notebook, Colab)
```Python
import pandas as pd
pd.plotting.register_matplotlib_converters()
import matplotlib.pyplot as plt
%matplotlib inline
import seaborn as sns
print("Setup Complete")
```

### Load the data
Specify the filepath to laod the data (in CSV or _comma-separated values file_)
```Python
# Path of the file to read
fifa_filepath = "../input/fifa.csv"

# Read the file into a variable fifa_data
fifa_data = pd.read_csv(fifa_filepath, index_col="Date", parse_dates=True)
```
- `index_col="Date"` : set the value to the name of the first column `Date` (A1 in Excel); we want each entry in the first column to denote a different row 
- `parse_dates=True` : each row labels as a date

### Examine the data
```Python
# Print the first 5 rows of the data
fifa_data.head()
```
see the [output here](https://www.kaggle.com/alexisbcook/hello-seaborn/tutorial)

### Plot the data
```Python
# Set the width and height of the figure
plt.figure(figsize=(16,6))

# Line chart showing how FIFA rankings evolved over time 
sns.lineplot(data=fifa_data)
```