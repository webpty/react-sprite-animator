# React Sprite Scaled Animator

Project forked from https://github.com/jcblw/react-sprite-animator

[![Build Status](https://travis-ci.org/webpty/react-sprite-scaled-animator.svg?branch=master)](https://travis-ci.org/webpty/react-sprite-scaled-animator)

A React component that animates through an image sprite while scaling to its parent container. 

- [Animated Heart Example](http://react-sprite-animator.surge.sh/) 

<img src='https://raw.githubusercontent.com/jcblw/react-sprite-animator/master/examples/padman-go.gif' width='120px' height='134px'>


### Install

    $ npm i react-sprite-scaled-animator -S

### Usage

```html
<SpriteAnimator
  sprite='/path-to/sprite.svg'
  width={100}
  height={100}
/>
```

### Props

- width **{number}** - width of clipped sprite (original, non-scaled dimensions)
- height **{number}** - height of clipped sprite (original, non-scaled dimensions)
- sprite **{string}** - path to sprite
- direction **{string}** - horizontal/vertical
- shouldAnimate **{bool}** - if the sprite should animate
- startFrame **{number}** - the frame to start animation
- fps **{number}** - the frame rate (frames per second) target
- stopLastFrame **{bool}** - stops animation from looping
- frame **{number}** - manually sets current frame
- framesToPlay **{number}** - manually sets number of frames to play


**Only required for two-dimensional sprites**

- frameCount **{number}** - the total frame count of the sprite
- wrapAfter **{number}** - the row or column count of the sprite (direction: "horizontal" -> columns, "vertical" -> rows)
