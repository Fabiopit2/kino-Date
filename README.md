# kino-Date
<!DOCTYPE html>
<html lang="de">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>VIP Ticket</title>

<style>
body{
    margin:0;
    background:linear-gradient(135deg,#090909,#1f1f1f);
    display:flex;
    justify-content:center;
    align-items:center;
    height:100vh;
    font-family:Arial,sans-serif;
    color:white;
}

.ticket{
    width:360px;
    max-width:90%;
    background:#f7f1d5;
    color:#222;
    border-radius:20px;
    overflow:hidden;
    box-shadow:0 15px 40px rgba(0,0,0,.5);
    animation:appear .8s;
}

.header{
    background:#111;
    color:#ffd700;
    text-align:center;
    padding:20px;
}

.header h1{
    margin:0;
}

.content{
    padding:25px;
}

.line{
    border-top:2px dashed #999;
    margin:18px 0;
}

button{
    width:100%;
    padding:16px;
    border:none;
    border-radius:12px;
    background:#d62828;
    color:white;
    font-size:18px;
    cursor:pointer;
    transition:.25s;
}

button:hover{
    transform:scale(1.03);
}

.success{
    display:none;
    text-align:center;
    animation:appear .8s;
}

.success h1{
    color:#ffd700;
}

@keyframes appear{
from{
opacity:0;
transform:translateY(25px);
}
to{
opacity:1;
transform:translateY(0);
}
}
</style>
</head>

<body>

<div class="ticket" id="ticket">

<div class="header">
<h1>🎬 VIP TICKET</h1>
<p>Nur für eine ganz besondere Person ❤️</p>
</div>

<div class="content">

<h2>Film</h2>
<p><strong>THE ODYSSEY</strong></p>

<div class="line"></div>

<p><strong>Begleitung:</strong><br>❤️ mein Bebe ❤️</p>

<p><strong>Datum:</strong><br>17.07.2026</p>

<p><strong>Zeit:</strong><br>20:30</p>

<div class="line"></div>

<p style="text-align:center">
🍿 Zwei Tickets.<br>
Eines davon gehört hoffentlich dir.
</p>

<br>

<button onclick="acceptTicket()">
🎟️ Ticket annehmen
</button>

</div>

</div>

<script>

function acceptTicket(){

document.getElementById("ticket").innerHTML=`

<div class="header">
<h1>❤️ Reservierung bestätigt ❤️</h1>
</div>

<div class="content success" style="display:block;">

<h2>Yeeey! 🥹</h2>

<p>
Jetzt ist es offiziell...
</p>

<h2>Du bist mein Kino-Date für <br>🎬 THE ODYSSEY 🍿</h2>

<p>
Ich freue mich riesig auf einen wunderschönen Abend mit dir.<br><br>

❤️ Bis ganz bald ❤️
</p>

<p style="font-size:40px;">🍿✨❤️</p>

</div>

`;

}

</script>

</body>
</html>