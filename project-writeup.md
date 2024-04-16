Welcome to the Final Project!

You have two options:

- The Lights Out Game: Click the boxes to turn all the lights off!
- A Habit Tracker Application: Keep track of healthy habits

## Specifications

For both applications, we have established minimum criteria. The bulk of the assignment points come from passing these requirements. The examples show the spirit of the requirements, although there is a little wiggle room in exactly how you fulfill them - think of these as the minimum functionality, but if you make a _better_ interface we’ll be open to accepting that!

### Lights Out Game

Instructor Example:

Players must be able to:

1. See a grid of light boxes, all initially lit up
2. Click on a box to change its state, and also invert the state of the four adjacent lights
3. Detect if the game is won when all the lights are turned off, and display a victory message.
4. Have buttons to change the width and the height of the game.
5. Click a button to start a new game, and display the number of times the player has won
6. Support variant gameplay where the lights that change are “cardinal neighbors” (the default), “entire row/column”, and “diagonal neighbors”.
7. Have tests for the core functionality of the game

Extension Ideas:

- Easy: Have separate screens for the game title, game over, and victory
- Hard: Have a “solve this” button that slowly wins the game by performing the “follow the lights” algorithm

### Habit Tracker

Instructor Example:

Users must be able to:

1. See a list of default habits
2. Be able to add a new habit with a given name, but display a message if the habit already exists
3. Provide a way for the user to indicate whether a habit has been completed for the current active day
4. Be able to change the current active day being tracked using convenient buttons - at minimum, that means the ability to move to the next and previous days
5. See a graph (bar chart) with the counts of each habit
6. Be able to remove a habit (correctly updating the tracker and graph)
7. Have tests for the core functionality of the app

Extension Ideas:

- Easy: Have default buttons for some common habits (“Sleep 8 hours”, “Eat Healthy”, “Work on Schoolwork”)
- Medium: Add a “weekly goal” for each habit, and make the graph show progress towards the weekly goal.
- Hard: Have the ability to save and load (either by using localStorage or download/upload files).

## Collaboration Policy

You are allowed to work with one partner on the final project, but you must COLLABORATE equally.

**If you are going to work together, you must BOTH be committing.**

Your Git log will be the authoritative source for your grade. If the Git log does not reflect your shared development, then the partner not represented in the logs will earn zero points (and therefore fail the class).

Note that this means you must be dealing with merge conflicts. You cannot simply code from one person’s computer/git account. We are going to look closely at your logs to make sure you are equally contributing. You cannot have one person write all the TypeScript and one person write all of the HTML/CSS. We will look at the files, not just the commit frequency.

We will run similarity detection code across all repositories, to look for instances where students have shared code. In the case of obvious, extravagant code sharing, academic misconduct may be reported. Do not give or take code from any classmates in this course, or from any external source (e.g., tutor, chatgpt). You may base your code off code you found on the internet, but cite sources and make sure you are using it as an example.

## Milestones

We will have weekly milestone submissions to ensure that you are making adequate progress towards your goal.

For this assignment (April 21), you simply must fork the assignment and deploy your site without issues.

For the first milestone (April 28), we expect you to achieve at least 2 of the requirements.

For the second milestone (May 5), we expect you to achieve at least 4 of the requirements.

For the third milestone (May 12), we expect you to achieve at least 6 of the requirements.

For the final submission (May 19), we expect you to have finished everything.

## Styling and Creative Freedom

There is some ambiguity in the requirements. Ultimately, the instructors will decide if a given requirement is met. However, there is meant to be some flexibility for you to have more advanced functionality. But you need to make sure you meet the minimum requirements; if you are concerned about whether you are meeting that requirement, then you should check with your TA and/or instructor.

Some extra credit points will be available for functional sites that go above and beyond with their styling.

We strongly recommend that, once you have core functionality, you spend some time making your application look the way you want it to. This is something that you could put in your portfolio. Make it look good!

## Help Resources

You will need to make effective use of the help resources we have available.

- [Documentation for Webez](https://gsilber.github.io/WebEZ/)
- Example Webez applications:
  - [Task List](https://gsilber.github.io/WebEZ/example) ([source code](https://github.com/gsilber/WebEZ/tree/main/WebEZ-Example))
  - [Movies](https://gsilber.github.io/WebEZ/movies) ([source code](https://github.com/gsilber/WebEZ/tree/main/movies))
  - [Lander](https://gsilber.github.io/WebEZ/lander) ([source code](https://github.com/gsilber/WebEZ/tree/main/lander))
  - [Pong](https://gsilber.github.io/WebEZ/webpong) ([source code](https://github.com/gsilber/WebEZ/tree/main/web-pong))
- Good resources for HTML:
  - [MDN Tutorial](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics)
  - [W3 Schools Reference](https://www.w3schools.com/tags/default.asp)
- Good resources for CSS:
  - [MDN Tutorial](https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps/Getting_started)
  - [W3 Schools Reference](https://www.w3schools.com/cssref/index.php)

Be cautious in how much help you accept, since you will need to be able to explain and justify every line you submit - if you don’t understand something, you need to learn how it works before you can use it!

## Submission

The final submission for the project (and this assignment) will be a deployed website. Failure to deploy means that you will earn zero points.

## Starting

To begin the project, follow this link to clone the repo.

If you are going to work with a partner, add them to the repository.
