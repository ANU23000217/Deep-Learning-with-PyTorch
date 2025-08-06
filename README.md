# PyTorch Basics Exercises

## AIM:
Write a Python program using PyTorch that performs the following tasks:

### Software Required:
- Python 3.x
- PyTorch
- Jupyter Notebook (for interactive development and execution)

## Algorithm:


### Step 1:

#### Name: ANU RADHA N
#### Register Number: 212223230018

Perform standard imports
- Import `torch` and `NumPy`.

```python
# CODE HERE
import torch
import numpy as np
```

### Step 2:
Set the random seed for NumPy and PyTorch both to `42`.

```python
# YOUR CODE HERE
seed = 42
np.random.seed(seed)
torch.manual_seed(seed)
```

### Step 3:
Create a NumPy array called `arr` that contains 6 random integers between 0 (inclusive) and 5 (exclusive).

```python
# YOUR CODE HERE
arr = np.random.randint(0, 5, size=6)
print(arr)
```

### Step 4:
Create a tensor `x` from the array above.

```python
# YOUR CODE HERE
x = torch.tensor(arr, dtype=torch.int32)
print(x)
```

### Step 5:
Change the dtype of `x` from `int32` to `int64`.

```python
# YOUR CODE HERE
x = x.type(torch.int64)
print(x)
```

### Step 6:
Reshape `x` into a `3x2` tensor.

```python
# YOUR CODE HERE
x = x.view(3, 2)
print(x)
```

### Step 7:
Return the right-hand column of tensor `x`.

```python
# YOUR CODE HERE
right_column = x[:, 1].unsqueeze(1) 
print(right_column)
```

### Step 8:
Without changing `x`, return a tensor of square values of `x`.

```python
# YOUR CODE HERE
x_squared = x ** 2
print(x_squared)
```

### Step 9:
Create a tensor `y` with the same number of elements as `x`, that can be matrix-multiplied with `x`.
- Use PyTorch directly (not NumPy) to create a tensor of random integers between 0 (inclusive) and 5 (exclusive).

```python
# YOUR CODE HERE

y = torch.randint(0, 5, (2, 3), dtype=torch.int64)
print(y)
```

### Step 10:
Find the matrix product of `x` and `y`.

```python
# YOUR CODE HERE

result = torch.matmul(x, y)
print(result)
```

## Output:
i) Import and set up PyTorch and NumPy.
<img width="450" height="148" alt="image" src="https://github.com/user-attachments/assets/06d306dd-0679-4d0a-81c6-650a41040161" />


ii) Create and manipulate tensors.
<img width="1180" height="153" alt="image" src="https://github.com/user-attachments/assets/590a9a31-36fc-4f88-b1bd-e0474ed371fd" />
<img width="835" height="174" alt="image" src="https://github.com/user-attachments/assets/2e4f9ebc-4d98-4f40-b0dc-760f392ea7b6" />
<img width="419" height="108" alt="image" src="https://github.com/user-attachments/assets/1300e55b-adc4-4434-ad3c-982fb338e243" />
<img width="360" height="237" alt="image" src="https://github.com/user-attachments/assets/99e5f941-8fb9-4e17-a0be-a46555cebeed" />

<img width="523" height="199" alt="image" src="https://github.com/user-attachments/assets/6d5e32d5-77e7-44e4-9774-e775ea0b4939" />
<img width="330" height="141" alt="image" src="https://github.com/user-attachments/assets/dccc6038-61bb-41c7-989a-870478d45ce9" />

iii) Perform matrix operations.
<img width="556" height="126" alt="image" src="https://github.com/user-attachments/assets/88580d3f-b01d-4da2-aa71-6e0dbb7f90f0" />

<img width="577" height="190" alt="image" src="https://github.com/user-attachments/assets/2e74c100-9b00-46b3-aaba-9b19eaaedb81" />


## Result:
Thus, the PyTorch tensor operations, including reshaping, dtype conversion, and matrix multiplication, were successfully performed using the Python program.
