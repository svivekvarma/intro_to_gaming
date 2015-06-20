autoscale: true
footer: © New York Code + Design Academy 2015
slidenumbers: true

#[fit] Welcome to <br/>Intro To Game Development

---

# Who Is this guy?
- Developer in games for 10 years
- Started off as a tools developer at Electronic Arts, Microsoft and Vanguard Studios

![left](resources/me.jpg)

---


# Who Is this guy?
- Worked in game project for education and medicial studies since 2007
- Work at Little Bird Games
- Instructor for New York Development Accademy

![left](resources/me.jpg)

---

# Workshop structure
- A little philosophy
- Working with the Canvas
- Benefits of a graphics package
- The Three Types of Animation
- Basic interaction

---

# Software

- Easeljs : suite of visualization, sound and asset loading tools
- Tweenjs : excellent tweening engine
- https://github.com/wlongmire/intro_to_gaming

---

# Other Javascript Gaming Frameworks: 

- http://impactjs.com/
- https://phaser.io/
- http://gamua.com/area-51/

---

# These frameworks tend to focus on 2D gaming experiences and the tools crafted for them.

---

# Where is the play?

---

## Tools learned will work for any quick visualization tool you want to make from scratch.

---

# Working with the Canvas

---

# Working with the Canvas
- Introduced in HTML
- Allows for in browser rendering of 2D shapes and images
- Low level graphics interface. Fast and works with pixels.
- Can be used for 3d rendering using webgl

---

# Working with the Canvas
- Just a rectangle used for graphic rendering
- Can be accessed and styled just like any other html element

---

# Notes on Scalable Vector Graphics [SVG]
- Many data visualization packages are build using SVG
- Vector based, useful for importing/exported file formats
- All objects are saved as DOM objects. 
- Easy traversal and higher level.

---

# Working with the Canvas

```html
<canvas id="myCanvas" width="600" height="200"></canvas>
```

```javascript
<script>

    var canvas = document.getElementById('myCanvas');
    var context = canvas.getContext('2d');

</script>
```

---

# Working with the Canvas

- Contexts allow you to do simple drawing to the canvas

```javascript
<script>

    var canvas = document.getElementById('myCanvas');
    var context = canvas.getContext('2d');

    // do cool things with the context
    context.fillStyle = "green";
    context.fillRect(10,10, 100, 100);

    context.font = '40pt Calibri';
    context.fillStyle = 'blue';
    context.fillText('Hello World!', 150, 100);

</script>
```

---

# Working with the Canvas
## __Reference:__ http://www.w3schools.com/tags/ref_canvas.asp

---

# Using EaselJS

---

# Using EaselJS
## Just one part of the Createjs library

Libraries for sound, preloading assets, and tweening are also available.

---

# Why use EaselJS

- Object based graphics
- Easy hierarchical relationships
- Sprite Sheet integration
- Graphic Filters
- Interaction and touch events

---

# Why use EaselJS

- Object based graphics
- Easy hierarchical relationships
- Sprite Sheet integration
- Graphic Filters
- Interaction and touch events

---

# Using EaselJS

- createjs.stage object points to and controls canvas
- createjs.shape object holds drawn graphics
- craetejs.bitmap object holds images
- createjs.container object holds composite graphic objects
- http://www.createjs.com/docs/easeljs/classes/Graphics.html

---

# The Three Types of Animation
## The Game Loop Tweening, and Sprites

---

# Animating with the Game Loop

---

# Animating with the Game Loop

- A Game loop (or render loop) is a common pattern used in computer graphics.
- A single function at regular intervals.
- Graphic objects are updated according to a speed based on the time between function calls.
- The stage is redrawn.
- Used for user interactions, physics simulations, 

---

# Animating with the Game Loop
- In Easel this is accomplished using the Ticker class.
```javascript
    createjs.Ticker.addEventListener("tick", tick);
    //setup stage and shape object
    //attach to stage
  
    function tick() { 
	shape.x += 1;
	stage.update();
    }

```
---

# Animating with tweens
- Allows for pre-set sequences of animations
- Animations are automatically generated over time for any attribute over a given length of time.
- stage updates are handled automatically
- Also requires an implicit use of the Ticker class
- Great for flashy animations that do not require environment interaction (UI, feedback)
- Look at greenback's GSP package when you get a chance.

---

# Animating with tweens

```javascript
    
    //assume circle created and added to stage
    createjs.Tween.get(circle)
          .to({ x: 100 }, 500, createjs.Ease.linear)

    createjs.Ticker.setFPS(60);    
    createjs.Ticker.addEventListener("tick", stage);

```
---

# Animating with tweens

```javascript
    
    //assume circle created and added to stage
    createjs.Tween.get(circle)
          .to({ x: 100 }, 500, createjs.Ease.linear)

    createjs.Ticker.setFPS(60);    
    createjs.Ticker.addEventListener("tick", stage);

```

---

# Animating with sprites

- Used for character based 2d animation and pixel art.
- Takes a sequence of static images and shows them in sequence over a length of time.

---

# Animating with sprites

![inline](resources/sonic.gif)

---

# Animating with sprites

http://www.htmlgoodies.com/html5/client/html5-gaming-how-to-animate-sprites-in-canvas-with-easeljs.html#fbid=T8__qj8V36e

---

# Simple Interaction

---

# Simple Interaction
- Easel Allows for 

---