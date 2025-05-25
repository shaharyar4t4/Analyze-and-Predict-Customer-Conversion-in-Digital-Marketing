Analyze and Predict Customer Conversion in Digital Marketing
Description
This project aims to predict customer conversion for an insurance company using machine learning techniques. By analyzing historical marketing and demographic data, the model identifies customers most likely to subscribe to an insurance policy, enabling targeted marketing to improve conversion rates and reduce campaign costs. The project leverages Python libraries such as Pandas, NumPy, Scikit-learn, and XGBoost to preprocess data, perform exploratory data analysis (EDA), and build predictive models.
Table of Contents

Installation
Usage
Project Structure
Data
Methodology

Contributing
License

Installation

Clone the repository:git clone https://github.com/shaharyar4t4/Analyze-and-Predict-Customer-Conversion-in-Digital-Marketing.git


Navigate to the project directory:cd Analyze-and-Predict-Customer-Conversion-in-Digital-Marketing


Create a virtual environment (optional but recommended):python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate


Install dependencies:pip install -r requirements.txt

Ensure you have Python 3.8+ installed. The requirements.txt file includes libraries such as:
pandas
numpy
scikit-learn
xgboost
matplotlib
seaborn



Usage

Place the dataset (Digital Marketing Dataset.csv) in the project root or update the file path in the scripts.
Run the main script to preprocess data, train the model, and generate predictions:python main.py


Explore the Jupyter notebooks (notebooks/) for detailed EDA and model experimentation.
Check the results/ directory for model performance metrics (e.g., AUROC) and visualizations.

Example command to predict conversions for new data:
python predict.py --input new_data.csv --output predictions.csv

Project Structure
├── digital_Marketing.ipynb
├── digital_marketing_campaign_dataset.csv
├── README.md
└── LICENSE

Data
The dataset (Digital Marketing Dataset.csv) contains historical sales data with features such as:

Demographic data (e.g., age, job, marital status, education)
Campaign data (e.g., call type, day of the month, call duration, previous call outcome)
Target variable: Whether the customer subscribed to the insurance (yes/no)

The data is used to train and evaluate machine learning models, with a focus on identifying key factors influencing conversion.
Methodology

Data Preprocessing: Handle missing values, encode categorical variables, and normalize numerical features.
Exploratory Data Analysis (EDA): Analyze feature distributions and correlations to identify patterns.
Model Development: Train and evaluate models (e.g., Logistic Regression, Random Forest, XGBoost) using AUROC as the primary metric.
Feature Importance: Identify critical features contributing to conversion predictions.
Optimization: Perform hyperparameter tuning and address class imbalance using techniques like SMOTE.

For detailed methodology, refer to the Jupyter notebooks in the notebooks/ directory.
Results

Model Performance: The XGBoost model achieved the highest AUROC score, indicating strong predictive power.
Key Features: Call duration, previous call outcome, and customer demographics were among the most influential factors.
Business Impact: The model enables targeted telemarketing, potentially reducing campaign costs by focusing on high-conversion prospects.

Visualizations and metrics are available in the results/ directory.
Contributing

Fork the repository.
Create a new branch (git checkout -b feature-branch).
Commit your changes (git commit -m 'Add new feature').
Push to the branch (git push origin feature-branch).
Open a pull request.

Please adhere to the Code of Conduct and ensure contributions align with the project’s goals.
License
This project is licensed under the MIT License - see the LICENSE file for details.
