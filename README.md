# SupervisedProject

This is a dataset of bank transactions which have been classified as fraudulent or not.
Can you create a machine learning model to accurately predict whether a transaction is fraudulent or not?

I couldn't upload the file due to the large amount of data. I am attaching the link for it, here:
https://www.kaggle.com/ealaxi/paysim1

**Dataset**

Here are the first 5 rows of the dataset.

![alt text](https://github.com/Este-code/SupervisedProject/blob/main/images1/head.jpg)

**No missing values**

![alt text](https://github.com/Este-code/SupervisedProject/blob/main/images1/missing_value.png)

**Plot**
I displayed the type of transactions on a graph, divided by the transactions which are fraduolent and the ones that are not.
It's not so visible, due to the amount of data
However, CASH_OUT and TRANSFER transactions are the ones where fraud is involved.

![alt text](https://github.com/Este-code/SupervisedProject/blob/main/images1/count.jpg)

**Model**

Focusing on the observations that have been recorded as fraudolent, one can see that the amount of the transaction 
does not equal the difference between the new balance destination and the old balance destination.
I will prepare the dataset for the supervised model. 
"isFraud" column is going to be the target of the model.
I will select the features I will use to train and test the model: type (on which will require a label encoder), amount, oldbalanceDest, newbalanceDest.

![alt text](https://github.com/Este-code/SupervisedProject/blob/main/images1/encoder.png)

I have chosen the **Logistic Regression** beacuse this model has a binary output, therefore I'm classifing a transaction as fraudolent or not.

![alt text](https://github.com/Este-code/SupervisedProject/blob/main/images1/Model.png)

Accuracy: **99%**
