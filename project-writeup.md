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

Extension Ideas:

- Medium: **TESTS**: Have tests for the core functionality of the game
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

Extension Ideas:

- Medium: **TESTS**: Have tests for the core functionality of the application
- Easy: **DEFAULTS**: Have default buttons for some common habits ("Sleep 8 hours", "Eat Healthy", "Work on Schoolwork")
- Medium: **GOALS**: Add a "weekly goal" for each habit, and make the graph show progress towards the weekly goal.
- Hard: **SAVING**: Have the ability to save and load (either by using localStorage or download/upload files).

## Collaboration Policy

You are allowed to work with one partner **from your lab section** on the final project, but you must COLLABORATE equally.

**If you are going to work together, you must BOTH be making commits from your own account.**

Your Git log will be the authoritative source for your grade. If the Git log does not reflect your shared development, then the partner not represented in the logs will earn zero points (and therefore fail the class).

Note that this means you must be dealing with merge conflicts. You cannot simply code from one person’s computer/git account. We are going to look closely at your logs to make sure you are equally contributing. You cannot have one person write all the TypeScript and one person write all of the HTML/CSS. We will look at the files, not just the commit frequency.

We will run similarity detection code across all repositories, to look for instances where students have shared code. In the case of obvious, abusive code sharing, academic misconduct may be reported. Do not give or take code from any classmates in this course, or from any external source (e.g., tutor, chatgpt). You may base your code off code you found on the internet, but cite sources and make sure you are using it as an example. Refer to the syllabus and, if in doubt, talk to an instructor.

## Milestones

We will have weekly milestone submissions to ensure that you are making adequate progress towards your goal.

* For this assignment (April 21), you must fork the assignment, add your name and UD email to the site (requirement 1), and deploy your site without issues. Refer to [Part 5 of the walkthrough](https://ud-s24-cisc181.github.io/hw8-webez-basics-walkthrough/webez-basics#5-deploy-your-site) for more information about deploying your site (note that you skip the first step, since we have not damaged the deploy file this time). 
* For the first milestone (April 28), we expect you to achieve at least 3 of the requirements (two new requirements since the first requirement of adding your name).
* For the second milestone (May 5), we expect you to achieve at least 5 of the requirements.
* For the third milestone (May 12), we expect you to achieve all 7 of the requirements.
* For the final submission (May 19), we expect you to have finished everything. You will spend this week making sure your code is high-quality in terms of documentation, names, functional decomposition, etc.

### Progress Updates

**New as of 4/22/2024 at 2:39pm**

As you submit milestones, you need to update the `docs/progress.md` file to clearly indicate what requirements you have finished.

First, you will need to [sync the latest version](https://ud-s24-cisc181.github.io/hw8-webez-basics-walkthrough/pull-from-upstream.html) of the upstream repository (both on Github and in your VS Code). There are unlikely to be any merge conflicts, but be prepared to deal with them as needed.
Once you have pulled the latest changes, then you will find a new file in your top-level `docs/` folder named `progress.md` which has checkboxes for you to fill in with `X` marks.
Each time you complete a requirement, you should replace the empty whitespace with an `X`, like so:

```md
- [X] NAME
- [ ] GRID
- [ ] CLICKING
```

Do not remove requirements or alter the requirements' names, or generally modify the rest of the Markdown in the file. Doing so may cause an automatic system to reject your submission or misinterpret your completion rate, and give you a lower grade than you would have otherwise earned. You should only put the `X` in the blank or leave the blank as a whitespace.

Note that if a feature is no longer working, you should clear the box. Claiming that a feature is working when it is not will have negative repurcussions on your grade and is technically academic misconduct.

You can test if your Progress list has deployed successfully by adding `docs/progress` to the end of your URL, which will show a page like this: <https://ud-s24-cisc181.github.io/final-project-template/docs/progress>

## Styling and Creative Freedom

There is some ambiguity in the requirements. Ultimately, the instructors will decide if a given requirement is met. However, there is meant to be some flexibility for you to have more advanced functionality. But you need to make sure you meet the minimum requirements; if you are concerned about whether you are meeting that requirement, then you should check with your TA and/or instructor.

Some extra credit points will be available for functional sites that go above and beyond with their styling. We strongly recommend that, once you have core functionality, you spend some time making your application look the way you want it to. This is something that you could put in your portfolio. Make it look good! It may also influence your grader (people tend to be influenced heavily by how nice websites look, even if we try to be unbiased).

## Code Quality Grading

**New as of 5/07/2024 at 9:50am**

Once you are finished with your project code, check over the following:

* Chosen good variable/function/class names (clear, concise, consistent, conventional, and correct)
* Included good jsdoc documentation for your classes, functions, and methods.
* Decomposed complicated functions with helper functions
* Decomposed components into ways that make sense (not too massive, but also not unnecessary ones)
* Avoided global state (e.g., a global variable). Global *constants* and top-level functions are fine, but storing data in a mutable global variable is bad practice.

Your TA will be grading your code's quality based on the ideas above.

Make sure your program and website runs; **broken programs do not earn points.**

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

To begin the project, follow this link to clone the assignment: <https://classroom.github.com/a/PpxBwu6A>

If you are going to work with a partner, add them to the repository.

Then, complete the first requirement (adding your name and UD email to the site).

Save/add/commit/push, and then make sure your site deploys.

Then start working on the next requirement for your chosen project!

## Frequently Asked Questions (FAQ)

Any commonly recurring questions will be answered here.

**Q:** *Can I work with my friend if they are in a different lab section than I am?*\
**A:** No, you must be in the same lab section to work together. You will be working on the project during lab time, and we will take attendance as usual.

**Q:** *Can I modify the `tsconfig.json`, `.eslintrc.js`, or `.github/workflows/deploy.yml` files?*\
**A:** Tampering with the core infrastructure of the project (e.g., to turn off linting rules) is technically a form of academic dishonesty. Do not modify these files without permission by the instructor. Modifying them can be easily detected on our end and may be reported if it is done to bypass course requirements (e.g., disabling the `No Any Type` rule in the linter). Some files are perfectly fine to modify (e.g., `package.json`, `package-lock.json`) and others you are even invited to modify (e.g., `styles.css`). If you are unsure about whether you can modify a file, just ask!


~~**Q:** *What do you mean by "Have tests for the core functionality of the app"? What are the expectations for tests?*\~~
~~**A:** Our expectations for the tests are actually relatively low, compared to the tests we have had you writing all semester. You are not expected to test WebEZ functionality related to the DOM (HTML+CSS), so you do not need to simulate button clicks or anything (although that is possible, and you are free to do so for extra credit!). Instead, we want you to focus on *core* functionality, making sure it is sufficiently extracted from the interface. Think of the core logic, most complicated logic of your application. For example, in the Lights-Out game, you need to check and manipulate the board; in the habit tracker, you have to group up the habits to determine the bar graph amounts. This kind of logic can be isolated in your application so that you can write some tests for it directly. We expect you to find a way to write some compelling tests for that kind of core functionality. There is no miminum number of tests or amount of coverage that we specifically expect, but you should think about a range of test cases to ensure that you have valid and thorough tests.~~ (Superceded by next FAQ entry)

**Q:** *Why are the tests not required anymore?*\
**A:** A few reasons, but primarily because we didn't think we did enough to prepare you for writing tests and because we want to reward those who have achieved the core functionality. However, the tests ARE important, and we do want you to see that they are valued. Hence, we plan to offer you points if you do a good job writing tests. Note that just having tests is not sufficient, nor is there some minimum number you need. We will only give you points if the tests are *valid* and *thorough*, covering a wide range of interesting cases. If you need ideas on how to write tests for WebEz, we strongly recommend checking out its source code repository (particularly all of the [example applications' tests](https://github.com/gsilber/WebEZ/blob/main/WebEZ-Example/src/app/components/taskviewer/taskviewer.component.test.ts)). You are not required to test that WebEZ works, your goal is to write tests that exercise the functionality you have created with WebEZ. *(Added 5/7/24 at 9:52am)*

**Q:** *I have finished the milestone for this week. Do I have to attend lab?*\
**A:** Lab attendance is required until you have completed the entire project AND confirmed with your TA. When you finish all the requirements, email your TA and ask them to check your deployed site (provide them a link). They will need to respond with a positive confirmation that all requirements are completed. If you miss lab (regardless of your milestone progress), then you will be marked absent.

**Q:** *Am I allowed to use other libraries instead of WebEz?*\
**A:** No, you must use WebEz for this project. We have not covered other libraries in this course, and we want to ensure that you are able to complete the project with the tools we have provided. If you have a specific need that you think WebEz cannot meet, please ask your TA or instructor for help. Note that abusing HTML manipulating code using JQuery or the DOM API (`document.querySelector`) is also not allowed. *(Added 5/7/24 at 9:51am)*

## Change Log

We'll keep track of changes to the project in this Change Log, in case we have to make significant changes or clarifications.

* Version 0.0.1 (4/17/24 at 10:26am): Initial version posted
* Version 0.0.2 (4/18/24 at 1:30am): Added partner from lab specification
* Version 0.0.3 (4/18/24 at 10:39am): Added clarification about tampering with files
* Version 0.0.4 (4/22/24 at 12:53pm): Added clarification on test expectations
* Version 0.1.0 (4/22/24 at 2:45pm): Added Progress Updates section to explain the `progress.md` file
* Version 0.1.1 (4/23/24 at 12:25pm): Included "pull from upstream" link in progress updates section.
* Version 0.1.2 (4/23/24 at 12:37pm): Clarified lab attendance regarding milestones.
* Version 0.2.0 (5/07/24 at 10:00am): 
  * Modified project requirement TESTS to be optional
  * Added section about code style and quality
  * Clarified both in FAQ
