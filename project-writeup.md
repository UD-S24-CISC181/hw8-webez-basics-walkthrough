---
title: Final Project Writeup
layout: page
---

# Final Project Writeup

Welcome to the Final Project!

You have two options:

- The Lights Out Game: Click the boxes to turn all the lights off!
- A Habit Tracker Application: Keep track of healthy habits

## Specifications

For both applications, we have established minimum criteria. The bulk of the assignment points come from passing these requirements. The examples show the spirit of the requirements, although there is a little wiggle room in exactly how you fulfill them - think of these as the minimum functionality, but if you make a _better_ interface we’ll be open to accepting that!

### Lights Out Game

Instructor Example: <https://ud-s24-cisc181.github.io/example-lights-out/>

Players must be able to:

1. **NAME**: See the authors of the game (name and UD email) visibly on the screen.
2. **GRID**: See a grid of light boxes. The initial state of each box should be random (you're free to choose the likelihood of a box being on), but at least one box must be on.
3. **CLICKING**: Click on a box to change its state and also the states of its neighbors (see VARIANTS below).
4. **VICTORY**: Detect if the game is won (the state of every box is off) and, if so, display a victory message that includes the number of clicks.
5. **RESIZE**: Have buttons to change the width and the height of the grid.
6. **RESET**: Click a button to start a new game.
7. **VARIANTS**: Support variant gameplay where the lights that change are "cardinal neighbors" (the default), "entire row/column", and "diagonal neighbors".
8. **TESTS**: Have tests for the core functionality of the game

Extension Ideas:

- Easy: **MENUS**: Have separate screens for the game title, game over, and victory
- Medium: **LEADER BOARD**: Have a arcade-style persistant leader board that tracks a user-provied name and number of clicks for each variant
- Hard: **SOLVER**: Have a "solve this" button that slowly wins the game by performing the ["follow the lights" algorithm](https://stackoverflow.com/questions/19795973/lights-out-game-algorithm)

### Habit Tracker

Instructor Example: <https://ud-s24-cisc181.github.io/example-habit-tracker/>

Users must be able to:

1. **NAME**: See the authors of the game (name and UD email) visibly on the screen.
2. **LIST**: See a list of default habits
3. **ADD**: Be able to add a new habit with a given name, but display a message if the habit already exists
4. **TRACK**: Provide a way for the user to indicate whether a habit has been completed for the current active day
5. **MOVE**: Be able to change the current active day being tracked using convenient buttons - at minimum, that means the ability to move to the next and previous days
6. **GRAPH**: See a graph (bar chart) with the counts of each habit
7. **REMOVE**: Be able to remove a habit (correctly updating the tracker and graph)
8. **TESTS**: Have tests for the core functionality of the app

Extension Ideas:

- Easy: **DEFAULTS**: Have default buttons for some common habits ("Sleep 8 hours", "Eat Healthy", "Work on Schoolwork")
- Medium: **GOALS**: Add a "weekly goal" for each habit, and make the graph show progress towards the weekly goal.
- Hard: **SAVING**: Have the ability to save and load (either by using localStorage or download/upload files).

## Collaboration Policy

You are allowed to work with one partner on the final project, but you must COLLABORATE equally.

**If you are going to work together, you must BOTH be making commits from your own account.**

Your Git log will be the authoritative source for your grade. If the Git log does not reflect your shared development, then the partner not represented in the logs will earn zero points (and therefore fail the class).

Note that this means you must be dealing with merge conflicts. You cannot simply code from one person’s computer/git account. We are going to look closely at your logs to make sure you are equally contributing. You cannot have one person write all the TypeScript and one person write all of the HTML/CSS. We will look at the files, not just the commit frequency.

We will run similarity detection code across all repositories, to look for instances where students have shared code. In the case of obvious, abusive code sharing, academic misconduct may be reported. Do not give or take code from any classmates in this course, or from any external source (e.g., tutor, chatgpt). You may base your code off code you found on the internet, but cite sources and make sure you are using it as an example. Refer to the syllabus and, if in doubt, talk to an instructor.

## Milestones

We will have weekly milestone submissions to ensure that you are making adequate progress towards your goal.

* For this assignment (April 21), you must fork the assignment, add your name and UD email to the site (requirement 1), and deploy your site without issues. Refer to [Part 5 of the walkthrough](https://ud-s24-cisc181.github.io/hw8-webez-basics-walkthrough/webez-basics#5-deploy-your-site) for more information about deploying your site (note that you skip the first step, since we have not damaged the deploy file this time). 
* For the first milestone (April 28), we expect you to achieve at least 3 of the requirements.
* For the second milestone (May 5), we expect you to achieve at least 5 of the requirements.
* For the third milestone (May 12), we expect you to achieve at least 7 of the requirements.
* For the final submission (May 19), we expect you to have finished everything.

## Styling and Creative Freedom

There is some ambiguity in the requirements. Ultimately, the instructors will decide if a given requirement is met. However, there is meant to be some flexibility for you to have more advanced functionality. But you need to make sure you meet the minimum requirements; if you are concerned about whether you are meeting that requirement, then you should check with your TA and/or instructor.

Some extra credit points will be available for functional sites that go above and beyond with their styling. We strongly recommend that, once you have core functionality, you spend some time making your application look the way you want it to. This is something that you could put in your portfolio. Make it look good! It may also influence your grader (people tend to be influenced heavily by how nice websites look, even if we try to be unbiased).

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

To begin the project, follow this link to clone the assignment:

If you are going to work with a partner, add them to the repository.

Then, complete the first requirement (adding your name and UD email to the site).

Save/add/commit/push, and then make sure your site deploys.

Then start working on the first real requirement for your chosen project!
