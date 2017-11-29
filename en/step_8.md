## Change the position

Now that you can change the width and height of the hair, let's also make it possible to change the position so you can perch it perfectly on top of your head!

The process is almost the same as for the width and height of the hair, with one small difference. When you changed the width and height of the hair, you were modifying the `<img>` with the ID `hair-image`:

![Div or image](images/div-or-image.png)

To move the hair around, you will need to modify the `<div>` with the ID `hair` instead.

+ Add a top slider to your page - this will control how far from the top of the page the hair image is located.

```javascript
Top: <input type="range" min="1" max="300" value="50" id="hairtop">
```
+ Between the `<script>` and `</script>` tags, create a variable called `top_slider` to refer to the slider you just added:

```javascript
var top_slider = document.getElementById("hairtop");
```

+ Underneath this, but still within the `<script>` tags, add some code to change the distance from the top whenever the top slider's value is changed:

```javascript
top_slider.oninput = function() {
  document.getElementById("hair-image").style.top = this.value + "px";
}
```

+ Move the slider and you should see the hair image move closer or further from the top of the page.

+ Add a `left` slider in exactly the same way - repeat the same steps but replace `top` with `left` to allow your hair to be positioned at variable distances from the left of the page.
