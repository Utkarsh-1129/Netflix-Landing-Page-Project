# Responsive Netflix-Landing-Page-Project
Source Code for Responsive Netflix Landing Page using HTML and CSS: 

/****************************************************** HTML CODE *************************************************************************/

# HTML:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Netflix</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header class="header">
        <nav>
            <img src="logo.png" class="logo" alt="Netflix Logo">
            <div>
                <button class="language-btn">English <img src="down-icon.png" alt="Dropdown Icon"></button>
                <button>Sign In</button>
            </div>
        </nav>
        <div class="header-content">
            <h1>Unlimited movies, TV shows, and more.</h1>
            <h3>Watch anywhere. Cancel anytime.</h3>
            <p>Ready to watch? Enter your email to create or restart your membership.</p>
            <form class="email-signup">
                <input type="email" placeholder="Email address" required>
                <button type="submit">GET STARTED</button>
            </form>
        </div>
    </header>
    <div class="features">
        <div class="row">
            <div class="text-col">
                <h2>Enjoy on your TV.</h2>
                <p>Watch on Smart TVs, PlayStation, Xbox, Chromecast, Apple TV, Blu-ray players, and more.</p>
            </div>
            <div class="img-col">
                <img src="feature-1.png" alt="TV">
            </div>
        </div>
        <hr> <!-- Division between features -->
        <div class="row">
            <div class="img-col">
                <img src="feature-2.png" alt="TV">
            </div>
            <div class="text-col">
                <h2>Download your shows to watch offline</h2>
                <p>Save your favourites easily and always have something to watch.</p>
            </div>
        </div>
        <hr> <!-- Division between features -->
        <div class="row">
            <div class="text-col">
                <h2>Watch everywhere</h2>
                <p>Stream unlimited movies and TV shows on your phone, tablet, laptop, and TV.</p>
            </div>
            <div class="img-col">
                <img src="feature-3.png" alt="TV">
            </div>
        </div>
        <hr> <!-- Division between features -->
        <div class="row">
            <div class="img-col">
                <img src="feature-4.png" alt="TV">
            </div>
            <div class="text-col">
                <h2>Create profiles for kids</h2>
                <p>Send children on adventures with their favourite characters in a space made just for them—free with your membership.</p>
            </div>
        </div>
    </div>
    <hr>
    <div class="faq">
        <h2>Frequently Asked Questions</h2>
        <div class="accordion">
            <li>
                <input type="radio" name="accordion" id="first">
                <label for="first">What is Netflix?</label>
                <div class="content">
                    <p>Netflix is a streaming service that offers a wide variety of award-winning TV shows, movies, anime, documentaries, and more on thousands of internet-connected devices.</p>
                </div>
            </li>
            <li>
                <input type="radio" name="accordion" id="second">
                <label for="second">How much does Netflix cost?</label>
                <div class="content">
                    <p>Watch Netflix on your smartphone, tablet, Smart TV, laptop, or streaming device, all for one fixed monthly fee. Plans range from ₹ 199 to ₹ 799 a month. No extra costs, no contracts.</p>
                </div>
            </li>
            <li>
                <input type="radio" name="accordion" id="third">
                <label for="third">Where can I watch?</label>
                <div class="content">
                    <p>Watch anywhere, anytime, on an unlimited number of devices. Sign in with your Netflix account to watch instantly on the web at netflix.com from your personal computer or on any internet-connected device that offers the Netflix app, including smart TVs, smartphones, tablets, streaming media players and game consoles.</p>
                </div>
            </li>
            <li>
                <input type="radio" name="accordion" id="fourth">
                <label for="fourth">How do I cancel?</label>
                <div class="content">
                    <p>Netflix is flexible. There are no pesky contracts and no commitments. You can easily cancel your account online in two clicks. There are no cancellation fees – start or stop your account anytime.</p>
                </div>
            </li>
        </div>
        <small>Ready to watch? Enter your email to create or restart your membership.</small>
        <form class="email-signup">
            <input type="email" placeholder="Email address" required>
            <button type="submit">GET STARTED</button>
        </form>
    </div>
    <footer class="footer">
       <h2><p>Questions? Call 000-800-040-1843</p></h2>
       <div class="row">
        <div class="col">
            <a href="#">FAQs</a>
            <a href="#">Investor Relations</a>
            <a href="#">Privacy</a>
            <a href="#">Speed Test</a>
        </div>
        <div class="col">
            <a href="#">Help Center</a>
            <a href="#">Jobs</a>
            <a href="#">Cookie Preferences</a>
            <a href="#">Legal Notices</a>
        </div>
        <div class="col">
            <a href="#">Account</a>
            <a href="#">Ways to Watch</a>
            <a href="#">Corporate Information</a>
            <a href="#">Netflix Originals</a>
        </div>
        <div class="col">
            <a href="#">Media Center</a>
            <a href="#">Terms of Use</a>
            <a href="#">Contact Us</a>
            <a href="#">Speed Test</a>
        </div>
        <button class="language-btn">English <img src="down-icon.png" alt="Dropdown Icon"></button>
        <p class="copyright-txt">Netflix India Originals</p>
    </div>
    </footer>
</body>
</html>

/****************************************************** CSS CODE *************************************************************************/


# CSS:
* {
    margin: 0;
    padding: 0;
    font-family: 'Poppins', sans-serif;
    box-sizing: border-box;
}

body {
    background-color: black;
    color: #fff;
}

.header {
    width: 100%;
    height: 100vh;
    background-image: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)), url('header-image.png');
    background-position: center;
    background-size: cover;
    padding: 10px 8%;
    position: relative;
}

nav {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 10px 0;
}

.logo {
    width: 150px;
    cursor: pointer;
}

nav button {
    border: 0;
    outline: 0;
    background: red;
    color: #fff;
    padding: 7px 20px;
    font-size: 12px;
    border-radius: 4px;
    cursor: pointer;
    margin-left: 10px;
}

.language-btn {
    display: inline-flex;
    align-items: center;
    background: transparent;
    border: 1px solid #fff;
    padding: 7px 10px;
}

.header-content {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    text-align: center;
    color: #fff;
    max-width: 650px;
}

.header-content h1 {
    font-size: 60px;
    line-height: 70px;
    font-weight: 600;
}

.header-content h3 {
    font-size: 24px;
    margin-top: 20px;
}

.header-content p {
    font-size: 18px;
    margin: 20px 0;
}

.email-signup {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
}

.email-signup input[type="email"] {
    padding: 10px;
    font-size: 16px;
    border: 1px solid #ccc;
    border-radius: 4px 0 0 4px;
    outline: none;
    width: 70%;
    max-width: 400px;
}

.email-signup button {
    padding: 10px 20px;
    font-size: 16px;
    border: 0;
    border-radius: 0 4px 4px 0;
    cursor: pointer;
    background-color: red;
    color: #fff;
}

/************FEATURES***************/
.features {
    padding: 50px 12%;
    font-size: 100%;
}

.row {
    display: flex;
    width: 100%;
    align-items: center;
    flex-wrap: wrap;
    padding: 50px 0;
}

.text-col {
    flex-basis: 50%;
    margin-bottom: 20px;
}

.img-col {
    flex-basis: 50%;
    margin-bottom: 20px;

}

.img-col img {
    display: block;
    width: 90%;
    margin: auto;
}

.features h2 {
    font-size: 50px;
    font-weight: 600;
    margin-bottom: 20px;
}

.features p {
    font-size: 20px;
    line-height: 1.5;
}

/***********************FAQs********************/
.faq {
    padding: 10px 12%;
    font-size: 18px;
    text-align: center;
}

.faq h2 {
    font-weight: 500;
    font-size: 40px;
}

.accordion {
    margin: 60px auto;
    width: 100%;
    max-width: 750px;
}

.accordion li {
    list-style: none;
    width: 100%;
    padding: 5px;
}

.accordion li label {
    display: flex;
    align-items: center;
    padding: 20px;
    font-size: 18px;
    font-weight: 500;
    background: #303030;
    margin-bottom: 2px;
    cursor: pointer;
    position: relative;
}

label::after {
    content: '+';
    font-size: 34px;
    position: absolute;
    right: 20px;
    transition: transform 0.5s;
}

input[type="radio"] {
    display: none;
}

.accordion .content {
    background: #303030;
    text-align: left;
    padding: 0 20px;
    max-height: 0;
    overflow: hidden;
    transition: max-height 0.5s, padding 0.5s;
}

.accordion input[type="radio"]:checked + label + .content {
    max-height: 600px;
    padding: 30px 20px;
}

.accordion input[type="radio"]:checked + label::after {
    transform: rotate(135deg);
}

/*---------------------------FOOTER ------------------------*/

.footer {
    padding: 50px 15% 10px;
    border-top: 6px solid #333;
    text-align: center;
    color: #777;
}

.footer h2 {
    font-size: 18px;
    font-weight: 400;
    margin-bottom: 30px;
}

.footer .row {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
}

.footer .col {
    flex-basis: 25%;
    flex-grow: 1;
    max-width: bottom;
}

.footer .col a {
    display: block;
    text-decoration: none;
    color: #777;
    font-size: 14px;
    margin-bottom: 10px;
}

.footer .language-btn {
    color: #fff;
    padding: 10px 20px;
    border-radius: 3px;
}

.copyright-txt {
    font-size: 14px;
    margin-top: 20px;
    margin-bottom: 10px;
}

/******************Media Queries For**********************/
@media only screen and (max-width: 600px) {
    .logo {
        width: 100px;
    }

    nav button {
        padding: 5px 10px;
    }

    nav .language-btn {
        padding: 4px 8px;
    }

    .header-content h1 {
        position: unset;
        transform: none;
        padding-top: 150px;
    }

    .header-content {
        font-size: 30px;
    }

    .email-signup button {
        font-size: 12px;
        padding: 10px 15px;
    }

    .text-col, .img-col {
        flex-basis: 100%;
    }

    .features h2 {
        font-size: 30px;
    }

    .features p {
        font-size: 15px;
    }

    .row:nth-child(2), .row:nth-child(4) {
        flex-direction: column-reverse;
    }

    .features .row {
        padding: 10px 0;
    }

    .faq h2 {
        font-size: 20px;
    }

    .accordion .content {
        font-size: 14px;
    }

    .accordion li label {
        padding: 10px;
        font-size: 14px;
    }

    label::after {
        font-size: 22px;
    }
}

