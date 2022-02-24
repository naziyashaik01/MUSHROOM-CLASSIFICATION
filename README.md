# MUSHROOM-CLASSIFICATION
GOAL:In this project, we will examine the data and bUild different machine learning models that will detect if the mushroom is edible or poisonous by its specifications.
In this project, i used the python libraries namely NUMPY,PANDAS,MATPLOTLIB,SCIKIT LEARN.

Attribute Information or Dataset Details:

classes: edible=e, poisonous=p
cap-shape: bell=b,conical=c,convex=x,flat=f, knobbed=k,sunken=s
cap-surface: fibrous=f,grooves=g,scaly=y,smooth=s
cap-color: brown=n, buff=b, cinnamon=c, gray=g,green=r, pink=p, purple=u, red=e,white=w,yellow=y
bruises: bruises=t,no=f
odor: almond=a, anise=l, creosote=c, fishy=y, foul=f, musty=m, none=n, pungent=p,spicy=s
gill-attachment: attached=a,descending=d,free=f,notched=n
gill-spacing: close=c,crowded=w,distant=d
gill-size: broad=b,narrow=n
gill-color: black=k,brown=n,buff=b,chocolate=h,gray=g, green=r, orange=o, pink=p,purple=u,red=e,white=w,yellow=y
stalk-shape: enlarging=e,tapering=t
stalk-root: bulbous=b, club=c, cup=u, equal=e, rhizomorphs=z, rooted=r,missing=?
stalk-surface-above-ring: fibrous=f,scaly=y,silky=k,smooth=s
stalk-surface-below-ring: fibrous=f,scaly=y,silky=k,smooth=s
stalk-color-above-ring: brown=n, buff=b, cinnamon=c, gray=g, orange=o, pink=p, red=e,white=w,yellow=y
stalk-color-below-ring: brown=n, buff=b, cinnamon=c, gray=g, orange=o, pink=p, red=e,white=w,yellow=y
veil-type: partial=p,universal=u
veil-color: brown=n,orange=o,white=w,yellow=y
ring-number: none=n,one=o,two=t
ring-type: cobwebby=c, evanescent=e, flaring=f, large=l, none=n, pendant=p, sheathing=s,zone=z
spore-print-color: black=k, brown=n, buff=b, chocolate=h, green=r, orange=o, purple=u,white=w,yellow=y
population: abundant=a, clustered=c, numerous=n, scattered=s, several=v, solitary=y
habitat: grasses=g, leaves=l, meadows=m, paths=p, urban=u, waste=w, woods=d

If you want to check the original dataset than please click on the below link, its a Kaggle dataset

https://www.kaggle.com/uciml/mushroom-classification

First we need to import the necessary libraries
pandas : Use to handle Tabular data
numpy : Support for large, multi-dimensional arrays and matrices, help to perform mathematical functions on those arrays.
sklearn : It is a Machine Learning Library which allows to implement different Machine Learning models.

So, we upload our csv dataset using pandas function pd.read_csv().
The Dataset has 22 features and 1 target variable(i.e. class).
Our dataset is a categorical dataset with 2 class target column
p :- Poisonous Mushroom
e :- Edible Mushroom

There are total 8,124 rows without any null values present in our dataset and every feature including the target variable is of type object. Also look at the last line. info() function also shows how much memory is used by the dataset.

There is no data imbalance issue in dataset.

PREPROCESSING:

LABEL ENCODING:
Machine Learning model only accepts the numerical data and we have non-numerical values in data, so we will use Label Encoding, a preprocessing library of sklearn to convert non numeric data into numeric. This will give a random ranking to the values inside the column.
