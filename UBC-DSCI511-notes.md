# DSCI 511 Python Programming for Data Science Notes
## Linters and Formatting

Use `flake8` and `balck` package to check the style and formats of `.py` files

- `flake8` - `!flake8 path/file.py`
- `black` - `black path/file.py --check`, `black path/file.py`


## Numpy

### Create an array

- `np.linesapce(start, end, n)` Create an array with `n` equally spaced points between `start` and `end` 
- `np.full((r, c), num)` Create an 'r' * 'c' array full of 'num' values
- `np.random.rand(r, c)` Crate an 'r' * 'c' array with random values between 0 and 1 \[0, 1) from a uniform distribution 

### Methods and Attributes of `ndarray`

- `ndarray.transpose()`
- `ndarray.astype()`
- `ndarray.mean()`
- `ndarray.ndim`: number of dimension
- `ndarray.shape`: number of elements in each dimension
- `ndarray.size`: total number of elements in ndarray

### Broadcasting

ndarrays with different sizes cannot be used in arithmetic operations

- **NOT** all dimensions of arrays can be broadcasted. The dimensions have to:
    1. The dimensions have to equal, or
    2. One of the dimension is 1

### Reshaping Arrays

- `reshape()`
- `newaxis()` - add dimensions to an array for broadcasting purposes
- `revel()` / `flatten()` - "flatten" arrays to a single dimension
- 