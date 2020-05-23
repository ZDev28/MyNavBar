# MyNavBar
***
### Welcome to my own **NavBar** tutorial!

I don't copy from anyone lines of code, without the jQuery cdn XD

###### Let's start!

First we gonna take the jQuery cdn, because we need it:

```html
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
```
Here is it:

Now we gonna **Setup** our html file:
```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">
    <title>My Own Navbar</title>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
    <link href="style.css" rel="stylesheet" type="text/css" />
  </head>
  <body>
    <button class="shownavbar"><i>NavBar</i></button>
    <br>
    <div id="div1" style="display: none;"><a href="#">Home</a></div>
    <div id="div2" style="display: none;"><a href="#">About</a></div>
    <div id="div3" style="display: none;"><a href="#">Contact</a></div>
    <div id="div4" style="display: none;"><button class="hide">Hide Navbar</button></div>
    <script src="script.js"></script>
    <script src="jquery.js"></script>
  </body>
</html>
```

**Cool!**

Now let's write some css now!
```css
*{
  margin: 0;
  padding: 0;
  box-direction: border-box;
  font-family: sans-serif;
}
.shownavbar{
  border-radius: 10px 10px;
  height: 25px;
  width: 100px;
}
.shownavbar i{
  color: red;
}
.shownavbar:hover i{
  background: yellow;
  color: red;
}
.shownavbar:hover{
  background: yellow;
}
#div1{
  background: green;
  text-decoration: none;
}
#div2{
  background: red;
  text-decoration: none;
}
#div3{
  background: yellow;
  text-decoration: none;
}
#div1, #div2, #div3{
  text-align: center;
}
.hide{
  border-radius: 10px 10px;
  height: 25px;
  width: 100px; 
}
```

So we styled the page..
### Now we gonna start to the **real** code, it is ~~javascript~~!

```js
$("document").ready(function(){
  $(".shownavbar").click(function(){
    $("#div1").fadeIn();
    $("#div2").fadeIn();
    $("#div3").fadeIn();
    $("#div4").fadeIn()
  });
  $(".hide").click(function(){
    $("#div1").fadeOut();
    $("#div2").fadeOut();
    $("#div3").fadeOut();
    $("#div4").fadeOut();
  });
});
```
So we only used the `fadeIn()` and `fadeOut()` functions, to make it ~~SCARY~~ beautiful!
now we gonna [try it out!](https://navbar--zuhdi28.repl.co/)

My repl.it repl for this:
https://repl.it/@Zuhdi28/NavBar
My repl.it post for this:
https://repl.it/talk/share/My-Own-Navbar/38914

### I hope you had fun!!
