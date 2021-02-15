# Arabic word sense disambiguation contex-gloss benchmark

is a benchmark for training and testing Arabic gloss word sense dismbiguation.
the becnhcmark consists of 15549 senses for 5347 unique words with an average of 3 senses for each word. Most of the words(+4000) have from 2 to 4 senses , about 750 word have between 4-6 senses per word and the count decreases as the number of senses increases. Each record in the dataset is a tuple of three elements: word sense, a context example, and a definition of that word sense. 
the benchmark is in parquet format, and can be loaded using the following code:
```
import pandas as pd
df = pd.read_parquet("Path to 'new_df_pairs' file")
print(df)
```
finetunning_ber.ipynb file contains The code of our experment.
