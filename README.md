# How to Create SVG Images
**Author: Cory Schneider**

The purpose of this tutorial is to provide an easy way to start creating SVG images, showing how to adjust simple shapes and color.

This tutorial is designed for someone with very little to no experience creating SVG images. 

## Requirements
- A plain text editor
- A decent understanding of basic HTML and XML

Once you have a plain text editor open, an easy image to create right away and gain an understanding of what's going on is a simple circle.

**To do this, start off with:**

    <html>
    <body>
    
    <svg width="100" height="100" >
    	<circle cx="50" cy="50" r="30"  />
    </svg>
    
    </body>
    </html>
*This should produce an image that looks like this:*
![SVG Circle Image](https://i.imgur.com/mQAS2Di.png)

These numbers listed above can be adjusted to change the width, height, X coordinate, Y coordinate, and the radius. To add color, we would add "stroke", "stroke-width" and "fill". This should look like:

    <html>  
    <body>  
      
    <svg width="100"  height="100">  
    <circle cx="50"  cy="50"  r="30"  stroke="blue"  stroke-width="3"  fill="red"  />  
    </svg>  
      
    </body>  
    </html>

<html>  
<body>  
  
<svg width="100"  height="100">  
<circle cx="50"  cy="50"  r="30"  stroke="blue"  stroke-width="3"  fill="red"  />  
</svg>  
  
</body>  
</html>

Other predefined shape elements include:
- Rectangle `<rect>`
- Ellipse `<ellipse>`
- Line `<line>`
- Polyline `<polyline>`
- Polygon `<polygon>`
- Path `<path>`

These predefined shapes are all formatted in a similar way with the main difference being **points (X & Y)** and **style**.

**Example for a polygon:**

    <html>
    <body>
    
    
    <svg height="250" width="350">
    	  <polygon points="100,5 125,95 80,105" style="fill:red;stroke:black;stroke-width:2" />
    </svg>
    
    </body>
    </html>
	
*This should produce an image that looks like this:*

![SVG Circle Image](https://i.imgur.com/6tvXJAt.png)

Notice the points of the shape are listed by "x,y x2,y2, x3,y3" and different from the circle, the fill, stroke, and stroke width start with "style=". 

