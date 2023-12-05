# portfolio
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PortFolio Website</title>
    <style>
        *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: -apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,"Helvetica Neue",Arial,sans-serif,"Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol","Noto Color Emoji";
}


/* common code here */
.container{
    max-width: 1100px;
    margin: auto;
}

section{
    padding: 80px 0;
}

body,html{
    scroll-behavior: smooth;
}

body{
    background: #f5f5f5;
}

.title{
    width: 100%;
    text-align: center;
    font-size: 2.5rem;
    text-transform: uppercase;
    font-weight: 500;
}

.line{
    width: 80px;
    background: #0078ff;
    height: 4px;
    margin: 0 auto;
    margin-top: 10px;
}

.menu-btn{
    color: white;
    font-size: 23px;
    cursor: pointer;
    display: none;
}

.scrollbtn{
    height: 40px;
    width: 40px;
    position: fixed;
    right: 20px;
    bottom: 40px;
    background: #0078ff;
    padding: 8px;
    border: none;
    outline: none;
    border-radius: 50%;
    cursor: pointer;
    z-index: 500;
    pointer-events: auto;
}

.scrollbtn i{
    text-align: center;
    font-size: 20px;
    color: white;
}

/* navbar styling */
.navbar{
    position: fixed;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 2rem 8rem;
    z-index: 500;
    transition: 0.4s;
}

.navbar.sticky{
    position: fixed;
    top: 0;
    width: 100%;
    background: white;
    color: #0078ff;
    padding: 1.1rem 8rem;
    box-shadow: 0px 6px 9px 0px rgb(0 0 0 /6%);
}

.navbar .logo a{
    text-decoration: none;
    font-weight: 600;
    font-size: 30px;
    color: white;
}

.navbar.sticky .logo a{
    color: #0078ff;
}

.navbar .menu li{
    list-style: none;
    display: inline-block;
    margin-left: 35px;
    position: relative;
}

.navbar .menu li a{
    display: block;
    text-decoration: none;
    font-size: 16px;
    font-weight: 600;
    color: white;
}

.navbar.sticky .menu li a{
    color: #0078ff;
}

.navbar .menu li a::before{
    content: "";
    position: absolute;
    width: 0%;
    left: 0;
    bottom: -10px;
    height: 2px;
    background: white;
    transition: 0.2s;
}

.navbar.sticky .menu li a::before{
    background: #0078ff;
}

.navbar .menu li a:hover:before{
    width: 35px;
}

/* home styling */
.home{
    position: relative;
    left: 0;
    top: 0;
    height: 100vh;
    background: linear-gradient(rgba(0, 0, 0, 0.88),rgba(0,0,0,0.8)), url(images/intro-bg.jpg) center center/cover no-repeat;
    background-attachment: fixed;
    color: white;
}

.home .home-content{
    width: 100%;
    height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}

.home .home-content h1{
    font-size: 4.2rem;
    margin-bottom: 1.5rem;
}

.home .home-content span{
    font-size: 45px;
}

/* about me styling */
.about-content{
    background: white;
    width: 100%;
    padding: 2.5rem 3rem;
    display: flex;
    box-shadow: 0 1px 1px 0 rgb(0 0 0 /6%), 0 2px 5px 0 rgb(0 0 0 / 20%);
}

.about-content .info{
    width: 50%;
    padding: 5px;
    display: flex;
    flex-direction: column;
}

.about-content .info .personal{
    display: flex;
    align-items: center;
    width: 100%;
}

.about-content .info .personal .photo{
    width: 40%;
    display: flex;
}

.about-content .info .personal .photo img{
    border-radius: 5px;
}

.about-content .info .personal .name{
    align-items: flex-start;
    width: 60%;
}

.about-content .info .personal .name p{
    margin-bottom: 15px;
    font-size: 18px;
}

.about-content .info .personal .name p span{
    font-weight: 600
}

.about-content .info .skills{
    margin-top: 25px;
}

.about-content .info .skills h4{
    font-size: 20px;
    margin-bottom: 20px;
}

.about-content .info .skills .skill{
    width: 100%;
    display: flex;
    justify-content: space-between;
}

.about-content .info .skills {
    margin-top: 10px;
    height: 8px;
    width: 100%;
    
    position: relative;
    margin-bottom: 25px;
}

.about-content .info .skills {
    position: absolute;
    height: 100%;
}

.about-content .info .skills {
    width: 95%;
}

.about-content .info .skills {
    width: 85%;
}

.about-content .info .skills {
    width: 75%;
}

.about-content .info .skills {
    width: 70%;
}

.about-content .aboutme{
    width: 50%;
    padding: 0 20px;
}

.about-content .aboutme h5{
    font-size: 2rem;
    position: relative;
    font-weight: 500;
    margin-bottom: 2.5rem;
}

.about-content .aboutme h5::before{
    content: "";
    position: absolute;
    left: 0;
    bottom: -10px;
    width: 80px;
    height: 4px;
    background: #0078ff;
}

.about-content .aboutme p{
    font-weight: 300;
    margin-bottom: 15px;
    font-size: 20px;
}
.about{
    background-color: #0078ff;
}
.skills{
    padding-top: 280px;
    padding-left: 150px;
}
.name{
    padding-top: 90px;
    margin-right: 150px;
}

/* services section styling */
.Education{
    background: #111;
    color: white;
}

.Education .Education-content{
    margin-top: 2rem;
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: space-around;
}

.Education .Education-content .card{
    width: 330px;
    text-align: center;
    background: #222;
    padding: 20px 15px;
    margin-bottom: 30px;
    border-radius: 10px;
    cursor: pointer;
    transition: 0.3s;
}

.Education .Education-content .card:hover{
    background: #0078ff;
}

.Education .Education-content .card .card-content{
    transition: 0.3s;
}

.Education .Education-content .card:hover .card-content{
    transform: scale(1.07);
}

.Education .Education-content .card .card-content .icon{
    padding: 5px 0;
    color: white;
}

.Education .Education-content .card .card-content .icon i{
    font-size: 5rem;
}

.Education .Education-content .card .card-content .card-title{
    padding: 5px 0;
    font-size: 25px;
    font-weight: 500;
    color: #0078ff;
}

.Education .Education-content .card:hover .card-content .card-title{
    color: white;
}
ul{
    padding-left: 10px;
}

/* contact section styling */
.contact{
    position: relative;
    color: white;
    width: 100%;
    background: url(images/overlay-bg.jpg) center center/cover no-repeat;
    background-attachment: fixed;
    z-index: 0;
    padding-bottom: 30px;
}

.contact .overlay{
    position: absolute;
    left: 0;
    top: 0;
    width: 100%;
    height: 100%;
    background: #0078ff;
    opacity: 0.7;
    z-index: -1;
    pointer-events: none;
}

.contact .contact-content{
    background: white;
    color: black;
    z-index: 100;
    width: 100%;
    padding: 2.5rem;
    display: flex;
}

.contact .contact-content .heading{
    font-size: 2rem;
    font-weight: 500;
}

.contact .contact-content .line{
    margin: 0;
    width: 100px;
    height: 4px;
    margin-top: 12px;
    margin-bottom: 25px;
}

.contact .contact-content .message{
    width: 50%;
    padding: 0 15px;
}

.contact .contact-content .message .field{
    width: 100%;
    margin-bottom: 20px;
}

.contact .contact-content .message .field input,
.contact .contact-content .message .field textarea{
    width: 100%;
    height: 40px;
    border: 1px solid #888;
    outline: none;
    border-radius: 5px;
    padding-left: 15px;
    font-size: 16px;
}

.contact .contact-content .message .field textarea{
    height: 100px;
    padding-top: 5px;
}

.contact .contact-content .message button{
    padding: 15px 25px;
    background: #0078ff;
    color: white;
    font-size: 20px;
    border-radius: 10px;
    outline: none;
    border: none;
    cursor: pointer;
}

.contact .contact-content .gettouch{
    width: 50%;
    padding: 0 15px;
}

.contact .contact-content .gettouch p{
    color: rgba(0,0,0,0.6);
    font-weight: 300;
    margin-bottom: 20px;
    font-size: 20px;
    line-height: 1.5;
}

.contact .contact-content .gettouch .info{
    margin-bottom: 15px;
}

.contact .contact-content .gettouch .info i{
    font-size: 18px;
    color: #0078ff;
    margin-right: 15px;
}

.contact .contact-content .gettouch .social{
    width: 100%;
}

.contact .contact-content .gettouch .social i{
    width: 45px;
    font-size: 25px;
    color: white;
    background: #444;
    padding: 10px;
    text-align: center;
    margin: 20px 5px 0 0;
    cursor: pointer;
    border-radius: 5px;
    transition: 0.5s;
} 

.contact .contact-content .gettouch .social i:hover{
    background: #0078ff;
    transform: translateY(-10px);
}

.contact .footer{
    margin-top: 35px;
}

.contact .footer p{
    text-align: center;
    font-size: 18px;
}

.contact .footer p a{
    text-transform: none;
    color: white;
}

/* responsive styling start here */
@media (max-width:1024px){
    .navbar,
    .navbar.sticky{
        padding: 0.5rem 1.5rem;
    }

    .about .container{
        padding: 0 1.5rem;
    }

    .contact .container{
        padding: 0 1.5rem;
    }
}

@media (max-width:890px){
    .about .container{
        padding: 0 1rem;
    }

    .about-content{
        display: block;
        padding: 25px;
    }

    .about-content .info{
        width: 100%;
        display: flex;
        padding: 0;
    }

    .about-content .aboutme{
        width: 100%;
        padding: 0;
    }
}

@media (max-width:768px){
    .navbar,
    .navbar.sticky{
        padding: 0.5rem 2.5rem;
    }

    .navbar .menu{
        position: fixed;
        height: 100vh;
        width: 100%;
        left: -100%;
        top: 0;
        background: #0078ff;
        color: white;
        text-align: center;
        padding-top: 50px;
        transition: 0.5s;
    }

    .navbar .menu.active{
        left: 0;
    }

    .navbar .menu li{
        display: block;
        margin: 0;
    }

    .navbar .menu li a{
        display: inline-block;
        margin: 20px 0;
        font-size: 25px;
    }

    .navbar .menu li a:hover::before{
        width: 0vh;
    }

    .navbar .menu li a,
    .navbar.sticky .menu li a{
        color: white;
    }

    .navbar .menu-btn{
        display: block;
        z-index: 999;
    }

    .navbar.sticky .menu-btn i{
        color: black;
    }

    .navbar .menu-btn i.active:before{
        content: "\f00d";
    }

    .navbar.sticky .menu-btn i.active{
        color: white;
    }

    .home .home-content h1{
        text-align: center;
        padding: 0 20px;
        font-size: 3.2rem;
        margin-bottom: 1.5rem;
    }

    .home .home-content span{
        font-size: 40px;
    }

    .contact .container{
        padding: 0 15px;
    }

    .contact .contact-content{
        display: block;
    }

    .contact .contact-content .message{
        width: 100%;
        padding: 0;
        margin-bottom: 30px;
    }

    .contact .contact-content .message button{
        padding: 10px 15px;
    }

    .contact .contact-content .gettouch{
        width: 100%;
        padding: 0;
    }
}

@media (max-width:500px){
    .home .home-content h1{
        font-size: 2.5rem;
    }

    .home .home-content span{
        font-size: 30px;
    }

    .about-content .info .personal{
        display: block;
    }

    .about-content .info .personal .photo{
        width: 100%;
        margin-bottom: 20px;
    }

    .about-content .info .personal .name{
        width: 100%;
    }
}
    </style>
    <!-- typed.js  -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/typed.js/2.0.12/typed.min.js"></script>

    <!-- font awesome link -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
</head>
<body>

    <!-- scroll to top button -->
    <button class="scrollbtn" id="btn" type="button" onclick="scrolltoTop()"><i class="fa fa-arrow-up"></i></button>

    <!-- navbar code start here -->
    <nav class="navbar" id="navbar">
        <div class="logo">
            <a href="#home">PortFolio</a>
        </div>
        <ul class="menu" id="menu">
            <li><a href="#home" onclick="menu()">Home</a></li>
            <li><a href="#about" onclick="menu()">About</a></li>
            <li><a href="#Education" onclick="menu()">Education</a></li>
            <li><a href="#contact" onclick="menu()">Contact</a></li>
        </ul>
        <div class="menu-btn" onclick="menu()"><i class="fa fa-bars"></i></div>
    </nav>

    <!-- home section start here -->
    <div class="home" id="home">
        <div class="home-content">
            <h1 class="name">I am Kudumula Varalakshmi Himaja</h1>
            <p><span class="typing"></span></p>
        </div>
    </div>

    <!-- about section start here -->
    <section class="about" id="about">
        <div class="container">
            <div class="about-content">
                <div class="info">
                    <div class="personal">
                        <div class="photo">
                            <img src="images/testimonial-2.jpg" alt="">
                        </div>
                        <div class="name">
                            <p><span>Name:</span> K Varalakshmi Himaja</p>
                            <p><span>Profile:</span> Web Developer</p>
                            <p><span>Address:</span> Vijayawada</p>
                            <p><span>Phone:</span>9490224853</p>
                        </div>
                    </div>
                    <div class="skills">
                        <h4>Skills</h4>
                        <ul>
                            <li>Python</li>
                            <li>C</li>
                            <li>Java</li>
                            <li>Web development</li>
                            <li>Data Structures</li>
                        </ul>
                       
                    </div>
                </div>
                <div class="aboutme">
                    <h5>About me</h5>
                    <p>I am an enthusiastic, self-motivated, reliable, responsible
                        and hard working person. I am a mature team worker and
                        adaptable to all challenging situations. I am able to work
                        well both in a team environment as well as using own
                        initiative. I am able to work well under pressure and
                        adhere to strict deadlines.
                        </p>
                    <p>I am the one who is always passionate about the
                        evolving technology that creates wonders in our lives.
                        My interests lies in AI,ML, DS how it can help in the
                        progress of wider community. I always believe that
                        success can be achieved only when we implement our
                        plans wisely. I am a kind of person who is dedicated to
                        complete any task assigned to me with perfection.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- services section start here -->
    <section class="Education" id="Education">
        <div class="container">
            <h3 class="title">Education</h3>
            <div class="line"></div>
            <div class="Education-content">
                <div class="card">
                    <div class="card-content">
                        <div class="card-title">Schooling</div>
                        <p><ul>
                            <li>10th class</li>
                            <li>Bhashyam High School</li>
                            <li>Guntur</li>
                            <li>CGPA:10</li>
                        </ul></p>
                    </div>
                </div>
                <div class="card">
                    <div class="card-content">
                        <div class="card-title">Intermediate</div>
                        <p><ul>
                            <li>Intermediate</li>
                            <li>Sri Chaitanya Junior College</li>
                            <li>Vijayawada</li>
                            <li>Percentage:97.5%</li>
                        </ul></p>
                    </div>
                </div>
                <div class="card">
                    <div class="card-content">
                        <div class="card-title">Graduation</div>
                        <p><ul>
                            <li>B.tech</li>
                            <li>Vishnu Institute Of Technology</li>
                            <li>Bhimavaram</li>
                            <li>CGPA:9.2</li>
                        </ul></p>
                    </div>
                </div>
               
            </div>
        </div>
    </section>
    <!-- contact section start here -->
    <section class="contact" id="contact">
        <div class="overlay"></div>
        <div class="container">
            <div class="contact-content">
                <div class="message">
                    <form>
                        <h3 class="heading">Send Message us</h3>
                        <div class="line"></div>
                        <div class="field">
                            <input type="text" placeholder="Your Name">
                        </div>
                        <div class="field">
                            <input type="email" placeholder="Your Email">
                        </div>
                        <div class="field">
                            <input type="text" placeholder="Subject">
                        </div>
                        <div class="field">
                            <textarea cols="30" rows="10" placeholder="Message"></textarea>
                        </div>
                        <button type="submit">Send Message</button>
                    </form>
                </div>
                <div class="gettouch">
                    <h3 class="heading">Get in Touch</h3>
                    <div class="line"></div>
                    <div class="info"><i class="fa fa-map-marker"></i>Vijayawada,Andhra Pradesh</div>
                    <div class="info"><i class="fa fa-phone"></i>1234567890</div>
                    <div class="info"><i class="fa fa-envelope"></i>himajakudumula2004@gmail.com</div>
                    <div class="social">
                        <i class="fa fa-facebook"></i>
                        <i class="fa fa-instagram"></i>
                        <i class="fa fa-twitter"></i>
                        <i class="fa fa-youtube-play"></i>
                    </div>
                </div>
            </div>
        </div>
        <footer class="footer">
            <p>© Copyright PortFolio. All Rights Reserved</p>
            
        </footer>
    </section>
    
    <script src="main.js"></script>
</body>
</html>
