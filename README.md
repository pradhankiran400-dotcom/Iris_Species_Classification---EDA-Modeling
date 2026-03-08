<h1>1. What patterns did you find?</h1><br>
•	Linear Separability: The Iris-setosa class is perfectly and easily separable from the other two species in almost every scatter plot, especially when comparing petal dimensions.<br>
•	Class Balance: The dataset is extremely well-balanced, with Iris-versicolor at 34%, Iris-virginica at 33.3%, and Iris-setosa at 32.7%.<br>
•	Feature Correlation: There is a strong positive linear correlation between petal length and petal width; as one increases, the other tends to increase as well.<br>
<h1>2. Which features seem most important?</h1><br>
•	Petal Measurements: Petal Length and Petal Width are the most important features. They show the clearest distinction between the three species with minimal overlap in data clusters.<br>
•	Distinct Averages: Bar charts confirm that Iris-virginica has the highest average petal length and width, while Iris-setosa has the lowest.<br>
<h1>3. Any surprising observations?</h1><br>
•	Outliers in Sepal Width: Unlike the other features, Sepal Width is the only column containing outliers.<br>
•	Specific Anomalies: There are three unusually high values () for Iris-setosa and one unusually low value  for Iris-versicolor.<br>
•	Inverse Relationship: While Iris-setosa has the smallest petals, it surprisingly has the widest sepals on average.<br>
<h1>4. What preprocessing would you do before modeling?</h1><br>
•	Outlier Handling: I would address the 4 outliers identified in the Sepal Width column (indices 15, 32, 33, and 60) either by removing them or capping them to prevent them from skewing the model.<br>
•	Feature Scaling: Since the features have different ranges (e.g., Petal Width goes up to while Sepal Length goes up to ), applying StandardScaler  would be beneficial for algorithms like k-NN or SVM or Decision Trees(‘Not Need StandScaler’).<br>
•	Label Encoding: The species column is categorical, so it needs to be converted into numerical format  using LabelEncoder before being fed into a machine learning model.
