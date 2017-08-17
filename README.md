# jQuery Animations

## jQuery Animation Overview

- jQuery packs in two kinds of animations: fading and vertical sliding.
- These allow you to create simple animations while still enjoying all of the benefits of using JS such as action chaining.
- jQuery animations using DOM manipulation of the `style` attribute to create animations.
- As a result they should be used sparingly for performance reasons.

## Fades

##### Fade In:

```javascript
$("my-selector").fadeIn();
```

##### Fade Out:

```javascript
$("my-selector").fadeOut();
```

##### Fade Toggle (Back and Forth):

```javascript
$("my-selector").fadeToggle();
```

## Slides

##### Slide Down (Show the Element):

```javascript
$("my-selector").slideDown();
```

##### Slide Up (Hide the Element):

```javascript
$("my-selector").slideUp();
```

##### Slide Toggle (Back and Forth):

```javascript
$("my-selector").slideToggle();
```

## Custom Animations

- If none of the built-in animations suit you, jQuery also gives you a way to create your own animations.
- This function will dynamically alter the `style` attribute in the HTML document for each property you specify:

```javascript
$("my-selector").animate({
	"margin-top":"200px",
	"margin-left":"+=200px"
}, 600, "swing", function() {
	console.log("I just finished!");
});
```

## Animation Exercise: Gettysburg Address

- We will be working on a given front end to enable a few dynamic animations on the page.
- Please refer to the project linked in Slack.