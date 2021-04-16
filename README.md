# linkitz

A simple multi-purpose link website.

To create a new link, paste this code into a `file.html`. Change some links and titles to make it work.

```html
<!DOCTYPE html>
<html>
    <head>
        <!-- title -->
        <title>Gmail</title>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <!-- favicon -->
        <link id="favicon" rel="icon" href="../i/gmail.png"
        type="image/x-icon" />
        <!-- viewport and sizing -->
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <!-- redirect -->
        <meta http-equiv="refresh" content="5; URL=https://mail.google.com/mail/u/0/" />
        <style>
            .center {
                display: block;
                margin-left: auto;
                margin-right: auto;
            }
        </style>
    </head>
    <body>
        <img src="../i/gmail.png" style="display: none;">
        <img id="randomImage" style="height:100%;" class="center"/>
        <script>
            function getRandomImage() {
            var images = ['../i/random/motivation1.png', '../i/random/motivation2.png', '../i/random/motivation3.png', '../i/random/motivation4.png', '../i/random/motivation5.png', '../i/random/motivation6.png', '../i/random/motivation7.png', '../i/random/motivation8.png', '../i/random/motivation9.png', '../i/random/motivation10.png', '../i/random/motivation11.png', '../i/random/motivation12.png',];
            var image = images[Math.floor(Math.random()*images.length)];
            
            return image;
            }
            
            function displayRandomImage() {
            var htmlImage = document.getElementById("randomImage");
            htmlImage.src = getRandomImage();
            }
            displayRandomImage();
        </script>
    </body>
</html>
```