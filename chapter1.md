---
title: 'Creating Pivot Tables in Python Pandas'
description: 'Chapter description goes here.'
free_preview: true
---

## Introduction to Pandas Pivot Tables

```yaml
type: NormalExercise
key: e8c1edbe67
lang: python
xp: 100
skills: 2
```

In out first exercise we will create our very first pivot table in python.

`@instructions`
- Import pandas as pd, and seaborn as sns
- Load the tips dataset by using load_dataset() method of seaborn into dataframe `df`. The input argument should be `'tips'`
- Check the head of your dataframe
- Use pandas pivot_table() method to create a pivot table. Use the `sex` as the index, `day` as the columns, and the `tip` for the values to be shown inside the table.

`@hint`


`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}
import ____ as ____
import ____ as ____

df = sns.load_dataset('tips')
df.____()

df.pivot_table(index='sex', columns='day', values='tip')
```

`@solution`
```{python}
import pandas as pd
import seaborn as sns

df = sns.load_dataset('tips')
df.head()

df.pivot_table(index='sex', columns='day', values='tip')
```

`@sct`
```{python}

```
