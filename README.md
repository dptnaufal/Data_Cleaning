# Data_Cleaning
Definition of Data Processing

### Unclean data is the result of the following factors

There is an additional input available

Inconsistent data input from users

There was a problem/bug in the app

Abusers and fraudsters exist.

### Data cleaning processes that are commonly used

Handling missing value

Data standardization

Data transformation

Categorical data encoding

Outlier handling

### How to handling missing value, maye you can use syntax:

- data.info () 

- data.isnull().sum()

- data['aa'].value_counts()

### Label Encoding

- Label Encoding is the process of converting a categorical feature to a numerical feature by assigning different numbers to each unique value.

`code` le = preprocessing.LabelEncoder()

le.fit(data['aa'])

data['aa_label_encoding'] = le.transform(data['aa']) 

Embarked_Label_Encoding = data[['aa','embark_town_label_encoding',]]

Embarked_Label_Encoding.head()

### Ordinal Encoding

`code` data = sns.load_dataset('xx')

data.head()

- map_class = {'First':3,
             'Second':2,
             'Third':1}
             
  data['class_cat'] = data['class'].map(map_class)
  
  data[['class','class_cat']].head()
  
  # Requirment
  
  numpy and pandas
