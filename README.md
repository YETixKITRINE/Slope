import matplotlib.pyplot as plt
import numpy as np

# Get user input
y_intercept = float(input("Enter the y-intercept: "))
slope = float(input("Enter the slope: "))

# Generate x values
x = np.linspace(-10, 10, 100)
# Calculate y values
y = slope * x + y_intercept

# Plot the line
plt.plot(x, y, label=f"y = {slope}x + {y_intercept}")
plt.xlabel("x")
plt.ylabel("y")
plt.title("Line Plot")
plt.legend()
plt.grid(True)
plt.show()