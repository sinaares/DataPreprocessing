Data Preprocessing Template (Machine Learning)
This project provides a basic data preprocessing pipeline in Python, commonly used as the first step in a Machine Learning workflow. It includes steps for handling missing data, encoding categorical variables, splitting the dataset, and feature scaling.

📁 Dataset
The project expects a CSV file named Data.csv in the same directory as the script. The file should contain:

At least one categorical feature in the first column (e.g., country names),

Numerical columns with possible missing values,

A target/output column in the last column (e.g., "Yes"/"No").

📦 Libraries Used
numpy

pandas

matplotlib (not used but imported for future visualizations)

scikit-learn

⚙️ Preprocessing Steps
Load Dataset
Reads the CSV and separates it into features x and target y.

Handle Missing Data
Uses SimpleImputer to replace missing values in numerical columns with the column mean.

Encode Categorical Variables

One-Hot Encoding for the first column (e.g., countries)

Label Encoding for the target column

Split Dataset

80% training set

20% test set

Feature Scaling
Applies standardization (StandardScaler) to numerical columns (excluding encoded columns).

🧪 Output
After preprocessing, it prints:

x_train: Scaled and encoded feature set used for training

x_test: Scaled and encoded feature set used for testing

📝 Example Usage
bash
Copy
Edit
python data_preprocessing.py
Ensure Data.csv is in the same directory.

📌 Notes
Change test_size=0.2 and random_state=1 for different splits.

You can extend this script for model training and evaluation after preprocessing.
