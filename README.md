# my_first_project
<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>

<title>My First Code</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

body{
    font-family:'Poppins',sans-serif;
    min-height:100vh;
    background:linear-gradient(135deg,#0f172a,#111827,#1e293b);
    display:flex;
    justify-content:center;
    align-items:center;
    overflow:hidden;
    color:white;
}

/* Animation Background */

.bg{
    position:absolute;
    width:500px;
    height:500px;
    background:rgba(59,130,246,0.15);
    filter:blur(100px);
    border-radius:50%;
    animation:move 8s infinite alternate;
}

.bg2{
    position:absolute;
    right:-100px;
    bottom:-100px;
    width:400px;
    height:400px;
    background:rgba(168,85,247,0.15);
    filter:blur(100px);
    border-radius:50%;
    animation:move2 10s infinite alternate;
}

@keyframes move{
    from{
        transform:translateY(-40px);
    }
    to{
        transform:translateY(40px);
    }
}

@keyframes move2{
    from{
        transform:translateX(-50px);
    }
    to{
        transform:translateX(50px);
    }
}

/* Card */

.card{
    position:relative;
    width:350px;
    padding:35px;
    border-radius:28px;
    background:rgba(255,255,255,0.08);
    backdrop-filter:blur(15px);
    border:1px solid rgba(255,255,255,0.15);
    box-shadow:0 10px 40px rgba(0,0,0,0.4);
    text-align:center;
    z-index:10;
    animation:fade 1s ease;
}

@keyframes fade{
    from{
        opacity:0;
        transform:translateY(40px);
    }
    to{
        opacity:1;
        transform:translateY(0);
    }
}

.logo{
    width:90px;
    height:90px;
    margin:auto;
    border-radius:50%;
    background:linear-gradient(135deg,#3b82f6,#8b5cf6);
    display:flex;
    align-items:center;
    justify-content:center;
    font-size:38px;
    margin-bottom:20px;
    box-shadow:0 0 30px rgba(59,130,246,0.5);
}

h1{
    font-size:28px;
    margin-bottom:10px;
}

h1 span{
    background:linear-gradient(90deg,#60a5fa,#a855f7);
    -webkit-background-clip:text;
    -webkit-text-fill-color:transparent;
}

p{
    font-size:14px;
    color:#d1d5db;
    line-height:1.6;
    margin-bottom:25px;
}

/* Button */

button{
    border:none;
    padding:14px 30px;
    border-radius:14px;
    font-size:15px;
    font-weight:600;
    cursor:pointer;
    background:linear-gradient(90deg,#3b82f6,#8b5cf6);
    color:white;
    transition:0.3s;
    box-shadow:0 8px 20px rgba(59,130,246,0.3);
}

button:hover{
    transform:translateY(-3px) scale(1.03);
    box-shadow:0 12px 25px rgba(168,85,247,0.4);
}

/* Footer */

.footer{
    margin-top:20px;
    font-size:12px;
    color:#9ca3af;
}

</style>
</head>

<body>

<div class="bg"></div>
<div class="bg2"></div>

<div class="card">

    <div class="logo">
        💻
    </div>

    <h1>My <span>First Code</span></h1>

    <p>
        Bienvenue dans mon premier projet HTML créé avec GitHub Codespaces 🚀
    </p>

    <button>
        Commencer
    </button>

    <div class="footer">
        Créé par Napsteur Nikoue ✨
    </div>

</div>

</body>
</html>