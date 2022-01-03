# AmExpert_Hackathon_2021

### **Problem Statement**
A mid-sized private bank that includes a variety of banking products, such as savings accounts, current accounts, investment products, credit products, and home loans.
The task is to predict the next set of products (upto 3 products) for a set of customers (test data) based on their demographics and current product holdings.

### **Approach**
* It is Multi label Classification problem, where in we have to predicts the top 3 production only out of 22 types of different products for the Y Variable
* Products (both B1 and B2) are converted to multi-hot encodings. There are 22 types of products.
* Age and Vintage Variable were scaled down by Standardization
* Binary label was for Gender and City_Category, Variables
* One hot encoding was used for Customer_Category

### **Project Flow**
* Feature Engineering and EDA
* Split to train and test
* Standardization
* Model Building
* Model Evaluation
* Prediction on Given Test Set

### **Modeling**
* Neural Network is used with with 3 hidden layers of 32,26,8
* Leaky Relu Activation function is used for the input and the hidden layers to avoid dead relu
* Sigmoid Activation function is used for the output layer
* Adam optimizer is used for faster learning
* Used BinaryCrossEntropy loss since it is a Multi Label problem
* Avg_Precision_Score is used as a evaluation matrix
