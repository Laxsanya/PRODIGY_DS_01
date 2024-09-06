import pandas as pd
import numpy as np
import matplotlib.pyplot as plt

df=pd.read_excel('/content/population(3).xlsx')
print(df)
plt.figure(figsize=(10,8))
plt.bar(df['Country Name'],df['population of country'],color='red')
plt.title('population')
plt.xlabel('year')
plt.ylabel('country')
plt.show()

plt.hist(df['population of country'],color='skyblue',bins=20)
plt.show()
