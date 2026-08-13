<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>EV Charging Station</title>
<script src="https://cdnjs.cloudflare.com/ajax/libs/qrcodejs/1.0.0/qrcode.min.js"></script>
<style>
body{font-family:Arial;background:#f4f4f4}
.container{max-width:700px;margin:20px auto;background:#fff;padding:20px;border-radius:10px}
.page{display:none} .active{display:block}
input,select,button{width:100%;padding:10px;margin:8px 0}
button{background:green;color:#fff;border:none}
#qrcode{display:flex;justify-content:center;margin-top:20px}
</style>
</head>
<body>
<div class="container">

<div id="p1" class="page active">
<h2>Vehicle Details</h2>
<input id="vehicleNo" placeholder="KA01AB1234">
<select id="vehicleCompany">
<option value="">Select Vehicle</option>
<option>Ather 450X</option>
<option>Ola S1 Pro</option>
<option>TVS iQube</option>
<option>Hero Vida V2 Pro</option>
</select>
<button onclick="next1()">Next</button>
</div>

<div id="p2" class="page">
<h2>Battery Details</h2>
<p>Vehicle: <span id="vname"></span></p>
<p>Battery Capacity: <span id="cap"></span> Wh</p>
<input type="number" id="current" placeholder="Current Battery %">
<p>Remaining to 100%: <span id="remain">0</span>%</p>
<p>Power Needed: <span id="powerNeed">0</span> Wh</p>
<input type="number" id="required" placeholder="Required Charging %">
<p>Required Power: <span id="reqPower">0</span> Wh</p>
<p>Amount: ₹<span id="amt">0</span></p>
<button onclick="calc()">Calculate</button>
<button onclick="back1()">Back</button>
<button onclick="next2()">Next</button>
</div>

<div id="p3" class="page">
<h2>Payment QR</h2>
<p>Pay Amount: ₹<span id="payAmt"></span></p>
<div id="qrcode"></div>
<a id="upiBtn"><button>Pay Now</button></a>
<button onclick="back2()">Back</button>
</div>

</div>

<script>
let cap=0;

function show(id){
 document.querySelectorAll('.page').forEach(p=>p.classList.remove('active'));
 document.getElementById(id).classList.add('active');
}

function next1(){
 let no=document.getElementById('vehicleNo').value.toUpperCase().trim();
 let c=document.getElementById('vehicleCompany').value;
 let p=/^[A-Z]{2}[0-9]{1,2}[A-Z]{1,2}[0-9]{4}$/;
 if(!p.test(no)){alert('Invalid vehicle number');return;}
 if(!c){alert('Select vehicle');return;}

 if(c==='Ather 450X') cap=3700;
 if(c==='Ola S1 Pro') cap=4000;
 if(c==='TVS iQube') cap=3500;
 if(c==='Hero Vida V2 Pro') cap=3940;

 document.getElementById('vname').innerText=c;
 document.getElementById('cap').innerText=cap;
 show('p2');
}

function calc(){
 let current=Number(document.getElementById('current').value)||0;
 let req=Number(document.getElementById('required').value)||0;

 let remain=100-current;
 let powerNeed=(remain/100)*cap;
 let reqPower=(req/100)*cap;
 let amount=(reqPower*0.008).toFixed(2);

 document.getElementById('remain').innerText=remain;
 document.getElementById('powerNeed').innerText=powerNeed.toFixed(2);
 document.getElementById('reqPower').innerText=reqPower.toFixed(2);
 document.getElementById('amt').innerText=amount;
}

function back1(){show('p1');}

function next2(){
 let amount=document.getElementById('amt').innerText;
 document.getElementById('payAmt').innerText=amount;

 let upi='upi://pay?pa=7483239374-2@ibl&pn=SUPREETAGOUDA&am='+amount+'&cu=INR';
 document.getElementById('upiBtn').href=upi;

 document.getElementById('qrcode').innerHTML='';
 new QRCode(document.getElementById('qrcode'), {text: upi,width:250,height:250});

 show('p3');
}

function back2(){show('p2');}
</script>
</body>
</html>
