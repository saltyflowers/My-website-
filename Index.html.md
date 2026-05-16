<!DOCTYPE html>  
<html lang="en">  
<head>  
<meta charset="UTF-8" />  
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>  
<title>Salty’s Flower Bedding</title>  
  
<style>  
* {  
margin: 0;  
padding: 0;  
box-sizing: border-box;  
font-family: Arial, sans-serif;  
scroll-behavior: smooth;  
}  
  
body {  
background: #ffffff;  
color: #1f3d1f;  
}  
  
/* NAV */  
nav {  
position: fixed;  
top: 0;  
width: 100%;  
background: white;  
display: flex;  
justify-content: space-between;  
align-items: center;  
padding: 15px 25px;  
box-shadow: 0 2px 10px rgba(0,0,0,0.1);  
z-index: 1000;  
}  
  
nav h1 {  
font-size: 18px;  
color: #1f6b3a;  
}  
  
nav a {  
margin: 0 10px;  
text-decoration: none;  
color: #1f3d1f;  
font-weight: bold;  
}  
  
/* HERO */  
.hero {  
height: 100vh;  
background: linear-gradient(rgba(0,0,0,0.3), rgba(0,0,0,0.3)),  
url('https://images.unsplash.com/photo-1466692476868-aef1dfb1e735?auto=format&fit=crop&w=1400&q=80');  
background-size: cover;  
background-position: center;  
display: flex;  
flex-direction: column;  
justify-content: center;  
align-items: center;  
text-align: center;  
color: white;  
padding: 20px;  
}  
  
.hero h2 {  
font-size: 40px;  
margin-bottom: 10px;  
}  
  
.hero p {  
font-size: 18px;  
margin-bottom: 20px;  
}  
  
.btn {  
padding: 12px 20px;  
margin: 5px;  
border: none;  
cursor: pointer;  
border-radius: 25px;  
font-weight: bold;  
}  
  
.btn-green {  
background: #1f6b3a;  
color: white;  
}  
  
.btn-white {  
background: white;  
color: #1f6b3a;  
}  
  
/* SECTIONS */  
section {  
padding: 80px 20px;  
max-width: 1000px;  
margin: auto;  
}  
  
h2.section-title {  
text-align: center;  
margin-bottom: 30px;  
font-size: 28px;  
color: #1f6b3a;  
}  
  
/* SERVICES */  
.services {  
display: grid;  
grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));  
gap: 20px;  
}  
  
.card {  
padding: 20px;  
border-radius: 12px;  
box-shadow: 0 3px 10px rgba(0,0,0,0.1);  
text-align: center;  
}  
  
/* GALLERY */  
.gallery {  
display: grid;  
grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));  
gap: 15px;  
}  
  
.gallery img {  
width: 100%;  
border-radius: 10px;  
}  
  
/* FORM */  
form {  
display: flex;  
flex-direction: column;  
gap: 10px;  
max-width: 500px;  
margin: auto;  
}  
  
input, textarea, select {  
padding: 10px;  
border-radius: 8px;  
border: 1px solid #ccc;  
}  
  
button.submit {  
background: #1f6b3a;  
color: white;  
padding: 12px;  
border: none;  
border-radius: 20px;  
cursor: pointer;  
}  
  
/* FOOTER */  
footer {  
text-align: center;  
padding: 20px;  
background: #1f6b3a;  
color: white;  
margin-top: 40px;  
}  
</style>  
</head>  
  
<body>  
  
<!-- NAV -->  
<nav>  
<h1>Salty’s Flower Bedding</h1>  
<div>  
<a href="#home">Home</a>  
<a href="#services">Services</a>  
<a href="#gallery">Gallery</a>  
<a href="#contact">Contact</a>  
</div>  
</nav>  
  
<!-- HERO -->  
<div class="hero" id="home">  
<h2>Beautiful Flower Bedding & Yard Design</h2>  
<p>Pensacola, Florida • Clean Modern Landscaping • Lawn & Flower Experts</p>  
  
<button class="btn btn-green" onclick="document.getElementById('contact').scrollIntoView()">Free Quote</button>  
<button class="btn btn-white" onclick="window.location.href='tel:8506196444'">Call Now</button>  
</div>  
  
<!-- ABOUT -->  
<section>  
<h2 class="section-title">About Us</h2>  
<p style="text-align:center; max-width:700px; margin:auto;">  
Salty’s Flower Bedding creates clean, modern outdoor spaces with flower beds, lawn care, and backyard designs.  
We focus on simple, beautiful, and low-maintenance landscaping for homes in Pensacola, Florida.  
</p>  
</section>  
  
<!-- SERVICES -->  
<section id="services">  
<h2 class="section-title">Services</h2>  
  
<div class="services">  
<div class="card">🌸 Flower Bedding</div>  
<div class="card">🌿 Backyard Designs</div>  
<div class="card">🌱 Lawn Care</div>  
<div class="card">🧹 Yard Cleanups</div>  
<div class="card">🌾 Mulching</div>  
<div class="card">🌼 Seasonal Plants</div>  
</div>  
</section>  
  
<!-- GALLERY -->  
<section id="gallery">  
<h2 class="section-title">Our Work</h2>  
  
<div class="gallery">  
<img src="https://images.unsplash.com/photo-1501004318641-b39e6451bec6" />  
<img src="https://images.unsplash.com/photo-1461354464878-ad92f492a5a0" />  
<img src="https://images.unsplash.com/photo-1446071103084-c257b5f70672" />  
</div>  
</section>  
  
<!-- BOOKING -->  
<section id="contact">  
<h2 class="section-title">Book a Service</h2>  
  
<form onsubmit="event.preventDefault(); alert('Request sent! We will contact you soon.');">  
<input type="text" placeholder="Full Name" required />  
<input type="tel" placeholder="Phone Number" required />  
<input type="text" placeholder="Address (Pensacola area)" required />  
  
<select required>  
<option value="">Select Service</option>  
<option>Flower Bedding</option>  
<option>Lawn Care</option>  
<option>Yard Cleanup</option>  
<option>Full Backyard Design</option>  
</select>  
  
<textarea placeholder="Message / Details"></textarea>  
  
<button class="submit">Send Request</button>  
</form>  
  
</section>  
  
<!-- PAYMENT -->  
<section>  
<h2 class="section-title">Payments</h2>  
  
<p style="text-align:center;">  
Cash App: <b>$j4xty</b><br><br>  
Apple Pay available after booking confirmation<br><br>  
Cash accepted on arrival  
</p>  
</section>  
  
<!-- CONTACT -->  
<section>  
<h2 class="section-title">Contact</h2>  
  
<p style="text-align:center;">  
📍 Pensacola, Florida<br>  
📞 <a href="tel:8506196444">850-619-6444</a><br>  
📧 Jarvissalter402@gmail.com  
</p>  
</section>  
  
<footer>  
© 2026 Salty’s Flower Bedding • All Rights Reserved  
</footer>  
  
</body>  
</html>  
