
$$
F=P \times(1+r)^t
$$

Here,
- $F$ = Future Value
- $P$ = Present value
- $r$ = rate
- $t$ = time

Einstein Eqn. $E = mc^2$ 

---
### Code


```python
import matplotlib.pyplot as plt

# Parameters
PV = 1000   # Initial investment
r = 0.10    # Annual return rate (10%)
years = 10  # Number of years

# Calculate future values for each year
t = list(range(years + 1))
FV = [PV * (1 + r)**i for i in t]

# Plot
plt.figure(figsize=(6, 4))
plt.plot(t, FV, marker='o', label="10% Annual Return")
plt.title("Index Fund Growth at 10% Annual Rate")
plt.xlabel("Years")
plt.ylabel("Future Value ($)")
plt.grid(True)
plt.legend()
plt.show()
```


![[Pasted image 20250907094835.png]]


### Table

| Year | Return |     |
| ---- | ------ | --- |
| 0    | 1000   |     |
| 5    | 1600   |     |
| 10   | 2600   |     |
|      |        |     |