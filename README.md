# Regression Analysis Project

This repository contains implementations of various regression techniques using Python, NumPy, and Matplotlib.

## Overview

The project consists of three main parts:
1. Multilinear Regression
2. Generalized Regression with Polynomial Kernel
3. Generalized Regression with Non-polynomial Kernel

## Requirements

- Python 3.x
- NumPy
- Matplotlib

```bash
pip install numpy matplotlib
```

## Project Structure

```
├── data/
│   ├── Q1_data.txt
│   ├── regression_data_multiGen_group_25_train.txt
│   └── regression_data_uni_group_25_train.txt
├── src/
│   ├── multilinear_regression.py
│   ├── polynomial_regression.py
│   └── nonpolynomial_regression.py
└── README.md
```

## Features

### 1. Multilinear Regression
- Implementation with and without bias terms
- Data normalization
- Performance metrics:
  - Pearson Correlation
  - Mean Squared Error
  - Mean Absolute Error

### 2. Polynomial Regression
- Support for quadratic, cubic, and bi-quadratic terms
- Feature engineering
- Visualization of results
- Performance evaluation

### 3. Non-polynomial Regression
- Implementation of sigmoid activation
- Trigonometric feature transformations
- Regularization support
- Correlation analysis

## Usage

```python
# Example usage for multilinear regression
import numpy as np
from src.multilinear_regression import MultilinearRegression

# Load and preprocess data
X_train, y_train = load_data('data/Q1_data.txt')

# Create and train model
model = MultilinearRegression(with_bias=True)
model.fit(X_train, y_train)
```

## Results

The project includes various evaluation metrics:
- Correlation coefficients
- Mean Square Error
- Root Mean Square Error
- Visualization plots

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.
