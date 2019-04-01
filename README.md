# decision_tree_visualization
using graphviz to visualize decision tree in jupyter notebook

*source:  https://towardsdatascience.com/interactive-visualization-of-decision-trees-with-jupyter-widgets-ca15dd312084*

#### Requirements
* need to install sk-learn and graphviz
* to install packages from jupyter note book, you can use: 
```
!conda install --yes --prefix {sys.prefix} <package-name>
```
or alternatively:
```
%%bash
pip install <package-name>
```

#### I) Basic
* display tree only


#### II) Interactive
* display tree with interactive drop downs


#### Note:
For random forest model objects, you will need to select individual trees to display.
An estimator object will need to be chosen from the random forest model using *estimators_* and specifying the index.

```
model = RandomForestClassifier(<parameters>)
model.fit(X_train, y_train)
estimator = model.estimators_[0]
```
