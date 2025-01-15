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
