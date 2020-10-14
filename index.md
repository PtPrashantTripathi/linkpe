<!DOCTYPE html>
<html><head>
<meta http-equiv="content-type" content="text/html; charset=UTF-8">
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
<title>UPI LINK Generator</title>
</head>
<body>
<center>
<br>
<h3 style="color: #DAE0E2;">Scan Qr or Click on Pay Now :</h3>
<h4 id="name"></h4>
<canvas id="qr"></canvas>
<br>
<div style="margin-top: 30px;">
<a href="upi://pay?pn=UPAYI&amp;pa=240@ybl&amp;cu=INR&amp;am=4.0">
<img src="upi.png" height="100">
<br>
<button>Click here to Pay Now</button>
</a>
</div>
<br><p style="color: #EAF0F1">Developed BY: <a href="https://ptprashanttripathi.github.io" style="color: cyan;">Pt. Prashant Tripathi</a></p>
</center>

<script src="qrious.js"></script>
<script>
//upi://pay?pa=pt8435782545-2@okaxis&pn=Pt.%20Prashant%20Tripathi
const queryString = window.location.search;
const urlParams = new URLSearchParams(queryString);
const pa = urlParams.get('pa')
const pn = urlParams.get('pn')
//const url= 
document.getElementById("demo").innerHTML =   decodeURIComponent(pa);


      (function() {
        var qr = new QRious({
          element: document.getElementById('qr'),
          background: '#fff',
          foreground: '#000',
          size: 250,
          value: 'upi://pay?pn=UPAYI&pa=pt1998@ybl&cu=INR'
        });
      })();
</script>
</body></html>
