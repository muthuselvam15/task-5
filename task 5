import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Load dataset
df = pd.read_csv("twitter_training.csv", header=None)
df.columns = ['ID', 'Entity', 'Sentiment', 'Tweet']

print(df.head())
print(df.info())

# Sentiment distribution
plt.figure(figsize=(6,4))
sns.countplot(x='Sentiment', data=df)
plt.title("Sentiment Distribution")
plt.show()

# Top entities
plt.figure(figsize=(8,4))
df['Entity'].value_counts().head(10).plot(kind='bar')
plt.title("Top 10 Entities in Tweets")
plt.show()
