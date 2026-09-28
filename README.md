<!DOCTYPE html>
<html lang="am">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Abela eFootball Tournament</title>

<style>
*{
    box-sizing:border-box;
    margin:0;
    padding:0;
}

body{
    font-family:Arial,sans-serif;
    background:#0b0b0b;
    color:#fff;
}

header{
    background:linear-gradient(135deg,#151515,#250000);
    padding:25px 15px;
    text-align:center;
    border-bottom:3px solid #e53935;
}

.logo{
    font-size:34px;
    font-weight:bold;
    color:#e53935;
}

header p{
    color:#aaa;
    margin-top:7px;
}

nav{
    margin-top:20px;
    display:flex;
    justify-content:center;
    flex-wrap:wrap;
    gap:8px;
}

nav a{
    color:#fff;
    text-decoration:none;
    background:#222;
    padding:10px 14px;
    border-radius:6px;
    font-size:14px;
}

nav a:hover{
    background:#e53935;
}

.container{
    max-width:1000px;
    margin:25px auto;
    padding:0 15px;
}

.card{
    background:#171717;
    border:1px solid #292929;
    border-radius:12px;
    padding:20px;
    margin-bottom:20px;
}

.hero{
    text-align:center;
    padding:45px 20px;
    background:linear-gradient(135deg,#191919,#300000);
}

.hero h1{
    font-size:38px;
    color:#e53935;
}

.hero p{
    margin:12px 0 20px;
    color:#ccc;
}

.btn{
    display:inline-block;
    border:none;
    background:#e53935;
    color:white;
    padding:12px 20px;
    border-radius:7px;
    font-weight:bold;
    cursor:pointer;
    text-decoration:none;
}

.btn:hover{
    background:#c62828;
}

.section-title{
    color:#e53935;
    margin-bottom:15px;
    border-bottom:1px solid #333;
    padding-bottom:10px;
}

.info-grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(180px,1fr));
    gap:12px;
}

.info{
    background:#222;
    padding:18px;
    border-radius:8px;
    text-align:center;
}

.info strong{
    display:block;
    font-size:24px;
    color:#e53935;
    margin-bottom:5px;
}

.form-group{
    margin-bottom:15px;
}

label{
    display:block;
    margin-bottom:6px;
    color:#ddd;
}

input,select{
    width:100%;
    padding:12px;
    border:none;
    border-radius:6px;
    background:#292929;
    color:#fff;
    outline:none;
}

input:focus,select:focus{
    border:1px solid #e53935;
}

.score-inputs{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:12px;
}

table{
    width:100%;
    border-collapse:collapse;
    overflow:hidden;
}

th,td{
    padding:12px 8px;
    text-align:center;
    border-bottom:1px solid #333;
}

th{
    background:#292929;
    color:#e53935;
}

tr:hover{
    background:#202020;
}

.result{
    background:#222;
    padding:15px;
    border-radius:8px;
    margin-bottom:10px;
    display:flex;
    justify-content:space-between;
    align-items:center;
    gap:10px;
}

.approve{
    background:#2e7d32;
    border:none;
    color:white;
    padding:8px 12px;
    border-radius:5px;
    cursor:pointer;
}

.delete{
    background:#b71c1c;
    border:none;
    color:white;
    padding:8px 12px;
    border-radius:5px;
    cursor:pointer;
}

.timer{
    text-align:center;
    background:#300000;
    border:1px solid #e53935;
    padding:15px;
    border-radius:8px;
    margin-bottom:20px;
    color:#ff5252;
    font-size:20px;
    font-weight:bold;
}

.bracket{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:15px;
    overflow-x:auto;
}

.round{
    min-width:220px;
}

.round h3{
    text-align:center;
    color:#e53935;
    margin-bottom:10px;
}

.match{
    background:#222;
    border-left:3px solid #e53935;
    padding:12px;
    border-radius:6px;
    margin-bottom:15px;
}

.match div{
    padding:5px 0;
}

.admin{
    border:1px solid #4caf50;
}

.admin h2{
    color:#4caf50;
}

.hidden{
    display:none;
}

.message{
    margin-top:12px;
    padding:10px;
    border-radius:6px;
    background:#202020;
}

footer{
    text-align:center;
    padding:30px 15px;
    margin-top:40px;
    background:#050505;
    color:#777;
}

@media(max-width:600px){
    .hero h1{
        font-size:28px;
    }

    .score-inputs{
        grid-template-columns:1fr;
    }

    .result{
        flex-direction:column;
        align-items:stretch;
    }

    .bracket{
        grid-template-columns:1fr;
    }
}
</style>
</head>

<body>

<header>
    <div class="logo">⚽ ABELA eFOOTBALL</div>
    <p>Official Tournament Website</p>

    <nav>
        <a href="#home">Home</a>
        <a href="#register">ምዝገባ</a>
        <a href="#fixtures">Fixtures</a>
        <a href="#standings">Standings</a>
        <a href="#results">Results</a>
        <a href="#knockout">Knockout</a>
        <a href="#admin">Admin</a>
    </nav>
</header>


<div class="container">

<!-- HOME -->

<section id="home" class="card hero">

    <h1>ABELA eFOOTBALL TOURNAMENT</h1>

    <p>
        እንኳን ወደ Abela eFootball Tournament በደህና መጡ!
    </p>

    <a class="btn" href="#register">Register Now</a>

</section>


<!-- TOURNAMENT INFO -->

<section class="card">

    <h2 class="section-title">🏆 Tournament Information</h2>

    <div class="info-grid">

        <div class="info">
            <strong>16</strong>
            Players
        </div>

        <div class="info">
            <strong>10</strong>
            Minutes
        </div>

        <div class="info">
            <strong>100 ETB</strong>
            Entry Fee
        </div>

        <div class="info">
            <strong>2026</strong>
            Season
        </div>

    </div>

</section>


<!-- REGISTRATION -->

<section id="register" class="card">

    <h2 class="section-title">📝 Player Registration</h2>

    <form id="registrationForm">

        <div class="form-group">
            <label>Player Name</label>
            <input id="regName" type="text" placeholder="የተጫዋች ስም" required>
        </div>

        <div class="form-group">
            <label>eFootball ID</label>
            <input id="regID" type="text" placeholder="eFootball ID" required>
        </div>

        <div class="form-group">
            <label>Telegram Username</label>
            <input id="regTelegram" type="text" placeholder="@username" required>
        </div>

        <button class="btn" type="submit">
            Register
        </button>

    </form>

    <div id="registrationMessage"></div>

</section>


<!-- FIXTURES -->

<section id="fixtures" class="card">

    <h2 class="section-title">📅 Fixtures</h2>

    <table>

        <thead>
            <tr>
                <th>Match</th>
                <th>Player 1</th>
                <th>Player 2</th>
                <th>Status</th>
            </tr>
        </thead>

        <tbody id="fixturesTable">

            <tr>
                <td>1</td>
                <td>Player 1</td>
                <td>Player 2</td>
                <td>Pending</td>
            </tr>

            <tr>
                <td>2</td>
                <td>Player 3</td>
                <td>Player 4</td>
                <td>Pending</td>
            </tr>

        </tbody>

    </table>

</section>


<!-- STANDINGS -->

<section id="standings" class="card">

    <h2 class="section-title">📊 Standings</h2>

    <table>

        <thead>
            <tr>
                <th>#</th>
                <th>Player</th>
                <th>MP</th>
                <th>W</th>
                <th>D</th>
                <th>L</th>
                <th>GF</th>
                <th>GA</th>
                <th>GD</th>
                <th>Pts</th>
            </tr>
        </thead>

        <tbody id="standingsTable">

            <tr>
                <td>1</td>
                <td>Player 1</td>
                <td>0</td>
                <td>0</td>
                <td>0</td>
                <td>0</td>
                <td>0</td>
                <td>0</td>
                <td>0</td>
                <td>0</td>
            </tr>

        </tbody>

    </table>

</section>


<!-- RESULT -->

<section id="results" class="card">

    <h2 class="section-title">⚽ Submit Match Result</h2>

    <div class="timer" id="timer">
        የውጤት ማስገቢያ ጊዜ እየተቆጠረ ነው...
    </div>

    <form id="resultForm">

        <div class="form-group">
            <label>Player 1</label>
            <input id="player1" required>
        </div>

        <div class="form-group">
            <label>Player 2</label>
            <input id="player2" required>
        </div>

        <div class="score-inputs">

            <div class="form-group">
                <label>Player 1 Goals</label>
                <input id="score1" type="number" min="0" required>
            </div>

            <div class="form-group">
                <label>Player 2 Goals</label>
                <input id="score2" type="number" min="0" required>
            </div>

        </div>

        <button class="btn" type="submit">
            Submit Result
        </button>

    </form>

</section>


<!-- KNOCKOUT -->

<section id="knockout" class="card">

    <h2 class="section-title">🏆 Knockout Bracket</h2>

    <div class="bracket">

        <div class="round">

            <h3>Quarter Final</h3>

            <div class="match">
                <div>Player 1</div>
                <div>Player 8</div>
            </div>

            <div class="match">
                <div>Player 4</div>
                <div>Player 5</div>
            </div>

        </div>


        <div class="round">

            <h3>Semi Final</h3>

            <div class="match">
                <div>Winner QF1</div>
                <div>Winner QF2</div>
            </div>

        </div>


        <div class="round">

            <h3>Final</h3>

            <div class="match">
                <div>Winner SF1</div>
                <div>Winner SF2</div>
            </div>

        </div>

    </div>

</section>


<!-- ADMIN -->

<section id="admin" class="card admin">

    <h2 class="section-title">🔐 Admin Panel</h2>

    <div id="loginArea">

        <div class="form-group">
            <label>Admin Password</label>
            <input id="adminPassword" type="password" placeholder="Password">
        </div>

        <button class="btn" onclick="adminLogin()">
            Login
        </button>

        <div id="loginMessage"></div>

    </div>


    <div id="adminArea" class="hidden">

        <h3 style="margin-bottom:15px;color:#4caf50;">
            Pending Results
        </h3>

        <div id="pendingResults">
            <p style="color:#aaa;">
                ምንም pending result የለም።
            </p>
        </div>

        <br>

        <button class="delete" onclick="logout()">
            Logout
        </button>

    </div>

</section>

</div>


<footer>
    © 2026 Abela eFootball Tournament<br>
    All Rights Reserved.
</footer>


<script>

/* =========================
   TOURNAMENT DEADLINE
========================= */

const deadline =
new Date("Oct 1, 2026 18:00:00").getTime();

const timerInterval =
setInterval(updateTimer,1000);

function updateTimer(){

    const now = new Date().getTime();

    const distance = deadline-now;

    if(distance <= 0){

        document.getElementById("timer").innerHTML =
        "⛔ የውጤት ማስገቢያ ጊዜ አልፏል።";

        document.querySelector("#resultForm button").disabled=true;

        clearInterval(timerInterval);

        return;
    }

    const days =
    Math.floor(distance/(1000*60*60*24));

    const hours =
    Math.floor((distance%(1000*60*60*24))/(1000*60*60));

    const minutes =
    Math.floor((distance%(1000*60*60))/(1000*60));

    const seconds =
    Math.floor((distance%(1000*60))/1000);

    document.getElementById("timer").innerHTML =
    `⏳ ቀሪ ጊዜ፦ ${days} ቀን ${hours} ሰዓት ${minutes} ደቂቃ ${seconds} ሴኮንድ`;

}


/* =========================
   REGISTRATION
========================= */

document
.getElementById("registrationForm")
.addEventListener("submit",function(e){

    e.preventDefault();

    const name =
    document.getElementById("regName").value;

    const id =
    document.getElementById("regID").value;

    const telegram =
    document.getElementById("regTelegram").value;

    const players =
    JSON.parse(localStorage.getItem("players") || "[]");

    players.push({
        name:name,
        id:id,
        telegram:telegram
    });

    localStorage.setItem(
        "players",
        JSON.stringify(players)
    );

    document.getElementById(
        "registrationMessage"
    ).innerHTML =
    `<div class="message">
    ✅ ${name} በትክክል ተመዝግቧል!
    </div>`;

    this.reset();

});


/* =========================
   RESULT SUBMISSION
========================= */

document
.getElementById("resultForm")
.addEventListener("submit",function(e){

    e.preventDefault();

    const result={

        player1:
        document.getElementById("player1").value,

        player2:
        document.getElementById("player2").value,

        score1:
        Number(document.getElementById("score1").value),

        score2:
        Number(document.getElementById("score2").value),

        approved:false,

        time:new Date().toLocaleString()

    };


    const results =
    JSON.parse(
        localStorage.getItem("results") || "[]"
    );

    results.push(result);

    localStorage.setItem(
        "results",
        JSON.stringify(results)
    );


    alert(
        "✅ ውጤቱ ተልኳል! Admin ካፀደቀው በኋላ ይታያል።"
    );

    this.reset();

});


/* =========================
   ADMIN LOGIN
========================= */

/*
   CHANGE THIS PASSWORD
*/

const ADMIN_PASSWORD = "Abela2026";


function adminLogin(){

    const password = abela@1210
    document.getElementById("adminPassword").value;

    if(password === ADMIN_PASSWORD){

        document
        .getElementById("loginArea")
        .classList.add("hidden");

        document
        .getElementById("adminArea")
        .classList.remove("hidden");

        loadPendingResults();

    }else{

        document.getElementById(
            "loginMessage"
        ).innerHTML =
        `<div class="message">
        ❌ Wrong password
        </div>`;

    }

}


/* =========================
   ADMIN RESULTS
========================= */

function loadPendingResults(){

    const results =
    JSON.parse(
        localStorage.getItem("results") || "[]"
    );

    const pending =
    document.getElementById("pendingResults");

    const pendingResults =
    results.filter(r => !r.approved);


    if(pendingResults.length === 0){

        pending.innerHTML =
        "<p style='color:#aaa'>ምንም pending result የለም።</p>";

        return;
    }


    pending.innerHTML="";


    pendingResults.forEach((result,index)=>{

        const div =
        document.createElement("div");

        div.className="result";


        div.innerHTML=`

        <div>

        <strong>
        ${result.player1}
        </strong>

        ${result.score1}

        -

        ${result.score2}

        <strong>
        ${result.player2}
        </strong>

        <br>

        <small style="color:#888">
        ${result.time}
        </small>

        </div>

        <button class="approve"
        onclick="approveResult(${index})">
        Approve ✅
        </button>

        `;

        pending.appendChild(div);

    });

}


/* =========================
   APPROVE RESULT
========================= */

function approveResult(index){

    const results =
    JSON.parse(
        localStorage.getItem("results") || "[]"
    );

    const pending =
    results.filter(r => !r.approved);

    const selected =
    pending[index];


    const realIndex =
    results.findIndex(
        r => r === selected
    );


    results[realIndex].approved=true;

    localStorage.setItem(
        "results",
        JSON.stringify(results)
    );


    alert("✅ Result Approved!");

    loadPendingResults();

}


/* =========================
   LOGOUT
========================= */

function logout(){

    document
    .getElementById("adminArea")
    .classList.add("hidden");

    document
    .getElementById("loginArea")
    .classList.remove("hidden");

}


/* =========================
   LOAD STANDINGS
========================= */

function loadStandings(){

    const players =
    JSON.parse(
        localStorage.getItem("players") || "[]"
    );

    const table =
    document.getElementById("standingsTable");

    if(players.length === 0){

        table.innerHTML=`
        <tr>
        <td colspan="10">
        No players registered
        </td>
        </tr>`;

        return;

    }


    let html="";


    players.forEach((player,index)=>{

        html+=`

        <tr>

        <td>${index+1}</td>

        <td>${player.name}</td>

        <td>0</td>
        <td>0</td>
        <td>0</td>
        <td>0</td>
        <td>0</td>
        <td>0</td>
        <td>0</td>
        <td>0</td>

        </tr>

        `;

    });


    table.innerHTML=html;

}


loadStandings();

</script>

</body>
</html>
