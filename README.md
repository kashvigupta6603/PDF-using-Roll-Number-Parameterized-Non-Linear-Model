# Learning Probability Density Function from Air Quality Data

This project learns a probability density function (PDF) from real-world air quality data using basic statistical methods and Python.

The main goal is to understand how data distributions can be modeled and visualized from raw data.

---

## Dataset

- Name: India Air Quality Data
- Source: Kaggle
- Feature used: NO2 (Nitrogen Dioxide)

Only the NO2 column is used for analysis in this project.

---

## Approach

### Data Transformation

The input variable x is transformed using:

z = x + a sin(bx)

For the chosen parameters, the transformation does not change the data, so:

z = x

---

### Probability Density Function

The transformed data is modeled using:

p(z) = c · exp(−λ (z − μ)²)

This form is similar to a Gaussian distribution.

---

### Parameter Calculation

- μ (mu): mean of the data
- σ² (variance): variance of the data
- λ (lambda): 1 / (2σ²)
- c: sqrt(λ / π)

These values are computed directly from the dataset.

---

## Final Parameters

μ (mu)     = 25.809623  
λ (lambda) = 0.001460  
c          = 0.021561  

---

## Visualization

The output includes:
- Histogram of NO2 values
- Learned probability density function plotted on top

This helps visualize how well the distribution fits the data.

---

## Tools Used

- Python
- NumPy
- Pandas
- Matplotlib

Works on Google Colab and local Python environments.

---

## How to Run

1. Clone the repository
2. Download the dataset from Kaggle
3. Place the CSV file in the project folder
4. Run the Python script or notebook

---

## Notes

- Results are reproducible
- No randomness is used
- Focus is on understanding PDF learning from real data

---

## Author

Undergraduate Student
