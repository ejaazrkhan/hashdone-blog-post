## Animated Card (CSS Animation)


![Animated Card](https://cdn.hashnode.com/res/hashnode/image/upload/v1658668443525/OAv1DQIoW.png)
Create an animated card in HTML & CSS

To change the styling of a card based on the element's hover state, focus state, or any of its descendants state, use the pseudo-class selectors `:hover` and `:focus-within`.

Using `overflow:hidden`, hide the extra content of the card and show it on hover.

## HTML Code
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Animated Card</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="background-image"></div>
    <div class="card">
        <img src="https://images.wallpaperscraft.com/image/single/honda_s2000_honda_car_322685_1280x720.jpg"/>
        <h3>Hover Me</h3>
        <div class="focus-content">
          <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Eveniet quia fugit labore dolores sint reiciendis perspiciatis<br/>
        </div>
    </div>
</body>
</html>
```
## CSS Code
```css
body{
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
}
.background-image {
    position: fixed;
    left: 0;
    right: 0;
    display: block;
    background-image: url(https://images.wallpaperscraft.com/image/single/honda_s2000_honda_car_322685_1280x720.jpg);
    -webkit-filter: blur(4px);
    -moz-filter: blur(4px);
    -o-filter: blur(4px);
    -ms-filter: blur(4px);
    filter: blur(4px);
    width: 100%;
    height: 100%;
    background-size: cover;
}
.card {
    width: 300px;
    height: 280px;
    padding: 0;
    box-shadow: 0 2px 4px 0 rgba(0,0,0,0.1);
    border-radius: 8px;
    box-sizing: border-box;
    overflow: hidden;
    background-color: #fff;
    z-index: 1;
  }
  
  .card * {
    transition: 0.3s ease all;
  }
  
  .card img {
    margin: 0;
    width: 300px;
    height: 224px;
    object-fit: cover;
    display: block;
  }
  
  .card h3 {
    margin: 0;
    padding: 12px 12px 48px;
    line-height: 32px;
    font-weight: 500;
    font-size: 20px;
  }
  
  .card .focus-content {
    display: block;
    padding: 8px 12px;
  }
  
  .card p {
    margin: 0;
    line-height: 1.5;
  }
  
  .card:hover img, .card:focus-within img {
    margin-top: -80px;
  }
  
  .card:hover h3, .card:focus-within h3 {
    padding: 8px 12px 0;
  }
```
## Output
![Animated Card Output](https://cdn.hashnode.com/res/hashnode/image/upload/v1658668445330/hfaD7ZL2C.png)
[Preview](https://animated-card-bay.vercel.app/)

Blog:- https://beginners-developer.blogspot.com