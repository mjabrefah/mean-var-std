# Mean-Variance-Standard Deviation Calculator

This project implements a function `calculate()` that uses Numpy to compute various statistical measures for a 3x3 matrix.

## Function Description

The `calculate()` function is defined in `mean_var_std.py`. It takes a list of 9 numbers as input and returns a dictionary containing the mean, variance, standard deviation, max, min, and sum along both axes and for the flattened matrix.

### Input
- A list containing 9 digits

### Output
A dictionary with the following format:

```python
{
  'mean': [axis1, axis2, flattened],
  'variance': [axis1, axis2, flattened],
  'standard deviation': [axis1, axis2, flattened],
  'max': [axis1, axis2, flattened],
  'min': [axis1, axis2, flattened],
  'sum': [axis1, axis2, flattened]
}
```

### Process
1. The function converts the input list into a 3x3 Numpy array.
2. It then calculates the required statistical measures.
3. The results are returned in the specified dictionary format.

### Error Handling
- If a list containing less than 9 elements is passed into the function, it raises a `ValueError` exception with the message: "List must contain nine numbers."

### Note
The values in the returned dictionary are lists, not Numpy arrays.

## Example Usage

```python
result = calculate([0,1,2,3,4,5,6,7,8])
```

This would return:

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

## Dependencies
- Numpy

## Usage
1. Ensure you have Numpy installed.
2. Import the `calculate()` function from `mean_var_std.py`.
3. Call the function with a list of 9 numbers.

## Contributing
Feel free to open issues or submit pull requests if you have suggestions for improvements or find any bugs.
