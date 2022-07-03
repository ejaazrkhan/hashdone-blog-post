## Social media icons HTML and CSS

Create Social media icons with HTML and CSS.

## HTML Code 
```html
<!DOCTYPE html>
<html>
<head>
    <title>Social Icons Effects</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.14.0/css/all.min.css" />
    <link href="https://fonts.googleapis.com/css2?family=Montserrat&display=swap" rel="stylesheet">
    <link rel="stylesheet" type="text/css" href="style.css">
</head>
<body>
    <div class="container">
        <div class="wrapper">

            <a href="#" class="icon-container icon-container-facebook">
                <i class="fab fa-facebook-f"></i>
                <div class="icon-text icon-text-facebook">Facebook</div>
            </a>

            <a href="#" class="icon-container icon-container-twitter">
                <i class="fab fa-twitter"></i>
                <div class="icon-text icon-text-twitter">Twitter</div>
            </a>

            <a href="#" class="icon-container icon-container-github">
                <i class="fab fa-github"></i>
                <div class="icon-text icon-text-github">Github</div>
            </a>

            <a href="#" class="icon-container icon-container-instagram">
                <i class="fab fa-instagram"></i>
                <div class="icon-text icon-text-instagram">Instagram</div>
            </a>

        </div>
    </div>
</body>
</html>
```

## CSS Code
```css
*{
    font-family: 'Montserrat', sans-serif;
}
body{
    background-image: url(bg.jpg);
    background-size: cover;
}
.container{
    height: 100vh;
}
.wrapper {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
}
.icon-container {
    position: relative;
    width: 80px;
    height: 80px;
    display: flex;
    -webkit-box-align: center;
    align-items: center;
    -webkit-box-pack: center;
    text-decoration: none;
    justify-content: center;
    border-radius: 50%;
    -webkit-transition: all 0.15s ease;
    transition: all 0.15s ease;
    margin-left: 20px;
}
.icon-container i{
    font-size: 25px;
}
.icon-container-facebook {
    background: #3b5998;
    color: #fff;
}
.icon-container-twitter {
    background: #1DA1F2;
    color: #fff;
}
.icon-container-github {
    background: #000;
    color: #fff;
}
.icon-container-instagram {
    background: linear-gradient(45deg, #405de6, #5851db, #833ab4, #c13584, #e1306c, #fd1d1d);
    color: #fff;
}
.icon-text{
    position: absolute;
    top: 0;
    left: 50%;
    padding: 0.8rem 1rem;
    border-radius: 40px;
    font-size: 0.8rem;
    font-weight: bold;
    opacity: 0;
    pointer-events: none;
    text-transform: uppercase;
    -webkit-transform: translate(-50%, -100%);
    transform: translate(-50%, -100%);
    -webkit-transition: all 0.3s ease;
    transition: all 0.3s ease;
    z-index: 1;
}
.icon-text:after {
    display: block;
    position: absolute;
    bottom: 1px;
    left: 50%;
    width: 0;
    height: 0;
    content: "";
    border: solid;
    border-width: 10px 10px 0 10px;
    border-color: transparent;
    -webkit-transform: translate(-50%, 100%);
    transform: translate(-50%, 100%);
}
.icon-container:hover .icon-text {
    visibility: visible;
    opacity: 1;
    -webkit-transform: translate(-50%, -150%);
    transform: translate(-50%, -150%);
}
.icon-text-facebook {
    background: #3b5998;
    color: #fff;
}
.icon-text-facebook:after{
    border-top-color: #3b5998;
}

.icon-text-twitter {
    background: #1DA1F2;
    color: #fff;
}
.icon-text-twitter:after{
    border-top-color: #1DA1F2;
}

.icon-text-github {
    background: #000;
    color: #fff;
}
.icon-text-github:after{
    border-top-color: #000;
}

.icon-text-instagram {
    background: linear-gradient(45deg, #405de6, #5851db, #833ab4, #c13584, #e1306c, #fd1d1d);
    color: #fff;
}
.icon-text-instagram:after{
    border-top-color: #8739B0;
}
```
### Output
<iframe height="300" style="width: 100%;" scrolling="no" title="Social media icons HTML and CSS" src="https://codepen.io/ejaazkhan/embed/KKqmxyW?default-tab=html%2Cresult" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href="https://codepen.io/ejaazkhan/pen/KKqmxyW">
  Social media icons HTML and CSS</a> by Ejaaz Khan (<a href="https://codepen.io/ejaazkhan">@ejaazkhan</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>

My Blog:- https://beginners-developer.blogspot.com