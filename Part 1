# -*- coding: utf-8 -*-
"""MohammadThaher_21110274.ipynb

Original file is located at
    https://colab.research.google.com/drive/1sGtexTXCQC7FCzXFeeZ8vqKaQsQ2l6pK
"""

# Importing libraries
import pandas as pd  # For data manipulation and analysis
import numpy as np  # For numerical operations
import matplotlib.pyplot as plt  # For creating static, animated, and interactive visualizations
import seaborn as sns  # For data visualization based on matplotlib

# Loading the data
network_data = pd.read_csv('/content/WSNBFSFdataset.csv')

# Displaying the dataframe
network_data

# Display basic information about the dataset (Nulls / Data Types / column names)
print("Dataset Overview:")
network_data.info()

# Display the first five rows of the dataset
print("First Five Rows of the Dataset:")
network_data.head()

# Summary statistics of the numerical columns
print("Summary Statistics: ")
network_data.describe()

#Calculate the correlation matrix for the DataFrame
correlation_matrix = network_data.corr()
correlation_matrix

sns.heatmap(correlation_matrix, cmap="Blues")

# Visualization - histogram of 'Rest_Energy'
plt.figure(figsize=(10, 6))
sns.histplot(data=network_data, x='Rest_Energy', hue='behaviour', palette='Set2')
plt.title('Rest Energy histogram')
plt.show()

# Visualization - Line plot of 'Time' to identify outliers
plt.figure(figsize=(10, 6))
plt.plot(network_data['Time'], network_data['behaviour'])
plt.title('Behaviour vs Time')
plt.xlabel('Time (seconds)')
plt.ylabel('Behaviour')
plt.show()

# Visualization 1: Box plot of 'Rest_Energy'
plt.figure(figsize=(10, 6))
sns.boxplot(y='Rest_Energy', data=network_data, hue='Type', palette='Set1')
plt.title('Box Plot of Rest_Energy')
plt.ylabel('Rest_Energy')
plt.legend(loc='best')
plt.show()

# Visualization 2: Bar plot of 'Packet_Size' to show the count of occurrences
plt.figure(figsize=(10, 6))
sns.countplot(x='Packet_Size', data=network_data, hue='behaviour', palette={'No attack': 'lightblue', 'Under attack': 'red'})
plt.title("Bar Plot of Packet_Size by Behaviour")
plt.xlabel("Packet_Size")
plt.ylabel("Count")
plt.legend(title="Behaviour")
plt.show()

# Box plot to identify outliers
plt.figure(figsize=(10, 6))
sns.barplot(data=network_data, x='Type', y='Packet_Size')
plt.title('Packet Size Distribution by Type')
plt.xlabel('Type')
plt.ylabel('Packet Size')
plt.show()

# Time Range
time_range = network_data['Time'].max() - network_data['Time'].min()
print("Time Range:", time_range)

# Plot the time and event data
plt.plot(network_data['Time'], network_data['Event'])
plt.xlabel('Time (seconds)')
plt.ylabel('Number of events')
plt.show()

# Visualization 3: Scatter plot of 'Time' against 'Rest_Energy'
plt.figure(figsize=(10, 6))
sns.scatterplot(data=network_data, x='Time', y='Rest_Energy', hue='behaviour', palette={'No attack': 'blue', 'Under attack': 'red'})
plt.title("Scatter Plot of (Time vs. Rest_Energy by Behaviour)")
plt.xlabel("Time (seconds)")
plt.ylabel("Rest_Energy")
plt.legend(title="Behaviour")
plt.show()

# Create a contingency table for 'Type' and 'behaviour'
contingency_table = pd.crosstab(network_data['Type'], network_data['behaviour'])

# Display the contingency table
print("Contingency Table:")
contingency_table
