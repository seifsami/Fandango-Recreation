# Fandango Recreation

Description: A data analysis project attempting to recreate the article by FiveThirtyEight that showed popular website Fandango was inflating movie ratings. Completed using Python, specifically the libraries Pandas and Seaborn, amongst others. 

Original Article: https://fivethirtyeight.com/features/fandango-movies-ratings/

About the dataset: Dataset obtained from [here](https://github.com/fivethirtyeight/data/tree/master/fandango). Data set contains information for Fandango's movie ratings, as well as data scraped from various other movie rating sites.

I began by importing this dataset into Python, where then I cleaned it, performed analysis and created visualizations. [Full process is outlined here](https://github.com/seifsami/Fandango-Recreation/blob/main/FandangoDataAnalysisProject.ipynb)

**Example Code**
```

plt.figure(figsize=(14,6),dpi=200)
sns.kdeplot(data=fandango,x='RATING',clip=[0,5],fill=True,label='True Rating')
sns.kdeplot(data=fandango,x='STARS',clip=[0,5],fill=True,label='Stars Displayed')
plt.legend(loc=(1.05,0.5))

```
**Example Visualization**

![Example Python Project](https://user-images.githubusercontent.com/97905607/189716108-f62f4554-e9f8-4f98-b95e-aeecbe133b32.png)


