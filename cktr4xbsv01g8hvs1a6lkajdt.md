## Testimonial Section in HTML and CSS

Learn how to create testimonial section using HTML, CSS and Bootstrap

## HTML Code
```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Testimonial</title>
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css">
    <link rel="stylesheet" href="style.css" >
</head>

<body>
    <section class="testimonial-section py-3" id="testimonial">
        <div class="container">
            <h2 class="align-center pb-3 text-center">
                What Our Clients Say
            </h2>

            <div class="col-lg-10 testimonials-container">
                <div class="testimonials-item">
                    <div class="user row">
                        <div class="col-lg-3 col-md-4">
                            <div class="user_image">
                                <img src="images/user1.jpg" alt="" title="">
                            </div>
                        </div>
                        <div class="d-flex flex-column justify-content-center testimonials-caption pl-0 col-lg-9 col-md-8">
                            <div class="user_text">
                                <p class="mbr-text mbr-fonts-style mbr-lighter display-7">
                                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Nisi, saepe iusto blanditiis, architecto magni dolores perspiciatis expedita ut voluptates soluta neque voluptas eveniet
                                </p>
                            </div>
                            <div class="user_name mbr-bold mbr-fonts-style pt-3 font-weight-bold">
                                John Doe
                            </div>

                        </div>
                    </div>
                </div>
                <div class="testimonials-item">
                    <div class="user row">
                        <div class="col-lg-3 col-md-4">
                            <div class="user_image">
                                <img src="images/user2.jpg">
                            </div>
                        </div>
                        <div class="d-flex flex-column justify-content-center testimonials-caption pr-0 col-lg-9 col-md-8">
                            <div class="user_text">
                                <p class="mbr-text mbr-fonts-style mbr-lighter display-7">
                                    Lorem, ipsum dolor sit amet consectetur adipisicing elit. Mollitia sed molestiae ipsam repellat nemo architecto itaque similique suscipit beatae consequuntur.
                                </p>
                            </div>
                            <div class="user_name mbr-bold mbr-fonts-style pt-3 font-weight-bold">
                                John Doe
                            </div>

                        </div>
                    </div>
                </div>
                <div class="testimonials-item">
                    <div class="user row">
                        <div class="col-lg-3 col-md-4">
                            <div class="user_image">
                                <img src="images/user3.jpg" alt="" title="">
                            </div>
                        </div>
                        <div class="d-flex flex-column justify-content-center testimonials-caption pl-0 col-lg-9 col-md-8">
                            <div class="user_text">
                                <p class="mbr-text mbr-fonts-style mbr-lighter display-7">
                                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Pariatur deleniti eaque architecto, sed placeat, quo sunt delectus perferendis dolores ad quasi facere.
                                </p>
                            </div>
                            <div class="user_name mbr-bold mbr-fonts-style pt-3 font-weight-bold">
                                John Doe
                            </div>

                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</body>

</html>
```
## CSS Code
```css
.testimonial-section{
    background-image: url(images/bg.jpg), linear-gradient(rgb(255 253 253 / 90%),rgb(253 253 253 / 50%));
    background-blend-mode: overlay;
}
.testimonial-section h2,
.testimonial-section h3,
.testimonial-section p,
.testimonial-section .mbr-text {
    letter-spacing: normal;
}
.testimonial-section .underline .line {
    width: 2rem;
    height: 1px;
    background: #ffffff;
    display: inline-block;
}
.testimonial-section .testimonials-container {
    margin: 0 auto;
}
.testimonial-section .testimonials-container .testimonials-item:nth-child(2n) .user.row {
    flex-direction: row-reverse;
    -webkit-flex-direction: row-reverse;
}
.testimonials-container .testimonials-item:nth-child(2n) .user.row .testimonials-caption {
    text-align: right;
}
.testimonial-section .testimonials-container .testimonials-item .user.row {
    margin: 0;
}
.testimonial-section .testimonials-container .testimonials-item .user .user_image {
    width: 150px;
    height: 150px;
    overflow: hidden;
    margin: 2rem auto;
    border-radius: 50%;
}
.testimonial-section .testimonials-container .testimonials-item .user .user_image img {
    width: 100%;
    min-width: 100%;
    min-height: 100%;
}
@media (max-width: 260px) {
    .testimonial-section .user_image {
      width: 100% !important;
      height: auto !important;
    }
}
@media (max-width: 767px) {
    .testimonial-section, .testimonials-container .testimonials-item:nth-child(2n) .user.row .testimonials-caption{
        text-align: center;
    }
    .testimonial-section .testimonials-caption {
      padding: 0 2rem 2rem 2rem !important;
    }
    .testimonial-section .testimonials-caption .user_name {
        text-align: center;
        padding-top: 0px !important;
    }
}
```

## Video
[![Testimonial Section in HTML and CSS](https://cdn.hashnode.com/res/hashnode/image/upload/v1632050826501/Cdt0VUd4-.jpeg)](http://www.youtube.com/watch?v=JsW3-uaNGPw)

My Blog:- https://beginners-developer.blogspot.com