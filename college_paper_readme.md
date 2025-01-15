use college paper theme to style your plots

Setup:
---

```py
import matplotlib
print(matplotlib.get_configdir())
```

Use Example:
---

```py
import matplotlib.pyplot as plt

# Load the custom style
plt.style.use('college_paper.mplstyle')

# Create a sample plot
fig, ax = plt.subplots()
ax.plot([0, 1, 2, 3, 4], [0, 1, 4, 9, 16], marker='o', label='y = x^2')
ax.set_xlabel('X-axis')
ax.set_ylabel('Y-axis')
ax.set_title('Plot on College-Lined Paper')
ax.legend()

plt.show()

```

Use in Pandas:
```py
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt

# Load the custom style
plt.style.use('college_paper.mplstyle')

# Create a sample DataFrame
data = {
    'x': np.arange(10),
    'y': np.random.rand(10) * 10,
    'z': np.random.rand(10) * 5
}
df = pd.DataFrame(data)

# Plot using pandas
df.plot(x='x', y='y', kind='line', marker='o', title='Pandas Plot on College-Lined Paper')

# Show the plot
plt.show()
```

### Additinal Customization if Needed:

```py

# Plot using pandas with additional customizations
ax = df.plot(x='x', y='y', kind='line', marker='o', figsize=(8, 5), title='Pandas Plot on College-Lined Paper')
ax.set_xlabel('X-axis')
ax.set_ylabel('Y-axis')
ax.legend(['Custom Line'])

# Show the plot
plt.show()
```

- You can also combine multiple styles by passing a `list to plt.style.use()`, e.g. `plt.style.use(['college_paper.mplstyle', 'seaborn'])`

  
