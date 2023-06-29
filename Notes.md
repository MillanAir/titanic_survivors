# PPS (Predictive Power Score)
```python
import ppscore as pps # importing ppscore
```
Correlation matrices can identify the degree of linear relationship between two variables. However, they are not able to identify more complex relationships. __PPS overcomes this limitation__ by using a different metric to quantify the relationship between two variables. PPS is able to identify complex relationships such as: `Non-Linear Relationships`, `Monotonic Relationships`, `Thresholded Relationships` and `Interactions`.

[More on This Here](https://towardsdatascience.com/rip-correlation-introducing-the-predictive-power-score-3d90808b9598)

# Feature Engineering
As I noticed in number of references that feature engineering was crucial step for ace predictions. As I have gone through numerous notebooks on Kaggle, I have found there are various ways to make your own unique feature, some examples are mentioned below:
1. Age can be categorized as `Child`, `Adult` and `Old` and then can be converted to `One Hot Encoding`. This will avoid overfitting. Since the ages were diverse so the categories were made accordingly. For eg. `Infant`, `Child`, `Teenager`, `Young Adult`, `Adult`, `Senior` and `Old` were the categories made for age.
2. From the names we can extract the `Titles` like Mr., Mrs., etc. and can keep only the last names. Another piece of information we gain from the names is that a _person is married or not_. For eg. if the name is `Mrs. John Smith` then we can say that the person is married. This can be done by checking if the name contains `Mrs.` or `Mr.` or `Miss.` or `Master.`.
3. Another interesting thing is that you aren't limited to the data provided to you. Once you get a piece of information then there are various ways to gain more information online. For eg. Titanic Dataset contains the cabin numbers or Deck number but it is difficult to visualize so we can get the blueprints of titanic from google and can get the deck information from there. Here is an example of the same:![Titanic Blueprint](https://vignette.wikia.nocookie.net/titanic/images/f/f9/Titanic_side_plan.png/revision/latest?cb=20180322183733)
4. 