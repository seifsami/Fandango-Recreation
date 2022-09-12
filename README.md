# Fandango Recreation

Description: A data analysis project attempting to recreate the article by FiveThirtyEight that showed popular website Fandango was inflating movie ratings. Completed using Python, specifically the libraries Pandas and Seaborn, amongst others. 

Original Article: https://fivethirtyeight.com/features/fandango-movies-ratings/

About the dataset: Dataset obtained from [here](https://github.com/fivethirtyeight/data/tree/master/fandango). Data set contains information for Fandango's movie ratings, as well as data scraped from various other movie rating sites.

I began by importing this dataset into Python, where then I cleaned it, performed analysis and created visualizations. [Full process is outlined here.](https://github.com/seifsami/Fandango-Recreation/blob/main/FandangoDataAnalysisProject.ipynb)

**Example Code**
```
def move_legend(ax, new_loc, **kws):
    old_legend = ax.legend_
    handles = old_legend.legendHandles
    labels = [t.get_text() for t in old_legend.get_texts()]
    title = old_legend.get_title().get_text()
    ax.legend(handles, labels, loc=new_loc, title=title, **kws)
fig, ax = plt.subplots(figsize=(15,6),dpi=150)
sns.kdeplot(data=norm_scores,clip=[0,5],shade=True,palette='Set1',ax=ax)
move_legend(ax, "upper left")

```
**Example Visualization**
![Example Python Project Alt](https://user-images.githubusercontent.com/97905607/189716902-8cf320ec-a500-4773-b399-3e55753be263.png)

