---
title: "Animated Forms: A New Way to Engage Users (CSS Animation)"
seoTitle: "Animated Forms: A New Way to Engage Users (CSS Animation)"
seoDescription: "Create animated forms in HTML & CSS to engage users & improve completion rates. Use relevant, simple, & non-distracting animations."
datePublished: Sun Aug 20 2023 16:31:38 GMT+0000 (Coordinated Universal Time)
cuid: clljo16gi000009jv2pjn1rze
slug: animated-forms-a-new-way-to-engage-users-css-animation
canonical: https://beginners-developer.blogspot.com/2023/08/animated-forms-new-way-to-engage-users.html
tags: css, html5, css-animation

---

## Create an animated Form in HTML & CSS

Animated forms are a new way to engage users and make them more likely to complete your forms. By using animation, you can add a sense of movement and excitement to your forms, making them more visually appealing and easier to use.

There are many different ways to animate your forms. You can use simple animations, such as moving shapes or text, or you can create more complex animations, such as characters or objects that interact with the user. The type of animation you choose will depend on the purpose of your form and the target audience.

For example, if you are creating a form for children, you might use a fun and playful animation to keep them engaged. If you are creating a form for a business website, you might use a more professional animation to create a sense of trust and credibility.

No matter what type of animation you choose, make sure it is relevant to the content of your form and that it is easy to follow. The goal of animation is to make your form more user-friendly and enjoyable, so don't overdo it.

Here are some of the benefits of using animated forms:

Increased engagement: Animated forms are more visually appealing than static forms, which can lead to increased engagement from users.

Improved completion rates: Animated forms can help to improve completion rates by making the form more user-friendly and enjoyable.

Better user experience: Animated forms can provide a better user experience by making the form more interactive and engaging.

Increased brand awareness: Animated forms can help to increase brand awareness by creating a more memorable and engaging user experience.

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Animated Form</title>

    <!-- link style.css file -->
    <link rel="stylesheet" href="style.css">

    <!-- Boostrap 5 CDN Links, you can find it on boostrap website -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.1/dist/css/bootstrap.min.css" rel="stylesheet"
        integrity="sha384-iYQeCzEYFbKjA/T2uDLTpkwGzCiq6soy8tYaI1GyVh/UjpbCx/TYkiZhlZB6+fzT" crossorigin="anonymous">
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.1/dist/js/bootstrap.bundle.min.js"
        integrity="sha384-u1OknCvxWvY5kfmNBILK2hRnQC3Pr17a+RTT6rIHI7NnikvbZlHgTPOOmMi466C8"
        crossorigin="anonymous"></script>
</head>

<body>
    <div class="main-div">
        <div class="card">
            <div class="border-animation"></div>
            <div class="card-body p-5 text-white">
                <h5 class="card-title mb-5">Login</h5>
                <div class="mb-3 input-div position-relative">
                    <input type="email" class="form-control input-class">
                    <label for="email" class="text-secondary small">Email</label>
                </div>
                <br>
                <div class="mb-3 input-div position-relative">
                    <input type="password" class="form-control input-class">
                    <label for="password" class="text-secondary small">Password</label>
                </div>
                <div class="form-check">
                    <input type="checkbox" class="form-check-input">
                    <label for="password" class="form-check-label">Remember me</label>
                </div>
                <button class="btn btn-primary float-end" type="submit">Submit</button>
            </div>
        </div>
    </div>
</body>

</html>
```

## Explanation

The code is for an HTML form that uses Bootstrap 5 to style it. The form has three input fields: an email field, a password field, and a checkbox for remembering the user's login information. The form also has a submit button. The code starts with the declaration, which tells the browser that the document is an HTML5 document. The tag specifies that the language of the document is English. The `<head>` section of the document contains the metadata for the document, such as the title, charset, and links to CSS and JavaScript files. The `<body>` section of the document contains the main content of the document. In this case, the main content is the form. The form is wrapped in a `<div class="main-div">` element. This element is used to give the form a certain width and margin. The form itself is a `<div class="card">` element. This element is used to give the form a card-like appearance. The form has a `<div class="border-animation">` element inside it. This element is used to create a border animation around the form. The form also has a `<div class="card-body p-5 text-white">` element inside it. This element is used to give the form a white background and some padding. The form has three input fields: an email field, a password field, and a checkbox for remembering the user's login information. These input fields are all wrapped in a `<div class="mb-3 input-div position-relative">` element. This element is used to give the input fields some margin and to position them relative to each other. The submit button is a `<button class="btn btn-primary float-end" type="submit">Submit</button>` element. This element is used to submit the form data to the server. The code also uses Bootstrap 5 CDN links to style the form. These links are used to import the Bootstrap CSS and JavaScript files into the document.

```css
body{
    background-image: url(https://images.wallpaperscraft.com/image/single/eclipse_moon_circle_138151_1600x900.jpg);
}
.main-div{
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
}
.main-div .card{
    background-color: transparent;
    overflow: hidden;
}
.main-div .card-body{
    z-index: 9;
    background-color: #000;
    width: 99.2%;
    margin: 0.8px auto;
    max-height: 360px;
}
.input-div label{
    position: absolute;
    top: 18%;
    left: 9px;
    transition: 0.5s;
}
.input-class:focus ~ label{
    top: -28px;
    left: 0;
    transition: 0.5s;
    color: #fff !important;
}
.input-class{
    z-index: 9;
}
.main-div .border-animation{
    position: absolute;
    width: 100%;
    height: 100%;
    content: "";
    border: 2px solid #fff;
    animation: spin 10s linear infinite;
}
@keyframes spin {
    100% {
        transform: rotate(360deg);
    }
}
```

## Explanation

The body element has a background-image property that is set to the URL of an image. This will set the background image of the body element to the image specified by the URL.

The main-div element has a display, justify-content, and align-items properties that are set to flex, center, and center respectively. This will make the main-div element a flex container with its children centered both horizontally and vertically.

The main-div .card element has a background-color property that is set to transparent. This will make the card element transparent, so that the background image of the body element can be seen through it.

The main-div .card-body element has a z-index property that is set to 9. This will make the card-body element the topmost element in the card element, so that it will be displayed above the other elements in the card.

The input-div label element has a position property that is set to absolute. This will make the label element positioned absolutely, so that it will be positioned relative to the parent element.

The input-class:focus ~ label selector will apply the following styles to the label element when the input element is focused:

The top property is set to -28px. The left property is set to 0. The color property is set to #fff. The input-class selector will apply the following styles to the input element:

The z-index property is set to 9. The main-div .border-animation element has a position, width, height, content, and border properties that are set to absolute, 100%, 100%, "", and 2px solid #fff respectively. This will create a border animation around the card-body element.

The animation property of the border-animation element is set to spin 10s linear infinite. This will make the border animation rotate 360 degrees every 10 seconds, and it will loop infinitely.

The @keyframes rule defines the animation steps for the spin animation. The 100% step will rotate the border 360 degrees.

![Image description](https://cdn.hashnode.com/res/hashnode/image/upload/v1692548947413/eaad2d22-fcb2-4353-b1af-31ae6ec5c1b3.png align="left")

[Preview](https://animated-login-form-alpha.vercel.app/)

Blog:- [https://beginners-developer.blogspot.com](https://beginners-developer.blogspot.com)