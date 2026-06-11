# Flexbox

## What is Responsive Web Design

**Responsive web design (RWD)** is a development approach that allows for elements to dynamically change its appearance or layout depending on screen size. For example, elements may reorder, grow/shrink in size depending on the size of the screen.

There are different methods for incorporating responsive design. In this lab, we will explore a tool called **Flexbox** that helps create a fluid layout for website responsiveness. To learn more about other methods, check out [MDN Doc on responsive design](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Responsive_Design).

## Flexbox at a Glance

**Flexbox** (or Flexible Box) creates a flexible container around items. It is an efficient way to position, align, and distribute items that are responsive to screen size. When discussing the Flexbox Layout, we will identify two key terms: flex container and flex items.

![Image of flexbox container](https://css-tricks.com/wp-content/uploads/2018/10/01-container.svg)
![Image of flexbox items](https://css-tricks.com/wp-content/uploads/2018/10/02-items.svg)
Source: [CSS Tricks](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

- **Flex container:** This is a container or grouping of items. Properties for the container include organizing the direction, wrap, distribution, and alignment of the items contained in the flex container.
- **Flex item:** This refers to the elements contained in the flex container. Properties for the items include the order of items, changes in size based on screen size, and self-alignment compared to other items.

## Creating a Flexbox Container and Items

You may be wondering, how do we even define or create a Flexbox container and items? Typically developers use the `div` HTML element to create sections that will then be defined as a Flexbox. In the CSS style file, we add a rule for these `div` containers that set the property `display` to the value `flex`.

```css
.container {
	display: flex;
}
```

In the example above, we create a rule that all `div` elements with the class name `container` will have the `display` property with value `flex` (aka a Flexbox!). Once you have defined a flex container, all elements inside automatically act as flex items.
