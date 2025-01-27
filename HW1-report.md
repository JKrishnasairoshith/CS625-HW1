# HW 1 - CS 625, Spring 2025

Krishna Sai Roshith Jonnalagadda 

Due: January 26, 2025

## Git, GitHub

What is the URL of the GitHub repo that you created in your personal account?

   [https://github.com/JKrishnasairoshith/CS625-HW1](https://github.com/JKrishnasairoshith/CS625-HW1)

What is pull vs clone in GitHub?
-  **Pull**: The `git pull` command is used to fetch the latest changes from a remote repository and merge them into your local repository.
- **Clone**: The `git clone` command creates a local copy of a remote repository, allowing you to work on it locally.
You have committed a change on your local machine/remote. However, you want to undo the changes committed. How would you do that?

To undo a commit on your local machine (before pushing it to the remote):

To keep changes in the working directory:

git reset --soft HEAD~1

To discard the commit and changes:

git reset --hard HEAD~1

If the commit has been pushed to the remote,we will use git revert to create a new commit that undoes the changes:

git revert <commit_id>

## Markdown

Create a bulleted list with at least 3 items
- Study for the exam
- Complete homework assignments
- Go to the gym

Write a single paragraph that demonstrates the use of italics, bold, bold italics, code, and includes a link. The paragraph must explain your favorite Olympic sport/game, the country that won the most number of olympic GOLD medals (Summer) in your favorite sport in 2020 (Japan) and 2024 (France). You are free to include more information.
- One of my favorite Olympic sports is **basketball**. The USA has won the most Olympic GOLD medals in basketball in both the 2020 (Japan) and 2024 (France) Olympics. I enjoy watching the exciting moments of the game, especially the **_three-point shots_**. I always think of **Stephen Curry**, a fantastic player who can hit incredible three-pointers. Basketball is such an exciting game! You can check out more details about basketball's Olympic history [here](https://en.wikipedia.org/wiki/Basketball_at_the_Summer_Olympics).

Create a level 3 heading

### My Favorite Olympic Sport

Insert a image of your favorite Olympics sport/game, sized appropriately
![Basketball](https://github.com/JKrishnasairoshith/CS625-HW1/blob/main/Basketball.jpeg)

## Tableau

Insert the image of your horizontal bar chart here. Reminder, this should show countries that won the least number of medals only (excluding ZERO) in Paris2024 Summer Olynpics by continent (one country from each continent is ok).

In Tableau, In this chart, I have filtered the countries that won the least number of medals in the Paris 2024 Summer Olympics, excluding those with zero medals. The range is set from 10 to 126 medals to focus on countries that have won at least 10 medals. This helps highlight the performance of countries with a more significant number of Olympic achievements, while excluding those with fewer medals. The chart visualizes the countries with the least number of medals within this range.

Below is the chart showing these countries:

![Paris 2024 Summer Olympics - Least Medal Countries](https://github.com/JKrishnasairoshith/CS625-HW1/blob/main/Sheet%201%20(2).png?raw=true)
## Google Colab

What is the URL of your Google Colab notebook? " https://colab.research.google.com/drive/15ihCwqTNwFYZntnNnl7RBEDXEYNKSfYQ "

## Python/Seaborn

Insert the first penguin chart here

![Alt Text](https://github.com/JKrishnasairoshith/CS625-HW1/blob/main/Penguin%201.png)


Describe what the figure is showing.

The image above is a scatter plot showing the relationship between **bill length (in mm)** on the x-axis and **bill depth (in mm)** on the y-axis for a set of penguins. From the plot, it appears that there is a positive correlation between the two variables, meaning that as the bill length increases, the bill depth tends to increase as well, although not in a perfect linear manner.

There are several clusters of data points, which might indicate variations across different penguin species, though the species are not explicitly identified in this plot. The background of the plot is light gray, with grid lines that help in reading the values for both axes. The data points are represented as filled circles, and the axes are clearly labeled to show the measurements of bill length and bill depth.

This visualization provides a clear picture of how these two variables are related in the penguin dataset.

Insert the second penguin chart here
![Penguin 2 Image](https://github.com/JKrishnasairoshith/CS625-HW1/blob/main/Penguin%202.png)

Describe what the figure is showing.

The image above is a bar chart showing the body mass (in grams) of penguins across three species: Adelie, Gentoo, and Chinstrap. The chart compares the body mass of male and female penguins within each species. The bars for male penguins are colored in blue, and the bars for female penguins are colored in orange.

From the chart, we can observe that male penguins generally have a higher body mass compared to female penguins across all three species. Among the species, Gentoo penguins have the highest average body mass, followed by Chinstrap and Adelie penguins. The differences between male and female penguins in body mass are more pronounced in some species than others.

This visualization helps highlight the differences in body mass between genders within each species and provides a clear comparison of the sizes of different penguin species.

What happened when you removed the outer parentheses from the code? Why?

If you remove the outer parentheses in the second figure code, the code will no longer run as expected. In Python, parentheses are required to group function calls and method chaining properly

## Observable and Vega-Lite

What happens when you replace `markCircle()` with `markSquare()`?

When you replace markCircle() with markSquare(), the data points on the scatterplot will change from circles to squares. The shape of the marks will alter, but the data points and the relationships they represent will remain the same. Essentially, this is a visual change, where each point is rendered as a square instead of a circle.


What happens when you replace `markCircle()` with `markPoint()`?

markPoint() is typically used for points or individual marks in a scatterplot, similar to markCircle(). The main difference is that markCircle() renders the points as circles, while markPoint() may not explicitly define the shape unless specified. In some cases, markPoint() defaults to the standard point marker shape, which may be a smaller, simpler version of a circle. If no specific shape is set for markPoint(), it may have a different visual appearance from markCircle().

What change do you need to make to swap the x and y axes on the scatterplot?

To swap the x and y axes in a scatterplot, you would need to swap the encoding of the x and y fields in your Vega-Lite specification. For example, if the 

original code has:

"encoding": {
  "x": {"field": "fieldX", "type": "quantitative"},
  "y": {"field": "fieldY", "type": "quantitative"}
}

You would change it to:

"encoding": {
  "x": {"field": "fieldY", "type": "quantitative"},
  "y": {"field": "fieldX", "type": "quantitative"}
}

This swaps the fields used for the x and y axes.

Insert the bar chart image here

![Alt text](https://github.com/JKrishnasairoshith/CS625-HW1/blob/main/Vega-Lite.png)

Why do you think this chart is the result of this code change?

This bar chart is the result of changing the mark type from `markPoint()` to `markBar()`. The `markBar()` type is used to display data as bars, which is appropriate for comparing discrete categories. The change from point marks to bar marks results in a clear visual representation of the data in the form of bars, each representing a different category.


## References

Every report must list the references (including the URL) that you consulted while completing the assignment. Replace the items below with the references you consulted

 Reference 1, (https://docs.python.org/3/)
 Reference 2, (https://vega.github.io/vega-lite/docs/)
