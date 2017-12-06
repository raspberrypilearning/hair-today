## Add a slider

Let's add a slider so that the user of your app can change the width of the hair to make it fit on the pictured person's head properly.

+ Click on line 18. which is inside the div labelled `sliders`.

![Slider div](images/div-slider.png)

+ Add the following code to creat a width slider on your page — it will control the width of the hair image so we can fit it to the head.

```javascript
Width: <input type="range" min="1" max="300" value="50" id="hairwidth">
```
You should see the slider appear below your picture.

![New slider](images/new-slider.png)

If you move the slider at the moment, nothing happens. You need to write some code to tell the page: "When this slider is moved, change the width of the hair."

+ Position your cursor between the `<script>` and `</script>` tags. This is where you can write **JavaScript** code.

+ Create a variable called `width_slider`, which refers to the slider you just added, like this:

```javascript
var width_slider = document.getElementById("hairwidth");
```

Notice that the `id` of the slider you just created was `hairwidth`, and now you're using this to select the slider with the help of `getElementById`.

+ Below this line, but still within the `<script>` tags, add the following code to change the width of the hair whenever the slider's value changes:

```javascript
// When I move the width slider...
width_slider.oninput = function() {
  // Change the width of the hair
  document.getElementById("hair-image").style.width = this.value + "px";
}
```

This code says _"When the `width_slider` is moved, select the `hair-image` and set its `style.width` to the value of the slider (`this.value+"px"`)"_. '//' is how you tell your JavaScript code that what follows is a comment.

+ Move the slider — as you drag it, you should see the hair image get bigger or smaller.

![Move the width slider](images/move-width.gif)
