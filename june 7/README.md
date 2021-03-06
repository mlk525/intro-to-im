# Production Assignment

<details>
  <summary>(1/2) Digital Art with Transformations</summary>

# Digital Art with Transformations
Having already worked with trigonometric functions and [the rotate() function](https://github.com/mike-leo-k/intro-to-im/blob/master/june%203), I decided to apply the concepts I observed in class, including the translate() function and scaling the the trigonometric function. The final code is [here](https://github.com/mike-leo-k/intro-to-im/blob/master/june%207/digital_art_transformed.pde).

I first translated a sine graph (without scaling, generated by plotting points), with the following result:
<p align="center">
  <img width="700" src="https://github.com/mike-leo-k/intro-to-im/blob/master/june%207/pictures/trans_1.png">
</p>

Then, scaling the graph by a fact of 10:
<p align="center">
  <img width="700" src="https://github.com/mike-leo-k/intro-to-im/blob/master/june%207/pictures/trans_2.png">
</p>

Then, using a for() loop, with pushMatrix() at the beginning followed by an incremental downward translation (using translat(0, i), i += 15) and a subsequent popMatric(), I repeated the sine graph throughout the screen:
<p align="center">
  <br>
  <img width="500" src="https://github.com/mike-leo-k/intro-to-im/blob/master/june%207/pictures/trans_3.png">
</p>

Now, when rotating the coordinate system (with the rotate() transformation), translation is also required for the drawings to be displayed on screen. Implementing the function in the last step, I added a second for loop that would draw the same graphs vertically as well:
<p align="center">
  <img width="500" src="https://github.com/mike-leo-k/intro-to-im/blob/master/june%207/pictures/trans_4.png">
</p>

Using strokeWeight(), I increased the size of the points (and thus the graphs):
<p align="center">
  <br>
  <img width="500" src="https://github.com/mike-leo-k/intro-to-im/blob/master/june%207/pictures/trans_5.png">
</p>

Finally, using random(255) in the stroke(R, G, B) function, I set each point on each graph to have a random color:
<p align="center">
  <br>
  <img width="500" src="https://github.com/mike-leo-k/intro-to-im/blob/master/june%207/pictures/trans_6.png">
</p>


### Final Render
<p align="center">
  <img width="500" src="https://github.com/mike-leo-k/intro-to-im/blob/master/june%207/pictures/final_render.gif">
</p>

### Challenges/Discoveries
* Figuring out how to properly scale up the sine graph. Realizing that the x coroodinate needed to be proportionally scaled as well seems obvious in retrospect.
* I first tried using the fill() function to change the color of the points, but googling told me that stroke() controlled the colors of points.
* Calculating how much translation was required post-rotation. Thinking of the coordinate system as a movable graph sheet really helped.

</details>

<details>
  <summary>(2/2) Data Visualization</summary>
  
# Data Visualization

## Basic Analysis of the 1988 Seoul Olympics Participants & Winners
Having already collected data on this event for another project, I decided to use Processing to complete a simple data visualization of the compiled information. The data on the number of medals won was collected from [here](https://en.wikipedia.org/wiki/1988_Summer_Olympics_medal_table).

The 1988 Olympics were notable for several reasons: it was the first Olympics event with participation from all major blocs in international politics, following two consecutive events that were boycotted by various countries; it was the last Olympics event attended by the Soviet Union; finally, no nation has ever come close to the Soviet Union's utter domination of the medal table, with 55 gold medals and 132 medals in total.

I decided to analyze the performance of countries identified as communist states, due to the fact that most of these states would no longer exist by the following Olympics. A communist country is defined as a state that is administered and governed by a single communist party guided by Marxism–Leninism. I identified communist states using [this](https://en.wikipedia.org/wiki/Communist_state#List_of_communist_states) list.

The compiled list of countries, with their total medals and their status as a communist state (1 if they were, 0 if they were not), looked like this:
<p align="center">
  <img width="400" src="https://github.com/mike-leo-k/intro-to-im/blob/master/june%207/pictures/1988%20olympics.jpg">
</p>

AFter creating the CSV file, I used the [loadTable()](https://processing.org/reference/loadTable_.html) function and a for() loop to read the values of each row (with the row.getInt() function). Adding up the total participants and medals, as well as all the communist states participating and the medals won by them, I was able to display the data visually:
<p align="center">
  <br>
  <img src="https://github.com/mike-leo-k/intro-to-im/blob/master/june%207/pictures/data_vis_1.png">
</p>

With the bar on top representing the number of participating communist states out of all participants, and the second bar depicting the number of medals won by communist states out of all medals won. I printed the values calculated numerically as well:
<p align="center">
  <br>
  <img src="https://github.com/mike-leo-k/intro-to-im/blob/master/june%207/pictures/data_vis_2.png">
</p>

### Challenges/Discoveries
* Wasn't sure how to read the values from each row and use them for calculations. The [loadTable()](https://processing.org/reference/loadTable_.html) page was immensely helpful to figure this out.


## Visualization of Police Killings of Black Americans by State
Can be found [here](https://github.com/mike-leo-k/intro-to-im/blob/master/june%208%20(image_manipulation)/).

</details>
