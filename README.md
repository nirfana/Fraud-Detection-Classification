# Fraud-Detection-Classification
### **Objective**<br>
The goal of this project is to construct a machine learning model that predicts fraudulent activities. We'll explore five different classification models: K-Nearest Neighbor (KNN), Support Vector Machine (SVM), Decision Tree, Random Forest, and the boosting algorithm XGBClassifier. Each model will be carefully evaluated using cross-validation and performance metrics such as Recall and F1 score. After identifying the best base model, we'll fine-tune its parameters to improve its accuracy. Finally, we'll compare the tuned model with the base one to choose the best option for predicting fraudulent activities accurately and reliably.

### **Dataset Information**: <br>
This project utilizes a raw dataset sourced from kaggle.com titled *"Fraud Detection Dynamics: Financial Transaction"* uploaded by Rohit Sharma. The dataset provides comprehensive information about transactions, with a particular focus on identifying fraudulent activities. With over 6 million entries, it offers a rich and diverse collection of transactional data for analysis and modeling. For access to the dataset source, you can click [here](https://www.kaggle.com/datasets/rohit265/fraud-detection-dynamics-financial-transaction/data) or [download here](https://drive.google.com/file/d/1RwXs7S4xVicwS_KPvnO1KNR4bQLH2kpq/view?usp=sharing).

### **Dataset Description Table**:

| **Column Names** | **Description** |
| --- | --- |
| `step` | Represents a unit of time in the transaction process, though the specific time unit is not specified in the dataset. It could denote hours, days, or another unit, depending on the context. |
| `type` | Describes the type of transaction, such as transfer, payment, etc. This categorical variable allows for the classification of different transaction behaviors. |
| `amount` | Indicates the monetary value of the transaction, providing insight into the financial magnitude of each transaction. |
| `nameOrig` | Serves as the identifier for the origin account or entity initiating the transaction. This helps trace the source of funds in each transaction. |
| `oldbalanceOrg` | Represents the balance in the origin account before the transaction occurred, offering a reference point for understanding changes in account balances. |
| `newbalanceOrig` | Reflects the balance in the origin account after the transaction has been processed, providing insight into how the transaction affects the account balance. |
| `nameDest` | Functions as the identifier for the destination account or entity receiving the funds in each transaction. It helps track where the money is being transferred to. |
| `oldbalanceDest` | Indicates the balance in the destination account before the transaction, offering a baseline for assessing changes in account balances due to incoming funds. |
| `newbalanceDest` | Represents the balance in the destination account after the transaction has been completed, providing insight into the impact of incoming funds on the account balance. |
| `isFraud` | A binary indicator (0 or 1) denoting whether the transaction is fraudulent (1) or legitimate (0). This is the target variable for fraud detection modeling. |
| `isFlaggedFraud` | Another binary indicator (0 or 1) which may signal whether a transaction has been flagged as potentially fraudulent. This could serve as an additional feature for fraud detection algorithms. |

---
#### The deployed model can be accessed [here](https://huggingface.co/spaces/dnirfana/fraud-detection-classifier).
