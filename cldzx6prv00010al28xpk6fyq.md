---
title: "The Art of CSS Positioning"
datePublished: Sat Feb 11 2023 12:14:33 GMT+0000 (Coordinated Universal Time)
cuid: cldzx6prv00010al28xpk6fyq
slug: the-art-of-css-positioning
tags: css, web-development, webdev

---

So one day, sitting in a dark attic, there was a developer, named "Hakon Wium Lie", if you could pronounce it tell me how because I found it harder than centring a div.

CSS was created with the dedication and passion of creating something for developers that is more difficult to pronounce than Elon Musk's son's name.

There are a lot of weird things about CSS. But one thing we all agree on is that positioning is the weirdest.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1676100825285/d204f80a-8db3-4d97-9a25-af56ed58249d.png align="center")

I've been CSS's boyfriend for a few months now, and I know how to avoid her tantrums. And this is my diary, where I try to tell you on about how to avoid them as well.

One thing I tell every developer who says "I wanna love CSS" *<s>apart from "I'm gonna end your life, CSS is my girl!"</s>* is "you gotta learn how to divide and conquer"

So let's divide and conquer this CSS mystery!

![](https://i.imgflip.com/7as11k.jpg align="left")

I like to divide it into two parts:

* Native CSS Layouts
    
* The `position` property!
    

## Native CSS Layouts

So there are several native CSS layouts,

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1676101473684/c8666139-064f-4cd3-b371-89d1d1f0a231.png align="center")

I mean who needs these many layouts and half of them are trash:-

* Block just means that the element has 100% width
    
* Inline means that it only has the width of the element (Note: Margins don't work here)
    
* `None` means to hide the damn thing
    
* Contents mean to show the damn thing
    
* Inline-block is breeding b/w block and inline, you have margin, but no 100% width
    
* I still ain't know what `flow` is after working with CSS for years, so it is useless, just forget it.
    

Now let's come to flex, aka 💪 and grid.

### Flex

Flex just means that the element is the stack of coins you will be getting after writing this CSS, with each child element representing one penny.

You can stack it horizontally or vertically, and you can also specify how much space there should be between the elements.

Here is one image I stole from [css tricks](https://css-tricks.com) :

![](https://css-tricks.com/wp-content/uploads/2018/10/01-container.svg align="left")

The container is the flexbox, and the yellow thing is the items. That is flexbox. I say that flexbox isn't the most confusing part, so I'll leave the GOATs at css-tricks to explain it: [A Complete Guide to Flexbox | CSS-Tricks - CSS-Tricks](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

### Grid

Grid is like a flexbox, but this time it's a suitcase of cash and not just a stack.

\==&gt;&gt; Grid is flex but 2 dimensional

![Example of grid-column-gap and grid-row-gap](https://css-tricks.com/wp-content/uploads/2018/11/dddgrid-gap.svg align="left")

Yeah, I managed to steal another image, those people must be like: wtf 😂

Anyways, Grid is also not such a big problem with position, so here's a link: [A Complete Guide to CSS Grid | CSS-Tricks - CSS-Tricks](https://css-tricks.com/snippets/css/complete-guide-grid/)

### `position`

This one is actually sensible, it has 5 possible values:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1676106666413/69a78c86-dae6-4f91-ba43-64081da49042.png align="center")

### Static

This is the default, so you'll like never be setting this explicitly

### Relative

This will allow you to use `top` `bottom` `left` and `right` but respective to where the position of the element would have been if the position was the default. So if I set `top: 5px`; it is 5px off from the top position where it would have been.

### Absolute

It will just render your element on the axis. The axis will be the document by default, but if the element's parent has relative positioning, the axis is relative to the space inside the element.

So if an element has top: 4px, then the element will be 4px away from the top on the screen.

### Fixed

Fixed means it will stay there if you scroll. If an object has absolute positioning, it will go away once you scroll, but fixed will keep it at that position.

So fixed is absolute but fixed

### Sticky

So what you might have noticed is that with absolute and fixed positioning the element with overflows the element that is statically rendered. To save it from happening, sticky elements switch between static and fixed when scrolled.

This will not come in handy unless you are making a navbar, so I'll not detail it much.