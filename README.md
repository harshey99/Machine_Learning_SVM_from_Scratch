# Machine_Learning_SVM_from_Scratch


Student Name: Harshitha Bengaluru Raghuram
Student Id: 21235396
Course: MAI




Algorithm:
Classification Algorithms are used for mapping any point present in the dataset to any one of the classes. We have selected Linear Support Vector Machine Algorithm. The SVM algorithm can be applied on both Regression and Classification problems.
 SVM can be defined as a generalized form of Maximal Margin Classifier. Linear SVM is also called as “Hard Margin Classifier”. In “Hard Margin SVM Classifier” the dataset is perfectly classified in to 2 different classes using the hyperplane. In contrast, the “Soft Margin SVM Classifier” cannot perfectly divide the dataset into the classes. Thus, the datapoints that are misclassified by the hyperplane are called as Outliers. The Soft Margin SVM Classifier model ignores the outliers while performing the classification. 
Hyperplane:
In a 2 dimensional space, 1 dimensional hyperplane is used to classify the data. In a 3 dimensional space, 2 dimensional hyperplane is used to classify the data. To generalize, n dimensional space requires, n-1 dimensional hyperplane to classify the dataset. For solving classification problems, the SVM creates a hyperplane which can be used to divide the data in to categories or classes. 
Affine Subspace:
A Vector Space can be defined as a linear combination of vectors from V1, V2……Vk to Rn is a summation of the form β1V1+ β1V2+…… βkVk where β1, β2…..βk  ∈ R. 
The Affine Combination of Vectors can be defined as as a linear combination of vectors from V1, V2……Vk to Rn is a summation of the form β1V1+ β1V2+…… βkVk  such that 
∑k i=1 βi = 1.  The only difference between the vector space and affine subspace is the sum of all the weight vectors is equal to 1 in affine subspace. A vector space in 2 dimension is a plane whereas an affine space in 2 dimension is a line. 
If a line passes through the origin then it is both a vector subspace and affine subspace. However, if a line does not pass through the origin it is only an affine subspace.
Hyperplane Equation:
In a 2 dimensional space, the equation of a hyperplane is derived by adding bias to the equation of affine combination. The bias is denoted by using ‘b’. The bias can be called the “offset value of the hyperplane”.
h(x) = β1X1+β2X2+…………+b
From the above equation, for a given point x, 
If the value of h(x) = 0 then the point lies on the hyperplane.
If the value of h(x) is greater than zero or if h(x)  is less than zero  then the point lies on either side of the hyperplane.
Margin:
The points that lie nearest to the hyperplane are selected from both the classes. The selected points are termed as “Support Vectors”. The distance from the Support Vectors to the hyperplane is computed. The perpendicular distance between the Support Vectors and the Hyperplane is called “Margin”. When  the distance between then  Support vector and the Hyperplane is maximum, it is called Optimal Hyperplane. Since we select an Optimal Hyperplane, the decision boundary between the classes is widest. Size of the margin also increases the Confidence of the Classifier.
There are 2 types of margin namely Functional Margin and Geometric Margin. The functional margin relies on bias b and weight vectors β. Scaling of β and b would not modify hyperplane equation but will widen the margin. To avoid this Geometric Margin is used. The geometric margin uses the normalizer to prevent the widening of the margin.
Maximal Margin Classifier:
The sign of  h(xi) value is used to determine the label of the output is either 1 or -1. The distance between the point xi and the hyperplane is denoted by the magnitude.
 
Soft Margin Classifier:
In the real world, the data is not linearly separable as assumed in Hard Margin Classifier. Thus, the Hard Margin Classifier cannot be implemented in Inequality Constraint.
Slack Variable:
The slack variable can measure the amount of violation by a point from the margin. The slack variable uses misclassification penalty to differentiate between the datapoints. 
The data point is away from the margin or on the margin when misclassification penalty is zero. Secondly, when the misclassification penalty is greater than 1 the datapoint is misplaced.
If the misclassification penalty lies between 0 and 1 then the datapoint is in the correct position.
Regularisation:
In order to balance the cost of misclassification, the constants C and k are introduced.  C is the “Regularization Constant”.  Regularisation determines to what extent the misclassification of training example can be avoided. StandardScaler() is used to normalize the data.
If the value of C is large then the hyperplane with smaller margin is selected else when the value of C is small then the hyperplane with larger margin with the capacity to misclassify larger number of points is selected.
k can be assigned either 1 or 2. The value of k indicates the type of loss. k = 1 indicates “Hinge Loss” whereas  k = 2 signals “Quadratic Loss”.
Hinge Loss:
In SVM algorithm the Hinge loss can be defined as the line which distinguishes the “positive and negative instances”by assigning numeric values. If hinge loss = 1 then the point lies on he left side otherwise if the  hinge loss = -1 then the point lies on the right side of the boundary. 
Gradient Descent:
When Hinge Loss is encountered, Gradient Descent is applied. The Gradient Descent is used to perform optimization for the objective function. The only drawback of Gradient Descent is it cannot be applied on Non Linear Boundaries. Gradient Descent performs optimization by converting inequality to equality constraint.
Objective function:
The aim of the Objective function is to minimize the slack variable. The misclassification cost can be balanced by using constants like C and k.
The loss becomes zero, while the margin is being maximized, then c becomes zero.
If the objective function will try to minimize the loss then c tends to infinity.


References:
https://towardsdatascience.com/a-definitive-explanation-to-hinge-loss-for-support-vector-machines-ab6d8d3178f1
http://www.adeveloperdiary.com/data-science/machine-learning/support-vector-machines-for-beginners-linear-svm/
https://towardsdatascience.com/https-medium-com-pupalerushikesh-svm-f4b42800e989
https://medium.com/machine-learning-101/chapter-2-svm-support-vector-machine-theory-f0812effc72
https://towardsdatascience.com/a-definitive-explanation-to-hinge-loss-for-support-vector-machines-ab6d8d3178f1



