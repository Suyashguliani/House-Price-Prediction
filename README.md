# House-Price-Prediction
This project uses machine learning to predict housing prices based on various features like the presence of a guestroom, basement, and other house characteristics. The model is built using a Linear Regression algorithm to estimate the price of a house given these features.

To run the project, you'll need Python and the following libraries:

--pandas
--scikit-learn

python housing_price_prediction.py
--The script will train a Linear Regression model and display the R² score for the predictions on the test data.

Data
--The dataset used for this project is Housing.csv, which contains the following columns:

----mainroad: Whether the house is on the main road (binary: "yes"/"no")
----guestroom: Whether the house has a guestroom (binary: "yes"/"no")
----basement: Whether the house has a basement (binary: "yes"/"no")
----hotwaterheating: Whether the house has hot water heating (binary: "yes"/"no")
----airconditioning: Whether the house has air conditioning (binary: "yes"/"no")
----prefarea: Whether the house is in a preferred area (binary: "yes"/"no")
----furnishingstatus: The furnishing status of the house (categorical: "furnished", "semi-furnished", "unfurnished")
----price: The price of the house (continuous variable)


Model Explanation
--The project uses a Linear Regression model to predict the house prices. Here's the process:

Preprocessing:

--Convert binary categorical columns (mainroad, guestroom, basement, etc.) to numeric values (1 for "yes", 0 for "no").
--Label encode the furnishingstatus column to transform the categorical values into numerical ones.

Train-Test Split:
--The dataset is split into training and testing sets using an 80-20 ratio.

Model Training:
--A Linear Regression model is trained on the training set (X_train and y_train).

Prediction and Evaluation:
--The trained model is used to predict house prices on the test set (X_test).
The performance of the model is evaluated using the R² score.

Results
--After running the model, it outputs the R² Score, which is a measure of how well the model explains the variance in the target variable (price). A higher R² score indicates a better fit of the model to the data.
--R² Score: <calculated_value>

License
--This project is licensed under the MIT License - see the LICENSE file for details.
