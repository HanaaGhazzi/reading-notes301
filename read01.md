# Responsive Web Design & Float ! 

_Responsive Web design is the approach that suggests that design and development should respond to the user’s behavior and environment based on screen size, platform and orientation._

### FLEXIBLE EVERYTHING 

**The first part, flexible layouts, is the practice of building the layout of a website with a flexible grid, capable of dynamically resizing to any width.** 

#### Relative Viewport Lengths

CSS3 introduced some new relative length units, specifically related to the viewport size of the browser or device. These new units include vw(Viewports width), vh(Viewports height), vmin(Minimum of the viewport’s height and width), and vmax(Maximum of the viewport’s height and width). 

_Reason being, the viewport height and width continually change from device to device. Website layouts need to adapt to this change and fixed values have too many constraints._

### Media Queries

**Media queries were built as an extension to media types commonly found when targeting and including styles. Media queries provide the ability to specify different styles for individual browser and device circumstances**

![media](https://www.seobility.net/en/wiki/images/6/6f/Media-Queries.png)

> Each media query may include a media type followed by one or more expressions. Common media types include all, screen, print, tv, and braille. The HTML5 specification includes new media types, even including 3d-glasses. Should a media type not be specified the media query will default the media type to screen.

### Flexible Media

**The final, equally important aspect to responsive web design involves flexible media. As viewports begin to change size media doesn’t always follow suit. Images, videos, and other media types need to be scalable, changing their size as the size of the viewport changes.**

![css](https://www.creativemediaworks.com/blog/wp-content/uploads/2014/01/Responsive-Graphic-1.jpg)


## What is “Float”?

_Float is a CSS positioning property. To understand its purpose and origin, we can look to print design. In a print layout, images may be set into the page such that text wraps around them as needed._


### What are floats used for?
floats can be used to create entire web layouts.

### Clearing the Float :
Float’s sister property is **clear**. An element that has the clear property set on it will not move up adjacent to the float like the float desires, but will move itself down past the float. Again an illustration probably does more good than words do.
 
 ### Techniques for Clearing Floats

- The Empty Div Method:
div is the most common because it has no browser default styling, doesn’t have any special function, and is unlikely to be generically styled with CSS. 

- The Overflow Method
This method can be beautifully semantic as it may not require additional elements. However if you find yourself adding a new div just to apply this, it is equally as non-semantic as the empty div method and less adaptable. 

- The Easy Clearing Method
uses a clever CSS pseudo selector (:after) to clear floats. Rather than setting the overflow on the parent, you apply an additional class like “clearfix” to it.



