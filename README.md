# Ex01 Portfolio
## Date:

## AIM
To create a Portfolio using HTML and CSS.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for introduction, about, projects, and contact details.

### STEP 5
Define global styles for fonts, colors, and layout.

### STEP 6
Style the header, navigation bar, and sections.

### STEP 7
Use Flexbox or CSS Grid for layout design.

### STEP 8
Add hover effects and transitions for interactivity.

### STEP 9
Add Images and Media.

### STEP 10
Use optimized images for a professional look.

### STEP 11
Open the HTML file in a browser to check layout and functionality.

### STEP 12
Fix styling issues and refine content placement.

### STEP 13
Deploy the Portfolio.

### STEP 14
Upload to GitHub Pages for free hosting.

## PROGRAM
```
Html:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lakshiya | Portfolio</title>

    <link rel="stylesheet" href="style.css">

    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
</head>
<body>

<header>

<nav>
    <h2 class="logo">Portfolio</h2>

    <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#contact">Contact</a></li>
    </ul>
</nav>

</header>

<!-- HERO -->

<section id="home" class="hero">

<div class="hero-text">

<h1>Hi, I'm <span>Lakshiya</span></h1>

<h3>AIML Student & Creative Developer</h3>

<p>
Passionate about Artificial Intelligence, Web Development,
Machine Learning and UI/UX Design. I enjoy building modern,
user-friendly digital experiences.
</p>

<a href="#projects" class="btn">View My Work</a>

</div>

<div class="hero-image">

<img src="laks photo.jpeg" alt="Profile Picture">

</div>

</section>

<!-- ABOUT -->

<section id="about">

<h2>About Me</h2>

<p>

I'm a B.Tech Artificial Intelligence & Machine Learning student with
a passion for creating beautiful websites and intelligent applications.
I enjoy solving problems, exploring new technologies, and continuously
improving my skills through projects and competitions.

</p>

</section>

<!-- PROJECTS -->

<section id="projects">

<h2>Projects</h2>

<div class="project-container">

<div class="card">



<h3>EcoTrack</h3>

<p>
Carbon Footprint Awareness Platform built using modern web technologies.
</p>

</div>

<div class="card">


<h3>Prompt Wars</h3>

<p>
Interactive AI Prompt Challenge platform designed for students.
</p>

</div>

<div class="card">


<h3>Portfolio Website</h3>

<p>
Responsive portfolio showcasing projects, skills and achievements.
</p>

</div>

</div>

</section>

<!-- CONTACT -->

<section id="contact">

<h2>Contact Me</h2>

<p>Email : lakshiya@example.com</p>

<p>LinkedIn : linkedin.com/in/lakshiya</p>

<p>GitHub : github.com/lakshy122007-pixel</p>

</section>

<footer>

<p>© 2026 Lakshiya Rajkumar | All Rights Reserved</p>

</footer>

</body>
</html>
```
```
CSS:
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    scroll-behavior:smooth;
}

body{
    font-family:'Poppins',sans-serif;
    background:#f0bce8;
    color:#1F2937;
}

/* NAVIGATION */

header{
    position:sticky;
    top:0;
    background:rgb(249, 250, 250);
    box-shadow:0 3px 10px rgba(0,0,0,.08);
    z-index:1000;
}

nav{
    width:90%;
    margin:auto;
    display:flex;
    justify-content:space-between;
    align-items:center;
    height:75px;
}

.logo{
    color:#801598;
    font-size:30px;
}

nav ul{
    display:flex;
    list-style:none;
}

nav ul li{
    margin-left:35px;
}

nav a{
    text-decoration:none;
    color:#333;
    font-weight:500;
    transition:.3s;
}

nav a:hover{
    color:#2563EB;
}

/* HERO */

.hero{

    width:90%;
    margin:auto;

    min-height:90vh;

    display:flex;
    justify-content:space-between;
    align-items:center;

}

.hero-text{

    width:55%;

}

.hero-text h1{

    font-size:60px;
    margin-bottom:20px;

}

.hero-text span{

    color:#2563EB;

}

.hero-text h3{

    font-size:30px;
    color:#4B5563;

}

.hero-text p{

    margin:30px 0;
    line-height:1.8;
    font-size:18px;

}

.btn{

    display:inline-block;
    text-decoration:none;

    background:#2563EB;
    color:white;

    padding:15px 35px;

    border-radius:40px;

    transition:.3s;

}

.btn:hover{

    background:#1D4ED8;

    transform:translateY(-3px);

}

.hero-image img{

    width:380px;
    border-radius:50%;
    box-shadow:0 15px 30px rgba(0,0,0,.2);

}

/* ABOUT */

section{

    padding:90px 10%;

}

section h2{

    font-size:42px;
    margin-bottom:30px;
    text-align:center;

}

section p{

    font-size:18px;
    line-height:1.9;
    text-align:center;

}

/* PROJECTS */

.project-container{

    display:flex;
    justify-content:center;
    gap:30px;
    flex-wrap:wrap;

}

.card{

    width:320px;

    background:white;

    border-radius:18px;

    overflow:hidden;

    box-shadow:0 10px 20px rgba(0,0,0,.08);

    transition:.4s;

}

.card:hover{

    transform:translateY(-10px);

    box-shadow:0 18px 35px rgba(0,0,0,.15);

}

.card img{

    width:100%;
    height:200px;
    object-fit:cover;

}

.card h3{

    margin:20px;

}

.card p{

    text-align:left;
    margin:0 20px 20px;
    font-size:15px;

}

/* CONTACT */

#contact{

    background:#2563EB;
    color:white;
    text-align:center;

}

#contact p{

    margin:12px;

}

/* FOOTER */

footer{

    text-align:center;
    padding:25px;
    background:#111827;
    color:white;

}

/* RESPONSIVE */

@media(max-width:900px){

.hero{

flex-direction:column-reverse;
text-align:center;
padding-top:50px;

}

.hero-text{

width:100%;

}

.hero-image img{

width:260px;
margin-bottom:40px;

}

nav{

flex-direction:column;
height:auto;
padding:20px;

}

nav ul{

margin-top:20px;
flex-wrap:wrap;
justify-content:center;

}

nav ul li{

margin:10px;

}

}
```

## OUTPUT


## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
