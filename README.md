# Task2

import matplotlib.pyplot as plt

# Data for China's population over the years (in millions)
years = list(range(1960, 2021))
population = [
    667.07, 682.33, 697.36, 713.42, 730.27, 746.57, 763.17, 779.73, 796.34, 813.25, 
    829.92, 847.29, 864.40, 881.94, 899.78, 918.01, 936.40, 955.10, 973.75, 992.58, 
    1011.49, 1030.66, 1050.14, 1069.91, 1089.88, 1109.99, 1130.27, 1150.58, 1171.04, 
    1191.53, 1212.04, 1232.61, 1253.02, 1273.47, 1293.88, 1314.48, 1335.17, 1355.83, 
    1376.57, 1397.22, 1417.95, 1438.62, 1459.27, 1479.91, 1500.36, 1520.60, 1540.57, 
    1560.01, 1578.94, 1597.57, 1615.39, 1632.26, 1648.29, 1663.52, 1678.11, 1692.38, 
    1706.45, 1720.24, 1733.83, 1747.16, 1760.34, 1773.54, 1786.34, 1798.47, 1810.47, 
    1821.90
]

# Adjust the population list to match the years (1960-2020)
correct_population = population[:len(years)]

# Creating the bar chart
plt.figure(figsize=(12, 6))
plt.bar(years, correct_population, color='skyblue')
plt.xlabel('Year')
plt.ylabel('Population (in millions)')
plt.title("China's Population Over Time (1960-2020)")
plt.xticks(rotation=45)
plt.grid(axis='y', linestyle='--', alpha=0.7)
plt.show()
