# NumPy — Numerical operations

| Tool                  | What it does                      | Example                     |
| --------------------- | --------------------------------- | --------------------------- |
| `np.array()`          | Creates an array                  | `np.array([1,2,3])`         |
| `np.arange()`         | Creates a number sequence         | `np.arange(0, 10)`          |
| `np.linspace()`       | Creates evenly spaced numbers     | `np.linspace(0, 10, 5)`     |
| `np.zeros()`          | Creates an array of zeros         | `np.zeros(5)`               |
| `np.ones()`           | Creates an array of ones          | `np.ones(5)`                |
| `np.mean()`           | Calculates average                | `np.mean(x)`                |
| `np.median()`         | Calculates median                 | `np.median(x)`              |
| `np.std()`            | Calculates standard deviation     | `np.std(x)`                 |
| `np.var()`            | Calculates variance               | `np.var(x)`                 |
| `np.min()`            | Finds minimum                     | `np.min(x)`                 |
| `np.max()`            | Finds maximum                     | `np.max(x)`                 |
| `np.sum()`            | Adds values                       | `np.sum(x)`                 |
| `np.sqrt()`           | Calculates square root            | `np.sqrt(25)`               |
| `np.round()`          | Rounds numbers                    | `np.round(3.14159, 2)`      |
| `np.abs()`            | Gets absolute value               | `np.abs(-10)`               |
| `np.reshape()`        | Changes array dimensions          | `x.reshape(2, 3)`           |
| `np.random.rand()`    | Generates random decimal values   | `np.random.rand(5)`         |
| `np.random.randint()` | Generates random integers         | `np.random.randint(1,10,5)` |
| `np.where()`          | Conditional replacement/filtering | `np.where(x > 5, 1, 0)`     |

Usually imported as:

```import numpy as np```

NumPy's main object is an array.

```numbers = np.array([1, 2, 3, 4, 5])```

Array properties
```
x.shape
x.ndim
x.size
x.dtype
```

These tell you:

shape → dimensions
ndim  → number of dimensions
size  → total elements
dtype → type of data

NumPy math is element-by-element

```x = np.array([1, 2, 3])

x + 5
```

Produces:
```
[6 7 8]
```
You can also do:
```
x * 2
x / 2
x ** 2
```