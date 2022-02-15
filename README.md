# new-repository-
@import url('https://fonts.googleapis.com/css2?family=Exo+2:wght@300;400&family=Open+Sans:ital,wght@0,300;0,400;0,600;0,700;0,800;1,300;1,400;1,600;1,700;1,800&display=swap');

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {

    height: 100vh;
    display: flex;
    justify-content: center;
    background: #000000;
}

html {
    font-family: 'Open Sans', sans-serif;
    font-weight: bold;
    scroll-behavior: smooth;
    overflow-x: hidden
}

section {
    position: absolute;
    background: #ffffffff;
    width: 1080px;
    height: auto;
}

#top {
    padding: 5% 10% 5% 10%;
    background: rgba(0, 0, 0, 0.658);
    z-index: 2;
    margin-top: 150px;
    height: 350px;
    align-content: center;
}

#top h2 {
    font-weight: bolder;
    color: #ff0062;
}

#top p {
    font-weight: bold;
    text-align: justify;
    color: #ffff;
    margin-top: 10px;
}

.slide-btn {
    background-image: linear-gradient(to bottom right, red, yellow);
    border: none;
    color: white;
    text-align: center;
    text-decoration: none;
    font-size: 15px;
    border-radius: 5px;
    width: 100px;
    height: 35px;
}

.slide-btn:hover {
    opacity: 0.6;
}

span {
    font-weight: 900;
}

/* CSS for Navbar */
#nav {
    width: 1080px;
    height: 84px;
}

.navbar {
    position: fixed;
    display: flex;
    overflow: hidden;
    justify-content: center;
    align-items: center;
    background-color: rgba(0, 0, 0, 0.8);
    z-index: 999;
    width: 1080px;
}

.nav-list {
    display: flex;
    justify-content: center;
    align-items: center;
    color: black;
}

.nav-list li {
    list-style: none;
    padding: 25px 10px;
}

.nav-list li a {
    text-decoration: none;
    color: rgb(255, 255, 255);
}

#brand {
    padding-right: 60px;
    font-size: 25px;
    font-weight: bold;
}

.nav-list li a:hover {
    text-decoration: none;
    color: rgb(255, 174, 0);
}

/* CSS for Carousel */
.carousel {
    margin-top: 83px;
    width: 1080px;
    height: 500px;
    overflow: hidden;
}

.frames {
    width: 500%;
    height: 500px;
    display: flex;
}

.frames input {
    display: none;
}

.frame {
    width: 20%;
    transition: 2s;
}

.frame img {
    width: 1080px;
    height: 500px;
}

/* For Manual Carousel Control */
.manual-control {
    position: absolute;
    width: 1080px;
    margin-top: -40px;
    display: flex;
    justify-content: center;
    visibility: visible;
}

.manual-control label {
    border: 1px solid #ffffff;
    padding: 5px;
    border-radius: 50%;
    cursor: pointer;
    transition: 1s;
}

.manual-control label:not(:last-child) {
    margin-right: 5px;
}

.manual-control label:hover {
    background: rgba(255, 255, 255, 0.6);
}


#radio1:checked~.first {
    margin-left: 0;
}

#radio2:checked~.first {
    margin-left: -20%;
}

#radio3:checked~.first {
    margin-left: -40%;
}

#radio4:checked~.first {
    margin-left: -60%;
}


/* For Automatic Carousel Control */
.auto-control {
    position: absolute;
    display: flex;
    width: 1080px;
    justify-content: center;
    margin-top: 460px;
}

.auto-control div {
    border: 1px solid #ffffff;
    padding: 5px;
    border-radius: 10px;
    transition: 1s;
}

.auto-control div:not(:last-child) {
    margin-right: 5px;
}

#radio1:checked~.auto-control .auto-btn1 {
    background: #ffffff;
}

#radio2:checked~.auto-control .auto-btn2 {
    background: #ffffff;
}

#radio3:checked~.auto-control .auto-btn3 {
    background: #ffffff;
}

#radio4:checked~.auto-control .auto-btn4 {
    background: #ffffff;
}

.sections {
    margin-top: 10px;
    margin-bottom: 30px;
    text-align: center;
    font-size: 260%;
}

#welcome {
    margin-top: 585px;
    padding-top: 110px;
    height: 1045px;
}

#projects {
    margin-top: 1630px;
    padding-top: 110px;
    height: 560px;
}


/* Welcome Section */
.row {
    width: 100%;
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
}

.image {
    background: #000000;
    position: relative;
    flex: 1;
    max-width: 460px;
    height: 300px;
    margin: 5px;
    overflow: hidden;
}

.image img {
    opacity: 0.8;
    position: relative;
    vertical-align: top;
    transition: 0.6s;
    transition-property: opacity;
    width: 100%;
    height: 100%;
}

.image:hover img {
    opacity: .2;
}

.image .details {
    position: absolute;
    top: 0;
    right: 0;
    color: #ffffff;
    width: 100%;
    height: 100%;
}

.image .details h2 {
    padding-left: 30px;
    padding-right: 30px;
    text-align: center;
    font-size: 35px;
    text-transform: uppercase;
    font-weight: 300;
    margin-top: 100px;
    transition: 0.4s;
    transition-property: transform;
}

.image .details h2 span {
    font-weight: 900;
}

.image:hover .details h2 {
    transform: translateY(-80px);
}

.image .details p {
    margin: 30px 30px 0 30px;
    font-size: 18px;
    font-weight: 600;
    text-align: center;
    opacity: 0;
    transition: 0.6s;
    transition-property: opacity, transform;
}

.image:hover .details p {
    opacity: 1;
    transform: translateY(-100px);
}

.more {
    position: absolute;
    background: rgba(255, 255, 255, 0.8);
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 15px;
    bottom: -60px;
    transition: 0.6s;
    transition-property: bottom;
}

.image:hover .more {
    bottom: 0;
}

.more .read-more {
    color: #000;
    text-decoration: none;
    font-size: 20px;
    font-weight: 500;
    text-transform: uppercase;
}

.more .read-more span {
    font-weight: 900;
}


/* Project Section */
.project-cards {
    width: 100%;
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
}

.image-p {
    background: #000000;
    position: relative;
    flex: 1;
    max-width: 216px;
    height: 320px;
    margin: 5px;
    overflow: hidden;
}

.image-p img {
    opacity: 0.8;
    position: relative;
    vertical-align: top;
    transition: 0.6s;
    transition-property: opacity;
    width: 100%;
    height: 100%;
}

.image-p:hover img {
    opacity: .3;
}

.image-p .details {
    position: absolute;
    top: 0;
    right: 0;
    color: #ffffff;
    width: 100%;
    height: 100%;
}

.image-p .details h2 {
    padding: 0px 15px 0px 15px;
    text-align: center;
    font-size: 35px;
    text-transform: uppercase;
    font-weight: 300;
    margin-top: 165px;
    transition: 0.4s;
    transition-property: transform;
}

.image-p .details h2 span {
    font-weight: 900;
}

.image-p:hover .details h2 {
    transform: translateY(-145px);
}

.image-p .details p {
    margin: 30px 30px 0 30px;
    font-size: 18px;
    font-weight: 600;
    text-align: center;
    opacity: 0;
    transition: 0.6s;
    transition-property: opacity, transform;
}

.image-p:hover .details p {
    opacity: 1;
    transform: translateY(-165px);
}

.more {
    position: absolute;
    background: rgba(255, 255, 255, 0.8);
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 15px;
    bottom: -60px;
    transition: 0.6s;
    transition-property: bottom;
}

.image-p:hover .more {
    bottom: 0;
}

.more .learn-more {
    color: #000;
    text-decoration: none;
    font-size: 20px;
    font-weight: 500;
    text-transform: uppercase;
}

.more .read-more span {
    font-weight: 900;
}

/* Pricing Secton */
#pricing {
    margin-top: 2190px;
    padding: 110px;
}

.columns {
    float: left;
    width: 33.3%;
    padding: 8px;
}

.price {
    list-style-type: none;
    border: 1px solid #eee;
    margin: 0;
    padding: 0;
    -webkit-transition: 0.3s;
    transition: 0.3s;
}

.price:hover {
    box-shadow: 0 8px 12px 0 rgba(0, 0, 0, 0.2);
}

.price .header {
    background-color: #111;
    color: white;
    font-size: 25px;
}

.price li {
    border-bottom: 1px solid #eee;
    padding: 10px;
    text-align: center;
}

.price .grey {
    background-color: #eee;
    font-size: 20px;
}

.button {
    background-color: #ff0062;
    border: none;
    color: white;
    padding: 5px 15px;
    text-align: center;
    text-decoration: none;
    font-size: 15px;
    border-radius: 5px;
}

.button:hover {
    background: #04AA6D;
}

/* Video Projects */
#video-projects {
    margin-top: 2800px;
    padding: 30px 30px 60px 30px;
    color: #fff;
    background: #944da0;
}

.video-column {
    float: left;
    width: 50%;
    padding: 5px;
}

.video {
    width: 100%;
}

.video:hover {
    box-shadow: 0 8px 12px 0 rgba(0, 0, 0, 0.2);
    border-radius: 5px;
}

/* Team */
#team {
    margin-top: 3350px;
    padding: 100px 60px 30px 60px;
}

.team-column {
    float: left;
    width: 33.3%;
    padding: 8px;
    text-align: -webkit-center;
}

.team-column img {
    border-radius: 50%;
    width: 69%;
}

.team-column .details {
    width: 100%;
    height: 100%;
    padding: 15px 10px 15px 10px;
}

.team-column .details h2 {
    font-weight: 300;
    text-transform: uppercase;
}

.team-column .details h1 {
    padding: 0px 30px 0px 30px;
    text-align: center;
    font-size: 15px;
    font-weight: 400;
}

.team-column .details h1 span {
    font-weight: 800;
}

.imageBox {
    position: relative;
    float: left;
    width: 100%;
}

.imageBox .imageInn img {
    border-radius: 50%;
    width: 69%;
    transition: 0.5s;
}

.imageBox .hoverImg {
    position: absolute;
    left: 0;
    top: 0;
    opacity: 0;
    width: 100%;
    transition: 0.5s;
}

.imageBox:hover .hoverImg {
    opacity: 1;
}

.imageBox:hover .imageInn img {
    box-shadow: 0px 0px 10px rgb(0, 0, 0);
}

/* Life in Zippy */
#life-in-zippy {
    width: 1080px;
    margin-top: 4170px;
    padding: 110px;
    background: rgb(172, 172, 172);
}

/* Position the image container (needed to position the left and right arrows) */
.gallery {
    position: relative;
}

.gallery .work-life img {
    vertical-align: middle;
}

/* Hide the images by default */
.work-life {
    display: none;
}

.work-life img {
    width: 100%;
    height: 100%;
}

/* Add a pointer when hovering over the thumbnail images */
.cursor {
    cursor: pointer;
}

/* Next & previous buttons */
.prev,
.next {
    cursor: pointer;
    position: absolute;
    top: 40%;
    width: auto;
    padding: 16px;
    margin-top: -50px;
    color: white;
    font-weight: bold;
    font-size: 20px;
    border-radius: 0 3px 3px 0;
    user-select: none;
    -webkit-user-select: none;
}

/* Position the "next button" to the right */
.next {
    right: 0;
    border-radius: 3px 0 0 3px;
}

/* On hover, add a black background color with a little bit see-through */
.prev:hover,
.next:hover {
    background-color: rgba(0, 0, 0, 0.8);
}

.row {
    height: 100px;
}

.row:after {
    content: "";
    display: table;
    clear: both;
}

/* Six columns side by side */
.column {
    float: left;
    width: 16.66%;
    height: 100px;
}

.column img {
    width: 100%;
    height: 100px;
}

/* Add a transparency effect for thumnbail images */
.demo {
    opacity: 0.6;
}

.active,
.demo:hover {
    opacity: 1;
}

/* Newsletter Section */
#newsletter {
    margin-top: 5115px;
    height: 390px;
    background: #000;
}

.newsletter {
    background: #000000;
    position: relative;
    flex: 1;
    height: 320px;
    overflow: hidden;
}

.newsletter img {
    opacity: 0.5;
    position: relative;
    vertical-align: top;
    transition: 0.6s;
    transition-property: opacity;
    width: 100%;
    height: 100%;
}

.newsletter:hover img {
    opacity: .2;
}

.newsletter .details {
    position: absolute;
    top: 0;
    right: 0;
    color: #ffffff;
    width: 100%;
    height: 100%;
}

.newsletter .details h2 {
    padding: 0px 15px 0px 15px;
    text-align: center;
    font-size: 35px;
    text-transform: uppercase;
    font-weight: 300;
    margin-top: 165px;
    transition: 0.6s;
    transition-property: transform;
}

.newsletter .details h2 span {
    font-weight: 900;
}

.newsletter:hover .details h2 {
    transform: translateY(-70px);
}

.newsletter .details p {
    margin: 30px 30px 0 30px;
    font-size: 18px;
    font-weight: 600;
    text-align: center;
    opacity: 0;
    transition: 0.6s;
    transition-property: opacity, transform;
}

.newsletter:hover .details p {
    opacity: 1;
    transform: translateY(-70px);
}

.email {
    font-weight: bold;
    padding-left: 5px;
    width: 255px;
    height: 35px;
    border-radius: 5px;
}

.signup-btn {
    border: none;
    background-image: linear-gradient(to bottom right, #8A2387, #E94057, #F27121);
    color: white;
    padding: 5px 15px;
    text-align: center;
    text-decoration: none;
    font-size: 12px;
    font-weight: bold;
    text-transform: uppercase;
    border-radius: 5px;
    height: 35px;
    width: 90px;
}

.signup-btn:hover {
    opacity: 0.8;
}


/* Blog Section */
#blog {
    margin-top: 5480px;
}

.blog-rows {
    width: 100%;
    height: 600px;
    padding: 0px 69px 69px 69px;
}

.blog-columns {
    float: left;
    width: 30%;
    margin: 15px;
    padding: 10px;
    transition: .5s;
}

.blog-columns:hover {
    box-shadow: 0px 0px 5px 0px rgb(0 0 0);
    border-radius: 10px;
}

.blog-columns img {
    width: 100%;
    border-radius: 5px;
}

.blog-columns p {
    text-align: justify;
    padding: 15px;
}

.blog-columns .date {
    text-align: center;
    padding-top: 10px;
}

.vl {
    opacity: 0.5;
    position: absolute;
    border: 0.5px solid black;
    width: 1px;
    height: 495px;
    margin-top: 15px;
}

/* Contact Section */
#contact {
    margin-top: 6240px;
    background: #fdbc0c;
    padding: 80px;
}

.contact-column {
    float: left;
    width: 50%;
    height: 420px;
}

.map {
    margin: 10px;
    height: 400px;
}

.contact-form {
    padding-left: 40px;
    margin: 10px;
    height: 400px;
}

.form-title {
    font-size: 40px;
    font-weight: bold;
}

input:focus,
textarea:focus {
    outline: none;
}

.form-detail {
    font-weight: bold;
    padding-left: 5px;
    width: 255px;
    height: 35px;
    border-radius: 5px;
    border: none;
}

.form {
    padding: 10px 0px 10px 0px;
}

.msg {
    border-radius: 5px;
    border: none;
    height: 100px;
    font-weight: bold;
    padding-left: 5px;
    padding-top: 5px;
    width: 255px;
    font-family: 'Open Sans';
}

.send-btn {
    border: none;
    background: black;
    background-color: #b140c5;
    color: white;
    padding: 5px 15px;
    text-align: center;
    text-decoration: none;
    font-size: 12px;
    font-weight: bold;
    text-transform: uppercase;
    border-radius: 5px;
    height: 35px;
    width: 255px;
    transition: 0.4s;
}

.send-btn:hover {
    opacity: 0.8;
}

.send-btn:active {
    opacity: 0.6;
}

.footer {
    align-items: center;
    margin-top: 6820px;
    background-color: rgb(255, 255, 255);
    height: 160px;
}

.footer-column {
    float: left;
    width: 31%;
    margin: 1%;
    padding: 2%;
}

.footer-detail {
    font-size: 20px;
    text-transform: uppercase;
    padding-bottom: 5px;
}

.follow-column {
    float: left;
    text-align: center;
    width: 33.3%;
}

