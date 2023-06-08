<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
    <title>Home</title>
<style>
@import url('https://fonts.googleapis.com/css2?family=Sriracha&display=swap');
*{
    margin: 0;
    padding: 0;
}
.header{
    width: 100%;
    background-color: rgb(245,245,245);
    background-position: center;
    background-size: cover;
    position: sticky;
    top:0;
}
nav{
    display: flex;
    padding: 5px 20px 0px 0px;
    justify-content: space-between;
    align-items: center;
}
nav img{
    width: 170px;
    height: 55px;
    padding: 2px 5px 0px 60px;
}
.nav-links{
    flex: 1;
    text-align: right;
    padding: 0px 20px 0px 0px;
}
.nav-links ul li{
    list-style: none;
    display: inline-block;
    position: relative;
}
.NavBtn{
    font-size: 17px;
    float: right;
    color: #000;
    font-family: 'Open Sans',Helvetica;
    font-weight: 550;
    text-decoration: none;
    padding: 12px 18px 12px 18px;
    letter-spacing: 1px;
}
.NavBtn:hover{
    color: rgb(0,0,0);
    transition: transform 105ms;
    transform: translateY(-6px);
    --color: #3273A6;
    --position: center bottom;
    --width: 45px;
    --height: 3px;
    background: linear-gradient(var(--color), var(--color)) var(--position) / var(--width) var(--height) no-repeat;
    padding-bottom: 10px;
}
.RegistrationBtn {
    display: flex;
    font-family: 'Open Sans',Helvetica;
    font-weight: 550;
    text-decoration: none;
    color: rgb(0,0,0);
    background-color: rgb(255,200,0);
    float: right;
    padding: 12px 18px 12px 18px;
    border-radius: 20px;
    transition: all .3s ease;
    cursor: pointer;
    align-items: center;
    font-size: 17px;
}

.RegistrationBtn > .arrow {
    width: 8px;
    height: 8px;
    border-right: 2px solid #000000;
    border-bottom: 2px solid #000000;
    position: relative;
    transform: rotate(-45deg);
    margin: 0 6px;
    transition: all .3s ease;
}

.RegistrationBtn > .arrow::before {
    display: block;
    background-color: rgb(0,0,0);
    width: 5px;
    transform-origin: bottom right;
    height: 2px;
    position: absolute;
    opacity: 0;
    bottom: calc(-2px / 2);
    transform: rotate(45deg);
    transition: all .3s ease;
    content: "";
    right: 0;
}

.RegistrationBtn:hover > .arrow {
    transform: rotate(-45deg) translate(4px, 4px);
    border-color: rgb(0,0,0);
}

.RegistrationBtn:hover > .arrow::before {
    opacity: 1;
    width: 11px;
}

.RegistrationBtn:hover {
    background-color: rgba(255,200,0);
    color: rgb(0,0,0);
}

/* CSS for main element */

.body{
    position:relative;
    overflow:auto;
}
.title{
    background-image: linear-gradient(to bottom, rgba(0, 0, 0, 0.3) 0%, rgba(0, 0, 0, 0.3) 100%),url('backgroundImage.jpg');
    background-repeat: no-repeat;
    background-attachment: fixed;
    background-size: 100% 100%;
    width: 100%;
    min-height: 450px;
    max-height: 100%;
    display: flex;
    align-items: center;
}
@keyframes slide-in {
    from {
      transform: translateX(-100%);
      opacity: 0.15;
    }
    to {
      transform: translateX(0%);
      opacity: 1;
    }
}
.title-text{
    padding: 50px 150px;
    background-color: rgba(0,0,0,0.65);
    animation: slide-in 900ms;
}
.title-text h1{
    text-align: center;
    display: inline-block;
    font-size: 100px;
    font-family: 'Open Sans',Helvetica;
    color: rgb(244, 244, 241);
    padding: 5px 0px 0px 0px;
    letter-spacing: 4px;
}
.title-text hr{
    color: rgb(244, 244, 241);
    width: 100%;
    border-top: 2px solid;
}

.title-text h2{
    font-size: 30px;
    font-family: 'Open Sans',Helvetica;
    color: rgb(244, 244, 241);
    letter-spacing: 2px;
}
.title-text p{
    text-align: center;
    width: 400px;
    font-size: 16px;
    font-family: 'Open Sans',Helvetica;
    color: rgb(244, 244, 241);
    letter-spacing: 1px;
    padding: 15px 0px 0px 0px;
}
.upcomingEvents{
    font-family: 'Open Sans',Helvetica;
    font-size: 30px;
    color:rgb(74,71,71);
    letter-spacing: 2px;
    background-color: rgb(244, 244, 241);
    padding: 10px 20px 10px 50px;
    max-height: 100%;
    text-align: center;
}
.UpcomingTitle:before{
    content: "";
    display: inline-block;
    width: 10%;
    margin: 2%;
    vertical-align: middle;
    border-bottom: 5px solid;
}
.UpcomingTitle:after{
    content: "";
    display: inline-block;
    width: 10%;
    margin: 2%;
    vertical-align: middle;
    border-bottom: 5px solid;
}
.UpcomingTitle{
    padding: 15px 0px 15px 0px;
    width: 70%;
    margin: 2% auto;
    text-align: center;
}
.slideshow-container {
  max-width: 90%;
  position: relative;
  margin: auto;
}
.slideshow img{
    width: 100%;
}
.footer{
    padding: 15px 0px 0px 0px;
    font-family: 'Open Sans',Helvetica;
    background-color: rgb(244, 244, 241);
    width: 100%;
    position: relative;
    bottom: 0;
}
.copy{
    padding: 6px;
    background:rgba(0,0,0,0.9);
    color:white;
    font-size: 10px;
    font-family: Verdana;
    text-align: center;
    bottom:0;
}
.bottom-links{
    text-align: center;
    padding: 0px 0px 15px 0px;
}
.links {
    text-align: center;
}
.links a{
    margin-left: 20px;
    margin-right: 20px;
    margin-bottom: 15px;
}
.links hr{
    background-color: rgb(0,0,0);
    width: 25%;
    height: 1px;
    margin-left: auto;
    margin-right: auto;
}
.fa {
  padding: 7px;
  width: 15px;
  text-decoration: none;
  border-radius: 50%;
  background-color: rgb(244, 244, 241);
  border-style: solid;
  border-color: black;
  border-width: 2px;
  color: black;
}
.fa-facebook {
  border-style: solid;
  border-color: black;
  border-width: 2px;
  color: black;
}
.fa-twitter {
  border-style: solid;
  border-color: black;
  border-width: 2px;
  color: black;
}
.fa-facebook:hover {
  background: #3B5998;
  color: white;
  border-style: solid;
  border-color: #3B5998;
}
.fa-twitter:hover {
  background: #55ACEE;
  color: white;
  border-style: solid;
  border-color: #55ACEE;
}
.fa-instagram:hover {
  background:radial-gradient(circle at 30% 107%, #fdf497 0%, #fdf497 5%, #fd5949 45%, #d6249f 60%, #285AEB 90%) border-box;
  color:white;
  border-radius: 50em;
  border: 2px solid transparent;
}
.fa-youtube:hover {
  background: #cb2027;
  color: white;
  border-style: solid;
  border-color: #cb2027;
}
.contact-title h2{
    font-family: 'Open Sans',Helvetica;
    font-size: 16px;
    letter-spacing: 2px;
    color: rgb(0,0,0);
    padding: 25px 0px 5px 0px;
}
.contact{
    position: relative;
    display: flex;
    justify-content: space-between;
}
.contact p{
    font-family: 'Open Sans',Helvetica;
    font-size: 14px;
    letter-spacing: 1px;
    text-decoration: none;
    color: rgb(0,0,0);
}
.email{
    display: flex;
    justify-content: center;
    align-items: center;
    transform: translateX(470px);
}
.address{
    display: flex;
    justify-content: center;
    align-items: center;
    transform: translateX(-400px);
}

</style>
</head>

<body>
    <section class="header">
        <nav class="nav-bar">
            <a href="Draft FrontPage.html"><img src="logo_maiset.png" alt="Logo for MAISET"></a>
            <div class="nav-links">
                <ul>
                    <li><a class="NavBtn" href="FrontPage.html">HOME</a></li>
                    <li><a class="NavBtn" href="AboutPage.html">ABOUT</a></li>
                    <li><a class="NavBtn" href="TeamMemberPage.html">TEAM</a></li>
                    <li><a class="NavBtn" href="EventPage.html">NEWS & EVENT</a></li>
                    <li><a class="RegistrationBtn" href="https://forms.gle/ucrnyTdibkN6pYSz7" target="_blank">REGISTER NOW
                        <span class="arrow"></span></a></li>
                </ul>
            </div>
        </nav>
    </section>
    <section>
        <main>
            <div class="title">
                <div class="title-text">
                    <h2><em>WELCOME TO</em></h2>
                    <h1><strong>MAISET</strong></h1>
                    <hr>
                    <p><em>Malaysian Associations of Instrumentation, Science, Engineering and Technology </em></p>
                </div>
            </div>
            <div class="upcomingEvents">
                <h1 class="UpcomingTitle">UPCOMING EVENTS</h1>
                <div class="slide-container">
                    <div class="slideshow">
                        <img class="mySlides" src="images.jpeg" >
                        <img class="mySlides" src="images-3.jpeg">
                    </div>
                </div>
            </div>
        </main>
    </section>
    <section>
        <footer class="footer">
            <div class="footer-words">
                <div class="bottom-links">
                  <div class="links">
                    <a href="#facebook" class="fa fa-facebook"></a>
                    <a href="#twitter" class="fa fa-twitter"></a>
                    <a href="#instagram" class="fa fa-instagram"></a>
                    <a href="#youtube" class="fa fa-youtube"></a>
                    <hr>
                  </div>
                  <div class="contact-title">
                    <h2>CONTACT US</h2>
                    <div class="contact">
                        <p class="email">maiset.fizUPM19@gmail.com</p>
                        <p class="address">Department of Physics,
                        <br>Faculty of Science,
                        <br>Universiti Putra Malaysia,
                        <br>43000 UPM Serdang, Selangor. </p>
                    </div>
                  </div>
                </div>
            </div>
            <div class="copy">Copyrights &copy; MAISET 2023 | All rights reserved</div>
        </footer>
    </section>
<script>
var myIndex = 0;
carousel();

function carousel() {
  var i;
  var x = document.getElementsByClassName("mySlides");
  for (i = 0; i < x.length; i++) {
    x[i].style.display = "none";
  }
  myIndex++;
  if (myIndex > x.length) {myIndex = 1}
  x[myIndex-1].style.display = "block";
  setTimeout(carousel, 4000); // Change image every 4 seconds
}
</script>
</body>
</html>
