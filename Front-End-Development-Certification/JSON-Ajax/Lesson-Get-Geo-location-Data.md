# Author
![@Rafase282](https://avatars0.githubusercontent.com/Rafase282?&s=128)

Created by Rafase282

[Github](https://github.com/Rafase282) | [FreeCodeCamp](http://www.freecodecamp.com/rafase282) | [CodePen](http://codepen.io/Rafase282/) | [LinkedIn](https://www.linkedin.com/in/rafase282) | [Blog/Site](https://rafase282.wordpress.com/) | [E-Mail](mailto:rafase282@gmail.com)

## Get Geo-location Data
Every browser has a built in navigator that can give us this information.

The navigator will get our user's current longitude and latitude.

You will see a prompt to allow or block this site from knowing your current location. The challenge can be completed either way, as long as the code is correct.

By selecting allow you will see the text on the output phone change to your latitude and longitude

Here's some code that does this:

```js
if (navigator.geolocation) {

  navigator.geolocation.getCurrentPosition(function(position) {

    $("#data").html("latitude: " + position.coords.latitude + "<br>longitude: " + position.coords.longitude);

  });

}
```
