# Health Insurance Cost Prediction

## Overview
This project predicts health insurance costs using a Linear Regression model. The dataset contains various features like age, BMI, smoking status, and region to estimate the insurance charges.

## Dataset
The dataset consists of 1338 records and 7 columns:
- `age`: Age of the individual
- `sex`: Gender (encoded as 0 for male, 1 for female)
- `bmi`: Body Mass Index
- `children`: Number of dependents
- `smoker`: Smoking status (encoded as 0 for yes, 1 for no)
- `region`: Residential region (encoded as 0: southeast, 1: southwest, 2: northeast, 3: northwest)
- `charges`: The actual insurance cost (target variable)

## Requirements
Ensure you have the following dependencies installed:
```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

## Project Structure
- `insurance.csv`: Dataset file
- `insurance_analysis.ipynb`: Jupyter Notebook with data analysis and model training
- `README.md`: Project documentation

## Steps
1. **Data Loading & Preprocessing**
   - Encoded categorical variables
   - Checked for missing values
   - Split data into features (`X`) and target (`Y`)

2. **Exploratory Data Analysis (EDA)**
   - Visualized distributions of age, BMI, and charges
   - Analyzed categorical features like smoker and region

3. **Model Training**
   - Used Linear Regression for prediction
   - Achieved an R² score of ~0.75 on training and ~0.74 on test data

4. **Prediction System**
   - Takes user input and predicts insurance cost

## Usage
Run the Jupyter Notebook to train and evaluate the model. You can test predictions with custom inputs like:
```python
input_data = (31,1,25.74,0,1,0)
prediction = regressor.predict([input_data])
print('Predicted Insurance Cost:', prediction[0])
```

## Future Enhancements
- Implement non-linear models (Random Forest, Gradient Boosting)
- Feature engineering for better accuracy
- Deploy as a web application

## Author
Vaibhavkr2004

## License
This project is open-source and available under the MIT License.

