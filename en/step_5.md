## Add the images

+ Open up the starter trinket [rpf.io/combover](http://rpf.io/combover){:target="_blank"}.

You will see some HTML code inside `index.html` and some CSS code inside `style.css`.

![Starter code](images/starter-code.png)

+ Click on the image icon near the top right-hand corner of the code area.

![Image icon](images/image-icon.png)

+ Click **Add image**, then **Upload**, then **Click to select files**. You will need a free Trinket account to be able to upload images.

+ Select the hair image you just made and the image of a face you've chosen.

Wait for the images to upload, then make sure that both are selected in green so that you can use them in this trinket.

![Selected in green](images/green-images.png)

Make a note of the file names of the images — in this example, we have `face.jpg` and `quiff.png`

I am using a photo of myself, so I know that I have permission to use it and that I am happy for it to be seen in public on the internet.

+ Go back to `index.html` and look at the code on lines 9 to 15.

![Image code](images/image-code.png)

+ Here is a good place to add the image license. You can add a comment in your code between `<!--` and `-->` to place the license text for your image:

```javascript
<div id="hair"> <!-- Hair image by Tim Lucas CC BY 3.0, via Wikimedia Commons -->
    <img src="" id="hair-image">
</div>
```

Where you see `src=""` in the code, you need to add the name of the picture you want to display between the quotation marks.

+ Add the file name of your face image between the quotation marks of the first image tag.

![Add the face image](images/original-image.png)

+ In exactly the same way, add the file name of the hair image inside the second image tag.

You should see both images appear in the area to the right of the code area. However, the hair might be floating around somewhere!

![See both images](images/both-images.png)
