# Code4mom.js Library

code4mom.js is a simple, light weight Javascript library used for creating simple web applications faster and easier. As this lightweight library supports manipulating DOM (Documents Object Model) which means with code4mom.js you can fully work with DOM elements. <br> Some of the features it provides are as follow:
- Manipulate DOM (Documents Object Model)
- Prevent form action 
- Access the browser web camera (This feature works fully with Chrome and Firefox)
- Create html elements 
- Hiding and showing html elements
- Vibrate device feature.

 Here Is a Documentation that will guide you through using the library:

## Using code4mom.js 
Code4mom.js JavaScript library can be used locally by downloading/cloning to your local system and linking with the html tag:

```html
<script src="code4mom.js"></script>
```
OR By CDN
```html
<script src="https://cdn.jsdelivr.net/gh/yhoungdev/code4mom.js/code4mom.js" ></script>
```

## Functions 
Code4mom.js has different functions for performing different actions, some of it functions are:
- `el()`: This function is used to specify the html element of the tag. This function incorporate DOM manipulation attributes. 
- `print()`: Prevent form input. 
- `webCam()`: This function is used to access the browser web camera.
- `hide()`: This function is used to hide an element
- `block()`: This function is used to show an element
- `cls()`: This function is used to create a class
- `remove()`: This function is used to remove a class

More details on code4mom.js functions are provided below:

## Writing to an Element
To write to an element, code4mom.js uses the `el()` function to get the html element, while the `print()` function is used to write to the element. 
```javascript
   <h3></h3> // html 
    el('h3').print('hello world') // hello world
```

## Prevent form input
To prevent form input, use the `el()` function to get the html element, and the `prevent()` to stop it action.
```javascript
 // html
<form>
  <input type="text" name="name">
  <input type="submit">
</form>
  // code4mom.js
  el('form').prevent() // prevent form from reloading
```
This will prevent the form action from reloading

## Access web camera
The `webCam()` function is used to access the browser web camera in code4mom.js, Note the `el()` function to get element of the html tag.
```javascript
<video></video> // html
   // code4mom.js
  el('video').webCam()
```
The `el()` get the element of the video and `webcam()` access your camera. 

## Hiding and showing element
To hide an element, code4mom.js uses the `hide()` function, while `block()` function to show the element.
```javascript
 // html
 <h3>Hello world</h3>
   // code4mom.js
  el('h3').hide() // It hides Hello world
```
```javascript
 // html
 <h3>Hello world</h3>
  // code4mom.js
  el('h3').block() // it shows Hello world
```

## Add and remove class
To add a class, code4mom.js uses the `cls()` function, while to remove class `remove()` is used.
```javascript
 // code4mom.js
el().cls('//classname') // to add class
el('//element').remove() // to remove class
```

## Add Event Listener
The `el()` function to get the element and `on('//your event' , function )` to trigger the Event Listener.
```javascript
 // html
 <button type="button">Click me</button>
   // code4mom.js
  el('button').on('click', ()=> {
      alert('hello this is code4mom.js')
  })
```
This sample get the element of a button and add a click event to it 

## Write to DOM context
The `el()` function to get the DOM element, and the `text()` to write to the DOM.
``` javascript
 // html
 <span></span>
   // code4mom.js
  el('span').text('hello world')
```

## Create an HTML element
To create an HTML element, code4mom.js uses `create()` function while the `elem()` function is to specify the content of the html. For example:<br>
The element of our create() function is `button` and the elem content is **click me**. This piece of Code4mom.js function will then create the html button element. 
```javascript   
    create('button').elem('Click me')
    // this will create a button with Click me elem content
```
```javascript
    create('div').elem('hello testing code4mom')
     // create a div element with the elem content
```
In the sample, this create a div that has a text hello testing code4mom.js

## Device viberator
Snippet: <br>
```javascript
 app().shake(//duration in milliseconds)
```
Example is:
```javascript
  app().shake(2000)
```
In the sample your device vierates for 2 seconds.

## Get input value
The `value()` function is used to get a value from an input filed.
```javascript
    el('input').value()
```

<br><br>
Have any issue, kindly make issue. Pull request welcome as well, but make sure to read the [Contributing Guidelines](./CONTRIBUTING.md) before making a pull request. 
