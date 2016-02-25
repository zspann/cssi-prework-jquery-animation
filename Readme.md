---
tags: cssi, javascript, jquery
level: 2
languages: javascript
---
#Animation with jQuery and CSS
One of the cooler features of jQuery is animation. The concept is pretty simple:

1. Use selectors to indicate which DOM elements to animate
2. Set a target CSS style and an optional time
3. jQuery gradually changes the style from one to the other, automatically calculating the intermediate styles at each millisecond

## Animation using the animate() Method
The animate() method is the most flexible method. The full syntax for the animate() method is below:

`$(selector).animate({params},speed,callback);`

* *params* - defines the CSS properties to be animated, must be numerical properties
* *speed* (optional) - specifies the duration of the effect "slow", "fast", or milliseconds
* *callback* (optional) - the function to be executed after the animation completes.

Here's an example:
```js
$('p').animate(
    {fontSize: 24},
    1500
)
```
Here we are changing the style of each paragraph to a font size of 24 (the params) over a period of 1500 ms (the speed).

## Animation Shortcuts
There are also some convenient shortcut methods for common animations developers use all the time:
* .slideUp()/ .slideDown() - an element moves up/down
* .fadeIn()/.fadeOut() - Show/Remove an element with a slow fade


Animation powers a multitude of web experiences - when a page has satisfying button clicks, when elements fade or slide (or both!) nicely onto and off the page - all excellent animation. Animation can be bad too - when the sliding is too slow, or the fades and slides in and out look cartoonish and silly.

##Resources

As with color, font, position, whitespace, and design generally, there is far more depth to animation than we are going to cover. You can check out [this tutorial](http://www.sitepoint.com/guide-jquery-animate-method/) to learn more. As always, getting good takes practice.

Check the [documentation](https://api.jquery.com/category/effects/) for more examples and explanations.
