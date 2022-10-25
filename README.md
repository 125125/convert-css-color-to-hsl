# **Simple color to hsl extension**

Converts Color Names, RGB, and HEX to HSL.

## Dependencies :

This extension relies on **vakhariaheet's** https://github.com/vakhariaheet/color-convertor

# **HSL Color Guide**

### What is hsl color?
hsl colors is hue + saturation + lightness

### What makes hsl colors better than hex/rgb/color names?
hsl colors is better because they are easier to modify
Here is an example
```css
.box {
  color:hsl(60 100% 50%)
}
```
So in the example above i use hue 57 degrees on the color wheel (Yellow Color) and 100% saturation and 50% lightness. If you increase lightness, the color will get lighter. So 100% lightness is white and 0% lightness is black.
So here is an example on how to make the color slightly lighter
```css
.box {
  color:hsl(60 100% 60%)
}
```
as you can see i just changed the last value to 60% and the color is now lighter. and the more you reduce the saturation the more "gray" the color will become.

hsl colors is actually written as the example below
```css
.box {
  color:hsl(60deg, 100%, 50%)
}
```
However, the comma is not needed and the deg is also not needed. But i include it as an example anyway. Because you can still write it this way, this is still valid css.

but if you do wish to use the **Comma Method** with an alpha channel you can write it like the example below
```css
.box {
  color:hsl(60, 100%, 50%, .5)
}
```

and without comma you write it like this
```css
.box {
  color:hsl(60 100% 50% / .5)
}
```
and this is also how this converter will convert your colors.
You can also use hsla which means Hue + Saturation + Lightness + Alpha. But hsla is not needed since you can use an alpha channel with just hsl

### Here is a few examples of other colors in hsl
```css
.box {
  color:hsl(0 0% 0%); /* Black Color */
  color:hsl(0 0% 100%); /* White Color */
  color:hsl(0 100% 50%); /* Red Color */
  color:hsl(39 100% 50%); /* Orange Color */
  color:hsl(60 100% 50%); /* Yellow Color */
  color:hsl(120 100% 50%); /* Green Color */
  color:hsl(240 100% 50%); /* Blue Color */
  color:hsl(300 100% 50%); /* Purple Color */
  color:hsl(350 100% 50%); /* Pink Color */
}
```
