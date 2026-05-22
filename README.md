# www.eagleyeviewtourstrecks.com
Your Trusted travel agent in Bhutan 
index.html<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Eagle Eye Tours & Treks Bhutan</title>

<style>
body{
margin:0;
font-family:Arial, sans-serif;
background:#0b0f14;
color:white;
}

/* HERO */
.hero{
height:100vh;
background:url('https://upload.wikimedia.org/wikipedia/commons/5/5e/Tiger%27s_Nest_Bhutan_cliff_monastery.jpg') center/cover no-repeat;
display:flex;
align-items:center;
justify-content:center;
text-align:center;
position:relative;
}

.hero::after{
content:"";
position:absolute;
inset:0;
background:rgba(0,0,0,0.6);
}

.hero-content{
position:relative;
z-index:2;
padding:20px;
}

.hero h1{
font-size:55px;
margin-bottom:10px;
}

.hero p{
font-size:18px;
opacity:0.9;
}

.btn{
display:inline-block;
margin:10px;
padding:12px 20px;
background:#ff9800;
border-radius:6px;
font-weight:bold;
text-decoration:none;
color:white;
}

/* SECTIONS */
section{
padding:70px 20px;
max-width:1100px;
margin:auto;
}

.title{
text-align:center;
font-size:36px;
margin-bottom:40px;
color:#ffd27a;
}

/* GRID */
.grid{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(260px,1fr));
gap:20px;
}

.card{
background:#121a24;
border-radius:12px;
overflow:hidden;
box-shadow:0 10px 25px rgba(0,0,0,0.4);
transition:0.3s;
}

.card:hover{
transform:translateY(-5px);
}

.card img{
width:100%;
height:220px;
object-fit:cover;
}

.card-content{
padding:15px;
}

/* PRICING */
.box{
background:#121a24;
padding:20px;
border-radius:12px;
max-width:600px;
margin:auto;
}

input,select{
width:100%;
padding:12px;
margin:10px 0;
border-radius:6px;
border:none;
}

.total{
font-size:24px;
color:#ffd27a;
font-weight:bold;
margin-top:10px;
}

/* FOOTER */
footer{
text-align:center;
padding:30px;
background:#000;
}
</style>
</head>

<body>

<!-- HERO -->
<div class="hero">
<div class="hero-content">
<h1>Eagle Eye Tours & Treks</h1>
<p>Discover the Real Himalayan Kingdom of Bhutan</p>

<a class="btn" href="https://wa.me/97517558956" target="_blank">WhatsApp Booking</a>
<a class="btn" href="tel:+97517558956">Call Now</a>
<a class="btn" href="https://facebook.com" target="_blank">Facebook</a>
</div>
</div>

<!-- DESTINATIONS -->
<section>
<h2 class="title">Explore Bhutan</h2>

<div class="grid">

<div class="card">
<img src="https://upload.wikimedia.org/wikipedia/commons/5/5e/Tiger%27s_Nest_Bhutan_cliff_monastery.jpg">
<div class="card-content">
<h3>Tiger’s Nest Monastery</h3>
<p>Most iconic cliff monastery in Bhutan.</p>
</div>
</div>

<div class="card">
<img src="https://upload.wikimedia.org/wikipedia/commons/3/3e/Paro_Valley_Bhutan.jpg">
<div class="card-content">
<h3>Paro Valley</h3>
<p>Green valley surrounded by Himalayan mountains.</p>
</div>
</div>

<div class="card">
<img src="https://upload.wikimedia.org/wikipedia/commons/1/1d/Thimphu_Bhutan_city_view.jpg">
<div class="card-content">
<h3>Thimphu City</h3>
<p>Capital city blending culture and modern life.</p>
</div>
</div>

<div class="card">
<img src="https://upload.wikimedia.org/wikipedia/commons/8/8c/Himalayan_trekking_path_Bhutan.jpg">
<div class="card-content">
<h3>Trekking Routes</h3>
<p>Adventure trekking through Himalayan trails.</p>
</div>
</div>

</div>
</section>

<!-- PRICING -->
<section>
<h2 class="title">Tour Package Calculator</h2>

<div class="box">

<p><b>USD 2500 per head / per day</b></p>

<label>Number of People</label>
<input type="number" id="people" value="1" min="1">

<label>Number of Days</label>
<input type="number" id="days" value="1" min="1">

<label>Package Type</label>
<select id="rate">
<option value="2500">Standard Tour</option>
<option value="3200">Premium Tour</option>
<option value="4200">Luxury VIP Tour</option>
</select>

<div class="total" id="total">Total: USD 2500</div>

<br>

<a class="btn" style="background:#0070ba"
href="https://www.paypal.com/paypalme/lepchadendup7"
target="_blank">
Pay with PayPal
</a>

</div>
</section>

<!-- FOOTER -->
<footer>
📞 17558956 | 💬 WhatsApp | 📘 Facebook: Dendup Wangyel Lepcha  
<br><br>
© Eagle Eye Tours & Treks Bhutan
</footer>

<!-- SCRIPT -->
<script>
function calc(){
let p=document.getElementById("people").value;
let d=document.getElementById("days").value;
let r=document.getElementById("rate").value;

let total=p*d*r;
document.getElementById("total").innerText="Total: USD "+total;
}

document.querySelectorAll("input,select").forEach(e=>e.oninput=calc);
calc();
</script>

</body>
</html>