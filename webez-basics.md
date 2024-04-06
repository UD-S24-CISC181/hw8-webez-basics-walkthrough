---
title: WebEZ Basics Walkthrough
layout: page
---

# WebEZ Basics Walkthrough

This walkthrough will help you build and deploy your first WebEZ application. You will learn how to create components, bind values, and handle basic events.

## 0) Setup

1. Click the Github classroom link to create your own copy of the starter repo: <https://classroom.github.com/a/xps8JAYp>
2. Clone the repo to your local machine in an appropriate directory.
3. Open the directory in VS Code, as you normally do.
4. Run `npm install` to install the dependencies.

```bash
npm install
```

5. Normally, you would then run `npm run start` to start the development server. However, we will be using the integrated debugger in VS Code. Activate this by pressing `F5` on your keyboard (or selecting the "Run" tab from the top menu and then clicking `Start Debugging`). This will open a new browser window with your application running. The debugger has a bunch of useful features, like setting breakpoints and inspecting variables - we'll talk more about them later on.

6. You should now be able to see your website. It won't be very exciting at first, but you can now start editing the code and see the changes in real-time!

## 1) Basic HTML

Let's start by adding some dynamic text to the page. We'll need to edit the `MainComponent`, which came with the starter repo. This is the main component that is displayed on the page, and there's always exactly one of them in every WebEZ application. Although we created the component for you, we haven't done anything else. Let's add some text to the page.

1. Expand the `src/app` folder in the sidebar. You will see four files there: `main.component.ts`, `main.component.html`, `main.component.css`, and `main.component.test.ts`. 

![Expand the src/app folder](images/src_app_example.png)

  * `main.component.html` is the HTML file that defines the structure of the component. This is where we put the visual content of your application.
  * `main.component.css` is the CSS file that defines the styles for the component. This is how we make things look pretty.
  * `main.component.ts` is the TypeScript file that defines the `MainComponent` class. This is where the application logic will go.
  * `main.component.test.ts` is a (mostly empty) test file for the component. We'll talk more about testing your own components later on.

2. Open `main.component.html`. You will see that it contains the following code:

```html
<div>
    <div class="header">
        <div class="title">hw8-webez-basics Example</div>
    </div>
</div>
```

This is the default content that comes with the starter repo. The `div` tag is a generic container that can hold other elements (a "division" of content). In this case, we have a `div` with the class `header`, which contains a `div` with the class `title`. The `class` attribute is used to apply CSS styles to the element. We'll talk more about CSS later on. For now, focus on the text inside of the `div` tags.

3. Change the text inside the `div` with the class `title` to something else. For example, you could change it to:

```html
<div class="title">My First WebEZ Application</div>
```

4. Save the file. You should see the changes reflected in the browser window automatically. If you don't see the changes, make sure that the debug mode is still running. 

5. Now, let's add a new element to the page with some more text. Add the following code after the `div` with the class `header`, but inside the outer `div`. The `p` tag is used to create a paragraph of text.

```html
<p>Welcome from the HTML side!</p>
```

If you did this correctly, the HTML should look something like the HTML below. Pay close attention to the structure of your HTML, and make sure you are closing all of your tags properly. The location of tags is important, as it determines how the elements are displayed on the page.

```html
<div>
    <div class="header">
        <div class="title">My First WebEZ Application</div>
    </div>
    <p>Welcome from the HTML side!</p>
</div>
```

6. Save the file, and confirm that the new text is displayed in the browser window.
7. We're going to modify the `p` tag to include an `id` attribute. This will make it easier to test our application later on. Add the `id` attribute to the `p` tag, like so:

```html
<p id="example-text">Welcome from the HTML side!</p>
```

Make sure you use the exact `id` value (`example-text`) as shown above. When you save the file, the page will not look any differently. The `id` attribute is used to uniquely identify an element in the HTML document, but does not affect the appearance of the element.

8. Now, let's add some dynamic text to the page. We're going to use TypeScript to change the text of a new `p` tag. Make a second, empty `p` tag with an `id` after the existing one, like so:

```html
<p id="example-target"></p>
```

<details>
<summary>Click here to see the full HTML so far</summary>

```html
<div>
    <div class="header">
        <div class="title">My First WebEZ Application</div>
    </div>
    <p id="example-text">Welcome from the HTML side!</p>
    <p id="example-target"></p>
</div>
```
</details>

> [!IMPORTANT]
> Make sure you are matching the `id` values exactly as shown above. This will become important when we run the tests later!

9. Open `main.component.ts`. This is the TypeScript file that defines the `MainComponent` class. This is where the application logic will go. You will see that it contains the following code:

```typescript
import html from "./main.component.html";
import css from "./main.component.css";
import { EzComponent } from '@gsilber/webez';

/**
 * @description MainComponent is the main component of the app
 * @extends EzComponent
 * 
 */
export class MainComponent extends EzComponent {

    constructor() {
        super(html, css);
    }
}
```

In WebEZ, components are defined as classes that extend the `EzComponent` class. The `MainComponent` class is the main component of the application, and it is the component that is displayed on the page. The `constructor` method is called when an instance of the class is created. In this case, we are calling the `super` method with the `html` and `css` variables. This is how we tell WebEZ to use the HTML and CSS files that we created. The `html` and `css` variables are just strings that contain the contents of the HTML and CSS files, imported from the files themselves.

10. Add a new private `string` field to the `MainComponent` class called `myText`, with the initial value `"Hello from the TypeScript side!"`. This field will hold the text that we want to display on the page.

```typescript
private myText: string = "Hello from the TypeScript side!";
```




Set a breakpoint in the code to see the current values of the variables.

Deploy the repo

- Deploy the repo
  - On the github site, go to Settings
  - Click Pages on the left
  - Change the source dropdown to be Github Actions

## 2) Boop Button Component

Make a new component: Boop Button
- cd src/app
- webez component boop-button
- Add the HTML
- Create the component and add it to MainComponent, don't forget to import
- Import the BindValue decorator
- Create the decorated field
- Create the decorated method
  - Try just adding "1", oops that is string concatenation!
  - Need to convert it to a number, do the math, and then convert it back
	
## 3) Image Selector Component
	
Make a new component: Image Selector
- webez component image-selector
- Put at least two images in the assets folder
- Make the image tag
- Make the select box tag
- Add the component at a specific place
- Wire up the select box to the image
- Add in @Change events

## 4) Simple Calculator Component
	
Make a new component: Simple Calculator
- webez component simple-calculator
- Add the HTML
- Create the component and add it to MainComponent, don't forget to import
- Left number, bind value
- Right number, bind value
- Operation select box, bind value
- Result, bind value

- onFirstNumberChange,
- onSecondNumberChange,
- onOperationChange

- calculate button

## 5) Joke Component

Make a new component: Joke
- webez component joke
- Add the HTML
- Create the component and add it to MainComponent, don't forget to import
- Add a span to display the joke
- Add a span to display the punchline
- Add a button to show the punchline
- BindVisibleToBoolean("punchline") for a visible attribute
- @Click("reveal")

## 6) Box Editor Component

Make a new component: Box Editor
- webez component box-editor
- Create the component and add it to MainComponent, don't forget to import
- Copy over the given HTML, piece by piece
- Have to explain the transformer syntax here
- Handle padding
- Handle margin
- Handle background color

## 7) Timer Component

Make a new component: Timer
- webez component timer
- Create the component and add it to MainComponent, don't forget to import
- Add a span to display the time
- Timer event binding to function that increases the number