# coqui-frogs

Do you hear those Coqui Frogs?

![Final Product Example](https://github.com/junior-devleague/coqui-frogs/blob/master/assets/example.png)

## Objective

Use **Window setInterval** methods, **HTML Audio** and **CSS** positioning to recreate the coqui frog scene!

## Prerequisites

To complete this project, students should have the following:
* Basic understanding of HTML structures.
* Basic understanding of JavaScript and DOM (Variables, Functions, getElementById)

## Concepts

JS | Description
---| -----------
setInterval | A method that calls a function every so many milliseconds. Resource: https://www.w3schools.com/jsref/met_win_setinterval.asp

## Your Challenge

### Part I

To complete Part I, fulfill the following requirements:
1. Set up your project file structure through the command line.
2. Create the following:
* HTML file
* CSS file
* JS file
* Assets folder (from repo)
3. Link all of your files correctly.

---

### Part II HTML

To complete Part II, fulfill the following requirements:

1. Create an ```audio``` element with an ```id``` of "sound". Set the ```src``` of this element to the correct path to the frog-sound.wav file.

2. Create FIVE ```img``` elements. Each element should have a ```src``` with the correct path to the bush.png image, a ```class``` of "bush" and an ```id``` of "bush1", "bush2", "bush3", "bush4", and "bush5" for each element. This is an example of one of them.

``` html
<img id="bush1" src="bush.png" alt="">
```

3. Create an ```img``` element with an ```id``` of "frog". Set the ```src``` of this element to the correct path to the frog.jpg image file.

---

### Part III CSS

To complete Part III, fulfill the following requirements:
1. Target the ```class``` of "bush".
* Set the ```position``` to a value that will make our images fixed to the location we want. Which value would that be? Resource: https://www.w3schools.com/cssref/pr_class_position.asp
* Set the ```bottom``` to 0px.

2. Target the ```id``` of "bush1".
* Set the ```width``` to 480px.
* Set the ```height``` to 400px.

3. Target the ```id``` of "bush2".
* Set the ```width``` to 450px.
* Set the ```height``` to 450px.
* Set the element 300px away from the left edge of the window. How do we do that? Resource: https://www.w3schools.com/cssref/pr_class_position.asp

4. Target the ```id``` of "bush3".
* Set the element to be 550px away from the left edge of the window.

5. Target the ```id``` of "bush4".
* Set the ```width``` to 500px.
* Set the ```height``` to 500px.
* Set the element to be 100px away from the right edge of the window.

6. Target the ```id``` of "bush5".
* Set the ```width``` to 430px.
* Set the ```height``` to 430px.
* Set the element to be 20px away from the right edge of the window.

7. Target the ```id``` of "frog".
* Set the ```position``` to fixed.
* Set the element 230px away from the bottom and 200px away from the left edge of the window.
* Make it so that the frog is BEHIND the bushes. How do we do that? Research the z-index property: https://www.w3schools.com/cssref/pr_pos_z-index.asp

---

### Part IV JS

To complete Part III, fulfill the following requirements:
1. Create a window.onload function as follows:

``` javascript
window.onload = function() {
  // Put the rest of your code on here!
}
```
When the window loads, all your code will be run!

2. Create a ```variable``` called "sound" that will store and get the audio element by id.

``` JavaScript

var sound = document.getElementById('putyourIDinhere!');
```

3. Create a ```variable``` called "frog" that will store and get the frog image by id.

``` JavaScript
var frog = document.getElementById('putyourIDinhere!');
```

4. Create a function called ```frogCroak```. In this function, make the sound play! Look up how to play audio in JavaScript: https://www.w3schools.com/jsref/met_audio_play.asp.

``` JavaScript
function frogCroak() {
  // how do we make our sound play?
}

```

5. Create a ```setInterval``` method that will run this function every 3000 milliseconds (3 seconds). Resource: https://www.w3schools.com/jsref/met_win_setinterval.asp

``` JavaScript

setInterval(nameOfFunction, milliseconds);
```
---

## Stretch Goals
1. Let's make our frog alternate between being above the bush and below the bush. You can change the positioning of the frog by using the following code:

``` javascript
frog.style.bottom = "200px";

// Pattern: [element].style.[property] = "[value]";
```
This will set the frog 200px away from the bottom of the window.

In your function, create an if statement that will check if the bottom is NOT equal to "200px". If that is true, set the bottom to 200px. Else, set the bottom to 230px.
