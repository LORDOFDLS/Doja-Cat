<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>DOJA CAT Fan Membership (Unofficial)</title>
<style>
*{box-sizing:border-box;margin:0;padding:0;-webkit-tap-highlight-color:transparent}
html{scroll-behavior:smooth;scroll-padding-top:70px;-webkit-text-size-adjust:100%}
:root{--pink:#ff4fa3;--black:#0b0b0d;--white:#fff;--gap:clamp(14px,3vw,28px)}
body{background:var(--black);color:var(--white);font-family:Georgia,'Times New Roman',serif;line-height:1.6;overflow-x:hidden;padding-bottom:env(safe-area-inset-bottom)}
h1,h2,h3,button,nav a,label{font-family:'Helvetica Neue',Arial,sans-serif}
img,svg{max-width:100%}

.notice{background:var(--pink);color:#000;text-align:center;padding:8px 14px;font:600 clamp(.68rem,2.4vw,.8rem) Arial,sans-serif;line-height:1.4}

nav{display:flex;justify-content:space-between;align-items:center;padding:12px 5%;position:sticky;top:0;background:rgba(11,11,13,.92);backdrop-filter:blur(10px);z-index:20;border-bottom:1px solid #1d1d22}
nav strong{color:var(--pink);font-size:1.15rem;letter-spacing:.2em}
.links{display:flex;gap:6px}
.links a{color:#fff;text-decoration:none;font-size:.8rem;letter-spacing:.1em;padding:10px 14px;border-radius:50px;transition:color .3s,background .3s}
.links a:hover{color:var(--pink)}
.burger{display:none;background:none;border:1px solid #333;color:#fff;width:44px;height:44px;border-radius:12px;font-size:1.3rem;cursor:pointer}

.hero{min-height:calc(100vh - 100px);min-height:calc(100dvh - 100px);display:flex;flex-direction:column;justify-content:center;align-items:center;text-align:center;padding:60px 6%;background:radial-gradient(circle at 50% 30%,rgba(255,79,163,.35),transparent 62%),radial-gradient(circle at 85% 90%,rgba(255,79,163,.15),transparent 50%)}
.hero h1{font-size:clamp(1.9rem,8vw,4.6rem);line-height:1.1;letter-spacing:.06em;animation:rise 1s ease both}
.hero h1 span{color:var(--pink)}
.hero p{max-width:560px;margin:20px 0 30px;color:#ddd;font-size:clamp(.95rem,3.4vw,1.15rem);animation:rise 1.3s ease both}
.btn{background:var(--pink);color:#000;border:0;padding:15px 30px;min-height:48px;font-weight:700;font-size:.85rem;letter-spacing:.1em;cursor:pointer;border-radius:50px;text-decoration:none;display:inline-flex;align-items:center;justify-content:center;transition:transform .3s,box-shadow .3s}
.btn:disabled{opacity:.7;cursor:wait}

@keyframes rise{from{opacity:0;transform:translateY(30px)}to{opacity:1;transform:none}}
@keyframes float{0%,100%{transform:translateY(0)}50%{transform:translateY(-6px)}}
.reveal{opacity:0;transform:translateY(30px);transition:opacity .8s ease,transform .8s ease}
.reveal.show{opacity:1;transform:none}

section{padding:clamp(48px,9vw,90px) 5%}
h2{text-align:center;font-size:clamp(1.4rem,5vw,2.4rem);letter-spacing:.08em;margin-bottom:clamp(26px,5vw,44px)}

.cards{display:grid;grid-template-columns:1fr;gap:var(--gap);max-width:1250px;margin:auto}
@media(min-width:560px){.cards{grid-template-columns:repeat(2,1fr)}}
@media(min-width:900px){.cards{grid-template-columns:repeat(3,1fr)}}
@media(min-width:1180px){.cards{grid-template-columns:repeat(5,1fr)}}
.card{padding:34px 20px;border-radius:20px;text-align:center;color:#111;transition:transform .35s,box-shadow .35s;position:relative;overflow:hidden}
.card::after{content:"";position:absolute;top:0;left:-120%;width:60%;height:100%;background:linear-gradient(100deg,transparent,rgba(255,255,255,.35),transparent);transform:skewX(-20deg);transition:left .8s}
.card h3{font-size:.95rem;letter-spacing:.1em;margin-bottom:10px}
.price{font:800 clamp(2.2rem,8vw,2.6rem) Arial,sans-serif;margin:10px 0 24px}
.card button{background:#111;color:#fff;border:0;padding:14px 20px;min-height:46px;width:100%;max-width:220px;border-radius:50px;font-weight:700;cursor:pointer;font-size:.75rem;letter-spacing:.08em;transition:background .3s,color .3s}
.card button:active{transform:scale(.97)}
.bronze{background:linear-gradient(145deg,#e0a070,#8c5a2b)}
.silver{background:linear-gradient(145deg,#f4f4f4,#9a9a9a)}
.gold{background:linear-gradient(145deg,#ffe27a,#c9971c)}
.premium{background:linear-gradient(145deg,#000,#1a1a1a);color:#f5c542;border:2px solid #f5c542}
.premium button{background:#f5c542;color:#000}
.super{background:linear-gradient(145deg,#000,#ff4fa3);color:#fff;border:2px solid var(--pink)}
.super button{background:#fff;color:#000}

@media(hover:hover){
  .btn:hover{transform:translateY(-3px);box-shadow:0 8px 24px rgba(255,79,163,.5)}
  .links a:hover{background:#1a1a1f}
  .card:hover{transform:translateY(-10px) scale(1.03);box-shadow:0 20px 40px rgba(255,79,163,.35)}
  .card:hover::after{left:140%}
  .card button:hover{background:var(--pink);color:#000}
}

#form-section{display:none;background:#141418}
.form-box{max-width:500px;margin:auto}
label{display:block;margin:18px 0 6px;font-weight:600;font-size:.8rem;letter-spacing:.1em}
input,select{width:100%;padding:14px;min-height:50px;border-radius:12px;border:1px solid #444;background:#0b0b0d;color:#fff;font-size:16px}
input:focus,select:focus{outline:2px solid var(--pink);border-color:var(--pink)}
.err{color:#ff7a9c;font-size:.82rem;min-height:1.2em;margin-top:4px}
.form-box .btn{width:100%;margin-top:24px}
.spinner{display:none;width:16px;height:16px;border:3px solid #000;border-top-color:transparent;border-radius:50%;animation:spin .7s linear infinite;margin-left:10px}
@keyframes spin{to{transform:rotate(360deg)}}
#msg{text-align:center;margin-top:16px}
#thanks{display:none;text-align:center;padding:clamp(28px,6vw,48px) 20px;border:2px solid var(--pink);border-radius:20px;max-width:600px;margin:auto;animation:rise .8s ease}
#thanks h3{color:var(--pink);margin-bottom:12px;font-size:clamp(1.05rem,4vw,1.4rem);line-height:1.3}
.hp{position:absolute;left:-9999px;opacity:0;height:0;width:0}

footer{padding:36px 5% calc(36px + env(safe-area-inset-bottom));text-align:center;font-size:.82rem;color:#aaa;border-top:1px solid #222}
#privacy{max-width:720px;margin:auto;color:#ccc}
#privacy p{margin-bottom:14px}

@media(max-width:640px){
  .burger{display:block}
  .links{display:none;position:absolute;top:100%;left:0;right:0;flex-direction:column;background:rgba(11,11,13,.98);padding:10px 5% 18px;border-bottom:1px solid #1d1d22}
  .links.open{display:flex}
  .links a{padding:14px;font-size:.9rem}
}
@media(prefers-reduced-motion:reduce){*{animation:none!important;transition:none!important}.reveal{opacity:1;transform:none}html{scroll-behavior:auto}}
</style>
</head>
<body>
<nav>
  <strong>DOJA CAT</strong>
  <button class="burger" id="burger" aria-label="Menu">☰</button>
  <div class="links" id="links"><a href="#plans">PLANS</a><a href="#privacy">PRIVACY</a></div>
</nav>

<header class="hero">
  <h1>JOIN THE <span>DOJA CAT</span> FAN COMMUNITY</h1>
  <p>Welcome, fans! Become a member of our independent fan community and be part of something special.</p>
  <a class="btn" href="#plans">VIEW MEMBERSHIPS</a>
</header>

<section id="plans">
  <h2 class="reveal">CHOOSE YOUR MEMBERSHIP</h2>
  <div class="cards">
    <div class="card bronze reveal"><h3>BRONZE MEMBERSHIP</h3><div class="price">$150</div><button data-plan="Bronze">SELECT BRONZE</button></div>
    <div class="card silver reveal"><h3>SILVER MEMBERSHIP</h3><div class="price">$200</div><button data-plan="Silver">SELECT SILVER</button></div>
    <div class="card gold reveal"><h3>GOLD MEMBERSHIP</h3><div class="price">$350</div><button data-plan="Gold">SELECT GOLD</button></div>
    <div class="card premium reveal"><h3>PREMIUM MEMBERSHIP</h3><div class="price">$500</div><button data-plan="Premium">SELECT PREMIUM</button></div>
    <div class="card super reveal"><h3>SUPER CARD MEMBERSHIP</h3><div class="price">$750</div><button data-plan="Super Card">SELECT SUPER CARD</button></div>
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
      <input id="email" type="email" inputmode="email" autocomplete="email" placeholder="you@gmail.com">
      <div class="err" id="emailErr"></div>

      <label for="plan">SELECTED MEMBERSHIP CARD</label>
      <select id="plan">
        <option value="">-- Select a membership --</option>
        <option>Bronze</option><option>Silver</option><option>Gold</option><option>Premium</option><option>Super Card</option>
      </select>
      <div class="err" id="planErr"></div>

      <input type="text" id="honey" class="hp" tabindex="-1" autocomplete="off" aria-hidden="true">
      <button class="btn" type="submit" id="submitBtn">SUBMIT APPLICATION<span class="spinner" id="spin"></span></button>
      <div id="msg" class="err" role="alert"></div>
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

<footer>© DOJA CAT Fan Membership. Independent.</footer>

<script src="https://cdn.jsdelivr.net/npm/@emailjs/browser@4.4.1/dist/email.min.js"></script>
<script>
// ===== EmailJS settings =====
const EMAILJS_PUBLIC_KEY='5q5NwQq81hwWTO7A4';
const EMAILJS_SERVICE_ID='service_lak8oed';
const EMAILJS_TEMPLATE_ID='template_e8339hh';
// ============================
emailjs.init({publicKey:EMAILJS_PUBLIC_KEY});

const PRICES={"Bronze":"$150","Silver":"$200","Gold":"$350","Premium":"$500","Super Card":"$750"};

// mobile menu
const links=document.getElementById('links');
document.getElementById('burger').addEventListener('click',()=>links.classList.toggle('open'));
links.querySelectorAll('a').forEach(a=>a.addEventListener('click',()=>links.classList.remove('open')));

// scroll reveal
const io=new IntersectionObserver(es=>es.forEach(en=>{if(en.isIntersecting){en.target.classList.add('show');io.unobserve(en.target)}}),{threshold:.15});
document.querySelectorAll('.reveal').forEach((el,i)=>{el.style.transitionDelay=(i%5)*80+'ms';io.observe(el)});

// card selection
const section=document.getElementById('form-section'),planSel=document.getElementById('plan');
document.querySelectorAll('.card button').forEach(b=>b.addEventListener('click',()=>{
  section.style.display='block';planSel.value=b.dataset.plan;
  document.getElementById('formWrap').style.display='block';
  document.getElementById('thanks').style.display='none';
  document.getElementById('planErr').textContent='';
  section.scrollIntoView({behavior:'smooth'});
}));

// submit
document.getElementById('appForm').addEventListener('submit',async e=>{
  e.preventDefault();
  const name=document.getElementById('name').value.trim().slice(0,100),
        email=document.getElementById('email').value.trim().slice(0,150),
        plan=planSel.value;
  const okEmail=/^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(email);
  document.getElementById('nameErr').textContent=name?'':'Please enter your full name.';
  document.getElementById('emailErr').textContent=okEmail?'':'Please enter a valid email address.';
  document.getElementById('planErr').textContent=PRICES[plan]?'':'Please select a membership.';
  if(!name||!okEmail||!PRICES[plan])return;
  if(document.getElementById('honey').value)return;

  const btn=document.getElementById('submitBtn'),spin=document.getElementById('spin'),msg=document.getElementById('msg');
  btn.disabled=true;spin.style.display='inline-block';msg.textContent='';

  try{
    const res=await emailjs.send(EMAILJS_SERVICE_ID,EMAILJS_TEMPLATE_ID,{
      name:name,
      email:email,
      membership:plan,
      price:PRICES[plan],
      date:new Date().toLocaleString(),
      to_email:'kendrathemylf000@gmail.com',
      subject:'NEW DOJA CAT MEMBERSHIP APPLICATION'
    });
    if(res.status!==200)throw new Error('failed');
    document.getElementById('formWrap').style.display='none';
    document.getElementById('thanks').style.display='block';
    document.getElementById('thanks').scrollIntoView({behavior:'smooth',block:'center'});
    e.target.reset();
  }catch(err){
    console.error(err);
    msg.textContent='Something went wrong sending your application. Please try again.';
  }finally{
    btn.disabled=false;spin.style.display='none';
  }
});
</script>
</body>
</html>
