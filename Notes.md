# Notes

## Data Exploration

First step for the task is to explore the data at hand and there are following techniques where we can gain better understanding of our data.

1. Populate Data

   - df.head(5)
   - df.describe
   - pandas profiling report
2. Visualizations

   - Auto Visualization
   - Describe the insights you gained in words like any important patterns
3. Statistics

   - Z-test, T-test is done to check similarities of patterns statistically as numerical evidence is great indicator w.r.t to visualizations.
   - PPS, predictive power score

### PPS (Predictive Power Score)

```python
import ppscore as pps # importing ppscore
```

Correlation matrices can identify the degree of linear relationship between two variables. However, they are not able to identify more complex relationships. **PPS overcomes this limitation** by using a different metric to quantify the relationship between two variables. PPS is able to identify complex relationships such as: `Non-Linear Relationships`, `Monotonic Relationships`, `Thresholded Relationships` and `Interactions`.

[More on This Here](https://towardsdatascience.com/rip-correlation-introducing-the-predictive-power-score-3d90808b9598)

## Learning Techniques

What kind of learning are you planning to use, for eg. Supervised Learning: Classification etc.
Then we can also construct useful features using feature engineering.

### Feature Engineering

I learned that feature engineering was crucial step for ace predictions. Going through numerous notebooks on Kaggle, I have found there are various ways to make your own unique feature, some examples are mentioned below:

1. Age can be categorized as `Child`, `Adult` and `Old` and then can be converted to `One Hot Encoding`. This will avoid overfitting. Since the ages were diverse so the categories were made accordingly. For eg. `Infant`, `Child`, `Teenager`, `Young Adult`, `Adult`, `Senior` and `Old` were the categories made for age.
2. From the names we can extract the `Titles` like Mr., Mrs., etc. and can keep only the last names. Another piece of information we gain from the names is that a _person is married or not_. For eg. if the name is `Mrs. John Smith` then we can say that the person is married. This can be done by checking if the name contains `Mrs.` or `Mr.` or `Miss.` or `Master.`.
3. Another interesting thing is that you aren't limited to the data provided to you. Once you get a piece of information then there are various ways to gain more information online. For eg. Titanic Dataset contains the cabin numbers or Deck number but it is difficult to visualize so we can get the blueprints of titanic from google and can get the deck information from there. Here is an example of the same:![Titanic Blueprint](https://vignette.wikia.nocookie.net/titanic/images/f/f9/Titanic_side_plan.png/revision/latest?cb=20180322183733)

## Pipeline Construction
