## Challenge: Change the height

Can you add another slider to allow people to change the height of the hair image? You will need to follow the following steps:

1) Add the HTML code for the slider inside `<div id="sliders">`. If you are copying and pasting, don't forget to change the `id` of the slider too.

2) Between the `<script>` tags, add a variable that refers to the `id` of the slider you just created.

3) Add some more JavaScript code to say _when the height slider is changed, change the height of the hair image_. You will need to change the code in the two places marked with `???` below.

```JavaScript
???.oninput = function() {
  document.getElementById("hair-image").style.??? = this.value + "px";
}
```

Test whether your code works - can you move the slider to change the height of the hair image?
