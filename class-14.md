### CSS
## Table of content

**CSS Transforms**
**CSS Transitions & Animations**


The actual syntax for the transform property is quite simple, including the transform property followed by the value. 
The value specifies the transform type followed by a specific amount inside parentheses.
*Example 2D Rotate :*

 ```bash
 .box-1 {
  transform: rotate(20deg);
}
.box-2 {
  transform: rotate(-55deg);
}
```
*Example 2D Scale :*

```bash
.box-1 {
  transform: scale(.75);
}
.box-2 {
  transform: scale(1.25);
}
```

*Example 2D Translate :*

```bash
.box-1 {
  transform: translateX(-10px);
}
.box-2 {
  transform: translateY(25%);
}
.box-3 {
  transform: translate(-10px, 25%);
}
```
*Example 2D Skew :*

```bash
.box-1 {
  transform: skewX(5deg);
}
.box-2 {
  transform: skewY(-20deg);
}
.box-3 {
  transform: skew(5deg, -20deg);
}
```

As mentioned, for a transition to take place, an element must have a change in state, and different styles must be identified for each state.
The easiest way for determining styles for different states is by using the :hover, :focus, :active, and :target pseudo-classes.

There are four transition related properties in total, including transition-property, transition-duration, transition-timing-function, and transition-delay. 
Not all of these are required to build a transition, with the first three are the most popular.

*Example :*

```bash
.box {
  background: #2db34a;
  transition-property: background;
  transition-duration: 1s;
  transition-timing-function: linear;
}
.box:hover {
  background: #ff7b29;
}
```

 8  simple effects that will add life to your UI :
 
 - Fade in  

 - Change color

- Grow & Shrink

- Rotate elements

- Square to circle

- 3D shadow

- Swing

- Inset border

