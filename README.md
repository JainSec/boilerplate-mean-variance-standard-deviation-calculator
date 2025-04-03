# Mean-Variance-Standard Deviation Calculator

## Project Overview
This project implements a Python function named `calculate()` in `mean_var_std.py` that utilizes NumPy to compute key statistical measures for a 3x3 matrix. The function processes a list of 9 numerical values, converts it into a NumPy array, and returns a dictionary containing the mean, variance, standard deviation, max, min, and sum along both axes and for the entire flattened matrix.

## Features
- Computes statistical measures (mean, variance, standard deviation, max, min, sum) for:
  - Each row
  - Each column
  - The entire matrix
- Utilizes NumPy for efficient computation
- Ensures the input list contains exactly 9 elements, raising a `ValueError` otherwise
- Returns results in a structured dictionary format with lists instead of NumPy arrays

## Function Details
### Function Name: `calculate()`
#### Input:
- A list of exactly 9 numerical values

#### Output:
- A dictionary structured as follows:
  ```python
  {
    'mean': [row_means, column_means, overall_mean],
    'variance': [row_variances, column_variances, overall_variance],
    'standard deviation': [row_std_devs, column_std_devs, overall_std_dev],
    'max': [row_max, column_max, overall_max],
    'min': [row_min, column_min, overall_min],
    'sum': [row_sums, column_sums, overall_sum]
  }
  ```

#### Example Usage:
```python
calculate([0,1,2,3,4,5,6,7,8])
```
##### Expected Output:
```python
{
  'mean': [[3.0, 4.0, 5.0], [1.0, 4.0, 7.0], 4.0],
  'variance': [[6.0, 6.0, 6.0], [0.6666666666666666, 0.6666666666666666, 0.6666666666666666], 6.666666666666667],
  'standard deviation': [[2.449489742783178, 2.449489742783178, 2.449489742783178], [0.816496580927726, 0.816496580927726, 0.816496580927726], 2.581988897471611],
  'max': [[6, 7, 8], [2, 5, 8], 8],
  'min': [[0, 1, 2], [0, 3, 6], 0],
  'sum': [[9, 12, 15], [3, 12, 21], 36]
}
```

## Error Handling
- If the input list contains fewer or more than 9 elements, the function raises a `ValueError` with the message:
  ```plaintext
  "List must contain nine numbers."
  ```

## Requirements
- Python 3.x
- NumPy

## Installation & Setup
1. Clone the repository:
   ```sh
   git clone https://github.com/your-repo-url.git
   ```
2. Navigate to the project directory:
   ```sh
   cd mean-var-std-calculator
   ```
3. Install dependencies:
   ```sh
   pip install numpy
   ```
4. Run the function in Python:
   ```python
   from mean_var_std import calculate
   print(calculate([0,1,2,3,4,5,6,7,8]))
   ```

## Author
- Pulkit Jain
- Contact: jain.infosec@gmail.com





This is the boilerplate for the Mean-Variance-Standard Deviation Calculator project. Instructions for building your project can be found at https://www.freecodecamp.org/learn/data-analysis-with-python/data-analysis-with-python-projects/mean-variance-standard-deviation-calculator
