Flex Less
=========

Flexbox is awesome! It's a powerful addition to CSS and you should be using it NOW!
The [CSS Flexible Box Layout Module](http://www.w3.org/TR/css3-flexbox/) has been a Candidate Recommendation since September 2012.

> "That’s cool! But I can’t use it because XYZ doesn’t support it."

Since when has that stopped us using box-shadows or border-radius?
Use flexbox now on small page components as progressive enhancement, and with Flex Less you wont have to worry about the countless vendor prefixes for flexbox.

Flex-Less is a mixin created to enable you to use all basic functions of CSS flexbox for all supported browsers.


## Flexbox support
Flexbox has had multiple types of syntax since it's introduction these are...

`display:box`   
Android  
Safari v.3+  
Blackberry v.7+  

`display:flexbox` 
IE v.10  

`display:flex`
Chrome  
Firefox  
Opera  
IE v.11  
Android v.4.4  
Safari v.6+  
Blackberry v.10+  

## Flex-less
If you want to learn more about FlexBox please visit [A Complete Guide to Flexbox](http://css-tricks.com/snippets/css/a-guide-to-flexbox/) a comprehensive and brilliant guide (as always) from CSS Tricks
(descriptions for each section below are from this very guide)

## How to use
Download and import the less file at the start of your less document.

```css
  @import "../flex-less.less";
```

Then you just need to call the mixin on the element you want, for example

```css
.products {
  .flex;
}
```
or change is use by using different variables for each element

```css
.products {
  .flex (flex-inline);
}
```

### Display
This defines a flex container; inline or block depending on the given value. It enables a flex context for all its direct children.

```css
.flex (@flex)
/*
Default:
  flex
@flex:
  flex, flex-inline
*/
```
  
### Flex-direction
This establishes the main-axis, thus defining the direction flex items are placed in the flex container. Flexbox is (aside from optional wrapping) a single-direction layout concept. Think of flex items as primarily laying out either in horizontal rows or vertical columns.

```css
.flex-direction(@type, @direction)
/*
Default:
  row, normal
Varaibles:
  @type: row, column
  @direction: normal, reverse
*/
```

### Flexbox-wrap
By default, flex items will all try to fit onto one line. You can change that and allow the items to wrap as needed with this property. Direction also plays a role here, determining the direction new lines are stacked in.

```css
.flex-wrap (@wrap)
/*
Default:
  wrap
Variables:
  wrap, nowrap, wrap-reverse
*/
```

### Flexbox Justify Content
This defines the alignment along the main axis. It helps distribute extra free space left over when either all the flex items on a line are inflexible, or are flexible but have reached their maximum size. It also exerts some control over the alignment of items when they overflow the line.

```css
.flex-justify-content (@justify-content)
/*
Default:
  start
Variables:
  start, end, center, space-between, space-around
*/
```
  
### Flexbox Align Items
This defines the default behaviour for how flex items are laid out along the cross axis on the current line. Think of it as the justify-content version for the cross-axis (perpendicular to the main-axis).

```css
.flex-align-items (@align-items)
/*
Default:
  stretch
Variables:
  center, baseline, stretch, start, end
*/
```
  
### Flexbox Align Content
This aligns a flex container's lines within when there is extra space in the cross-axis, similar to how ```justify-content``` aligns individual items within the main-axis.

```css
.flex-align-content (@align-content)
/*
Default:
  start
Variables:
  start, end, center, space-between, space-around
*/
```

## Flexbox Bugs
There is a superb repo on github which references all FlexBox browser bugs - 
https://github.com/philipwalton/flexbugs
