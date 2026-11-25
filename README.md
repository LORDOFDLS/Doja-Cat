<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>DOJA CAT Fan Membership (Unofficial)</title>
<style>
*{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth}
:root{--pink:#ff4fa3;--black:#0b0b0d;--white:#fff}
body{background:var(--black);color:var(--white);font-family:Georgia,'Times New Roman',serif;line-height:1.6}
h1,h2,h3,button,nav a{font-family:'Helvetica Neue',Arial,sans-serif;letter-spacing:.08em}
.notice{background:var(--pink);color:#000;text-align:center;padding:8px 12px;font:600 .8rem Arial,sans-serif}
nav{display:flex;justify-content:space-between;align-items:center;padding:16px 5%;position:sticky;top:0;background:rgba(11,11,13,.9);backdrop-filter:blur(8px);z-index:10}
nav strong{color:var(--pink);font-size:1.2rem;letter-spacing:.2em}
nav a{color:#fff;text-decoration:none;margin-left:18px;font-size:.8rem;transition:color .3s}
nav a:hover{color:var(--pink)}
.hero{min-height:80vh;display:flex;flex-direction:column;justify-content:center;align-items:center;text-align:center;padding:60px 6%;background:radial-gradient(circle at 50% 30%,rgba(255,79,163,.35),transparent 60%)}
.hero h1{font-size:clamp(2rem,7vw,4.5rem);line-height:1.1;animation:rise 1s ease both}
.hero h1 span{color:var(--pink)}
.hero p{max-width:560px;margin:20px 0 30px;color:#ddd;animation:rise 1.3s ease both}
.btn{background:var(--pink);color:#000;border:0;padding:14px 28px;font-weight:700;font-size:.85rem;cursor:pointer;border-radius:50px;text-decoration:none;display:inline-block;transition:transform .3s,box-shadow .3s}
.btn:hover{transform:translateY(-3px);box-shadow:0 8px 24px rgba(255,79,163,.5)}
@keyframes rise{from{opacity:0;transform:translateY(30px)}to{opacity:1;transform:none}}
section{padding:70px 5%}
h2{text-align:center;font-size:clamp(1.5rem,4vw,2.4rem);margin-bottom:40px}
.cards{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:24px;max-width:1200px;margin:auto}
.card{padding:32px 22px;border-radius:18px;text-align:center;color:#111;transition:transform .35s,box-shadow .35s;animation:rise .8s ease both}
.card:hover{transform:translateY(-10px) scale(1.03);box-shadow:0 20px 40px rgba(255,79,163,.35)}
.card h3{font-size:1rem;margin-bottom:10px}
.price{font:800 2.4rem Arial,sans-serif;margin:10px 0 24px}
.card button{background:#111;color:#fff;border:0;padding:12px 18px;border-radius:50px;font-weight:700;cursor:pointer;font-size:.75rem;transition:background .3s}
.card button:hover{background:var(--pink);color:#000}
.bronze{background:linear-gradient(145deg,#e0a070,#8c5a2b)}
.silver{background:linear-gradient(145deg,#f4f4f4,#9a9a9a)}
.gold{background:linear-gradient(145deg,#ffe27a,#c9971c)}
.premium{background:linear-gradient(145deg,#000,#1a1a1a);color:#f5c542;border:2px solid #f5c542}
.premium button{background:#f5c542;color:#000}
.super{background:linear-gradient(145deg,#000,#ff4fa3);color:#fff;border:2px solid var(--pink)}
.super button{background:#fff;color:#000}
#form-section{display:none;background:#141418}
.form-box{max-width:480px;margin:auto}
label{display:block;margin:16px 0 6px;font:600 .8rem Arial,sans-serif;letter-spacing:.1em}
input,select{width:100%;padding:13px;border-radius:10px;border:1px solid #444;background:#0b0b0d;color:#fff;font-size:1rem}
input:focus,select:focus{outline:2px solid var(--pink)}
.err{color:#ff7a9c;font-size:.8rem;min-height:1em}
.form-box .btn{width:100%;margin-top:24px}
.spinner{display:none;width:16px;height:16px;border:3px solid #000;border-top-color:transparent;border-radius:50%;animation:spin .7s linear infinite;vertical-align:middle;margin-left:8px}
@keyframes spin{to{transform:rotate(360deg)}}
#msg{text-align:center;margin-top:18px}
#thanks{display:none;text-align:center;padding:40px 20px;border:2px solid var(--pink);border-radius:18px;max-width:560px;margin:auto;animation:rise .8s ease}
#thanks h3{color:var(--pink);margin-bottom:10px}
footer{padding:40px 5%;text-align:center;font-size:.85rem;color:#aaa;border-top:1px solid #222}
#privacy{max-width:700px;margin:auto;color:#ccc}
#privacy p{margin-bottom:12px}
</style>
</head>
</body>
<nav><strong>DOJA CAT</strong><div><a href="#plans">PLANS</a><a href="#privacy">PRIVACY</a></div></nav>

<header class="hero">
  <h1>JOIN THE <span>DOJA CAT</span> FAN COMMUNITY</h1>
  <p>Welcome, fans! Become a member of our independent fan community and be part of something special.</p>
  <a class="btn" href="#plans">VIEW MEMBERSHIPS</a>
</header>

<section id="plans">
  <h2>CHOOSE YOUR MEMBERSHIP</h2>
  <div class="cards">
    <div class="card bronze"><h3>BRONZE MEMBERSHIP</h3><div class="price">$150</div><button data-plan="Bronze" data-price="$150">SELECT BRONZE</button></div>
    <div class="card silver"><h3>SILVER MEMBERSHIP</h3><div class="price">$200</div><button data-plan="Silver" data-price="$200">SELECT SILVER</button></div>
    <div class="card gold"><h3>GOLD MEMBERSHIP</h3><div class="price">$350</div><button data-plan="Gold" data-price="$350">SELECT GOLD</button></div>
    <div class="card premium"><h3>PREMIUM MEMBERSHIP</h3><div class="price">$500</div><button data-plan="Premium" data-price="$500">SELECT PREMIUM</button></div>
    <div class="card super"><h3>SUPER CARD MEMBERSHIP</h3><div class="price">$750</div><button data-plan="Super Card" data-price="$750">SELECT SUPER CARD</button></div>
  </div>
</section>

<section id="form-section">
  <h2>MEMBERSHIP APPLICATION</h2>
  <div class="form-box" id="formWrap">
    <form id="appForm" novalidate>
      <label for="name">FULL NAME</label>
      <input id="name" type="text" autocomplete="name">
      <div class="err" id="nameErr"></div>
      <label for="email">GMAIL ADDRESS</label>
      <input id="email" type="email" autocomplete="email" placeholder="you@gmail.com">
      <div class="err" id="emailErr"></div>
      <label for="plan">SELECTED MEMBERSHIP CARD</label>
      <select id="plan">
        <option value="">-- Select a membership --</option>
        <option>Bronze</option><option>Silver</option><option>Gold</option><option>Premium</option><option>Super Card</option>
      </select>
      <div class="err" id="planErr"></div>
      <button class="btn" type="submit" id="submitBtn">SUBMIT APPLICATION<span class="spinner" id="spin"></span></button>
      <div id="msg" class="err"></div>
    </form>
  </div>
  <div id="thanks">
    <h3>THANK YOU FOR YOUR INTEREST IN DOJA CAT FAN MEMBERSHIP!</h3>
    <p>Your membership application has been successfully submitted.</p>
  </div>
</section>

<section id="privacy">
  <h2>PRIVACY POLICY</h2>
  <p>We collect only your full name, email address and chosen membership, solely to process your application and contact you about it. We do not collect passwords or other personal data, and we do not sell or share your information.</p>
  <p>You may request deletion of your information at any time by contacting the site owner.</p>
</section>

<footer>© DOJA CAT Fan Membership. Independent, unofficial fan project, not affiliated with or endorsed by Doja Cat or her management.</footer>

<script>
const PRICES={"Bronze":"$150","Silver":"$200","Gold":"$350","Premium":"$500","Super Card":"$750"};
const section=document.getElementById('form-section'),planSel=document.getElementById('plan');
document.querySelectorAll('.card button').forEach(b=>b.addEventListener('click',()=>{
  section.style.display='block';planSel.value=b.dataset.plan;
  document.getElementById('formWrap').style.display='block';
  document.getElementById('thanks').style.display='none';
  section.scrollIntoView({behavior:'smooth'});
}));
document.getElementById('appForm').addEventListener('submit',async e=>{
  e.preventDefault();
  const name=document.getElementById('name').value.trim(),email=document.getElementById('email').value.trim(),plan=planSel.value;
  const okEmail=/^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(email);
  document.getElementById('nameErr').textContent=name?'':'Please enter your full name.';
  document.getElementById('emailErr').textContent=okEmail?'':'Please enter a valid email address.';
  document.getElementById('planErr').textContent=plan?'':'Please select a membership.';
  if(!name||!okEmail||!plan)return;
  const btn=document.getElementById('submitBtn'),spin=document.getElementById('spin'),msg=document.getElementById('msg');
  btn.disabled=true;spin.style.display='inline-block';msg.textContent='';
  try{
    // Backend must validate, derive price from plan, and send the email.
    const r=await fetch('/api/apply',{method:'POST',headers:{'Content-Type':'application/json'},body:JSON.stringify({name,email,plan})});
    if(!r.ok)throw new Error();
    document.getElementById('formWrap').style.display='none';
    document.getElementById('thanks').style.display='block';
    e.target.reset();
  }catch(err){
    msg.textContent='Something went wrong sending your application. Please try again.';
  }finally{btn.disabled=false;spin.style.display='none';}
});
</script>
</body>
</html>