﻿# Simple animation using HTML and CSS

This example shows how to create a spinner with just HTML and CSS.

The code is explaned bellow:

Initially all the border will be solid, with 16px kinda gray (#f3f3f3)
```
border: 16px solid #f3f3f3;
```

Then, 1/4 of the border will be this color blue (#3498db), or the color you wish:
```
border-top: 16px solid #3498db;
```

This sets the width and height of the circle:
```
width: 120px;
height: 120px;
```

The type of the animation will be `spin`, the duration, or the time of a 360 degrees rotation, will be `2s` (2 seconds). Linear indicates that the animation will have the same speed from the begin to the end (check possible values [here](https://www.w3schools.com/cssref/css3_pr_animation-timing-function.asp)). `infinite`, well the animation will never end...
```
animation: spin 2s linear infinite;
```

`@keyframes` is used to change the state of an element during the animation, you can set the states you wish when animating. Check more [here](https://www.w3schools.com/css/css3_animations.asp).
```
@keyframes spin{
	0% { transform: rotate(0deg); }
	100% { transform: rotate(360deg); }
}
```

You can see the code working [here](https://jsfiddle.net/tommfernandes/8bd4vhgL/).
