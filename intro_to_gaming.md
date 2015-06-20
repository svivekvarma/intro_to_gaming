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
- The Three Types of Animation
- Using the State Machine

---

# Software

- Createjs : suite of visualization, sound and asset loading tools
- Greensock's GSP : amazing tweening engine

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

# Using Easel JS (or another graphics package)

- Object based graphics
- Easy hierarchical relationships
- 

---

# The Three Types of Animation
## Getting started

---

# Using the State Machine
## Getting started

---
