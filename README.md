from google.colab import files
uploaded = files.upload()

import pandas
data=pandas.read_csv('chart.csv')
countries_unique=data['City'].unique()
unique_count = data['City'].nunique()
print(unique_count)
