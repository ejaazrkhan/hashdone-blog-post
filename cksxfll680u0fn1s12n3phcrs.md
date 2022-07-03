## Button Hover Effect in HTML and CSS (CSS Animation)

Simple Button hover Effect using HTML and CSS
### HTML Code:
```
<!DOCTYPE html>
<html>
<head>
    <title></title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins&display=swap" rel="stylesheet">
    <link href="style.css" rel="stylesheet">
</head>
<body>
    <div class="main-content">
        <div class="button-main">
            <button class="button"> Hover me</button>
        </div>
    </div>
</body>
</html>
```
### CSS
```
*{
    margin: 0;
    padding: 0;
    font-family: 'Poppins', sans-serif;
}
body{
    background-image: url('bg.jpg');
}
.main-content{
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
}
.button-main{
    position: relative;
}
.button{
    padding: 20px 70px;
    background-color: #e15f41;
    color: #fff;
    font-size: 16px;
    cursor: pointer;
}
.button:focus{
    outline: none;
}
.button:hover{
    background-color: #000;
}
.button:before, .button:after{
    -webkit-transition: all 0.25s;
    transition: all 0.25s;
    border-style: solid;
    border-width: 0;
    content: "";
    height: 24px;
    position: absolute;
    width: 24px;
    border-color: #000;
}
.button:before{
    border-left-width: 2px;
    border-top-width: 2px;
    left: -5px;
    top: -6px;
}
.button:after{
    border-bottom-width: 2px;
    border-right-width: 2px;
    bottom: -5px;
    right: -6px;
}
.button:hover:before, .button:hover:after{
    height: 100%;
    width: 100%;
}
```
Output:
![Button Hover Effect Output](https://cdn.hashnode.com/res/hashnode/image/upload/v1630254768525/Eo1X53Wpx.gif)Preview: https://button-hover-effects.vercel.app/
My Blog:- https://beginners-developer.blogspot.com/
