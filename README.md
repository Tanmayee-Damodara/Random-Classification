# <p align = "center" >RANDOM CLASSIFICATION</p>
## Aim:
To write a python program to perform random classification.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Google Colab / Jupiter Notebook

## Related Theoretical Concept:
<b>Random classifier:</b><div align = "justify">It creates a set of decision trees from randomly selected subset of training set. It then aggregates the votes from different decision trees to decide the final class of the test object. Random Forest is suitable for situations when we have a large dataset, and interpretability is not a major concern.</div><br>
<b>Purpose of Random classifier:</b>
<div align = "justify">One of the most important features of the Random Forest Algorithm is that it can handle the data set containing continuous variables as in the case of regression and categorical variables as in the case of classification.</div>

## Algorithm
1. In Random Forest, n number of random records are taken from the data set having k number of records.<br>
2. Individual decision trees are constructed for each sample.<br>
3. Each decision tree will generate an output.<br>
4. Final output is considered based on Majority Voting or Averaging for Classification and regression respectively.

## Program:
```
/*
Program to implement random classification.
Developed by    : M.D.Tanmayee
Register Number : 212219040163
*/

import matplotlib.pyplot as plt
from sklearn import datasets
x,y = datasets.make_blobs(n_samples=100,n_features=2,centers=2,cluster_std=1.05,random_state=2)
fig=plt.figure(figsize=(10,8))
plt.plot(x[:,0][y==0], x[:,1][y==0],'r^')
plt.plot(x[:,0][y==1], x[:,1][y==1],'bo')
plt.xlabel("Feature 1")
plt.ylabel("Feaure 2")
plt.title("Random Classification Data with 2 classes")
```

## Output:
![image](https://user-images.githubusercontent.com/89249977/169957610-57282d21-80b1-4380-a68c-37c14aad8d6e.png)

## Result:
Thus the random classifier was successfully implemented using python programming.
