## Challenge: change the height

Can you add another slider to allow people to change the height of the hair image? You will need to follow these steps:

+ Create another slider inside `<div id="sliders">` by copying and pasting the code for the width slider. Don't forget to change the label and the `id` of the new slider.

+ Between the `<script>` tags, add a variable that refers to the `id` of the slider you just created.

+ Add some more JavaScript code to say "When the height slider is moved, change the height of the hair image". You will need to change the code in the two places marked with `???` below. Look at the code you wrote earlier to help you.

```javascript
???.oninput = function() {
  document.getElementById("hair-image").style.??? = this.value + "px";
}
```

+ Test whether your code works. Can you move the slider to change the height of the hair image?
