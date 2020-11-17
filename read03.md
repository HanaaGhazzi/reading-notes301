# Javascript Templating

_Javascript templating is a fast and efficient technique to render client-side view templates with Javascript by using a JSON data source. The template is HTML markup, with added templating tags that will either insert variables or run programming logic._

### Mustache 
![why](https://miro.medium.com/max/875/1*P9q0tkeaRY2l1JOXaVKAig.png)
**As the name suggests, it was named mustache because the syntax resembles a Mustache. E.g. {{ placeholder }}**

> Mustache is a logic-less template syntax. It can be used for HTML, config files, source code — anything. It works by expanding tags in a template using values provided in a hash or object.


> **mustache.js** :is an implementation of the mustache template system in JavaScript. It is often considered the base for JavaScript templating. And, since mustache supports various languages, we don’t need a separate templating system on the server side.


## A Complete Guide to Flexbox 

1. **Properties for the Parent (flex container)**
![cont.](https://css-tricks.com/wp-content/uploads/2018/10/01-container.svg)
- display : This defines a flex container; inline or block depending on the given value. It enables a flex context for all its direct children.

- flex-direction : This establishes the main-axis, thus defining the direction flex items are placed in the flex container. Flexbox is (aside from optional wrapping) a single-direction layout concept. 

- flex-wrap :
1. nowrap (default): all flex items will be on one line
2. wrap: flex items will wrap onto multiple lines, from top to bottom.
3. wrap-reverse: flex items will wrap onto multiple lines from bottom to top.

![wrap](https://webdesignerwall.com/wp-content/uploads/2017/01/wrap.jpg)

- flex-flow : This is a shorthand for the flex-direction and flex-wrap properties, which together define the flex container’s main and cross axes. The default value is row nowrap.


- justify-content:
![just](https://css-tricks.com/wp-content/uploads/2018/10/justify-content.svg)

2. **Properties for the Children (flex items)**

![child](https://css-tricks.com/wp-content/uploads/2018/10/02-items.svg)
- Order : By default, flex items are laid out in the source order. However, the order property controls the order in which they appear in the flex container.

- flex-grow : This defines the ability for a flex item to grow if necessary. It accepts a unitless value that serves as a proportion. It dictates what amount of the available space inside the flex container the item should take up. 

- flex-shrink : This defines the ability for a flex item to shrink if necessary. 

- flex-basis : This defines the default size of an element before the remaining space is distributed. It can be a length (e.g. 20%, 5rem, etc.) or a keyword. The auto keyword means “look at my width or height property” (which was temporarily done by the main-size keyword until deprecated). The content keyword means “size it based on the item’s content” – this keyword isn’t well supported yet, so it’s hard to test and harder to know what its brethren max-content, min-content, and fit-content do. 

 - flex :This is the shorthand for flex-grow, flex-shrink and flex-basis combined. The second and third parameters (flex-shrink and flex-basis) are optional. The default is 0 1 auto, but if you set it with a single number value, it’s like 1 0.

 - align-self : This allows the default alignment (or the one specified by align-items) to be overridden for individual flex items.
![align](https://www.w3.org/TR/css3-flexbox/images/align-content-example.svg)


