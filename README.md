# credit-risk-classification

# CODE GIVEN IN MODULES

# Calculating the confusion matrix
cm = confusion_matrix(y_test, predictions)
cm_df = pd.DataFrame(
    cm, index=["Actual 0", "Actual 1"], columns=["Predicted 0", "Predicted 1"]
)

# Calculating the accuracy score
acc_score = accuracy_score(y_test, predictions)

-------------------------------------------

# Splitting into Train and Test sets
X_train, X_test, y_train, y_test = train_test_split(X, y, random_state=78)

-------------------------------------------

# Create predictions using the testing data
y_pred = knn.predict(X_test_scaled)

-----------------------------------------

# Print the classification report comparing the testing data to the model predictions
print(classification_report(y_test, y_pred))

----------------------------------------

# Split the dataset
X_train, X_test, y_train, y_test = train_test_split(X, y, random_state=1)

---------------------------------------

