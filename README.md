<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <title>Pour Julie 💖</title>
    <style>
        body {
            margin: 0;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            background: linear-gradient(to bottom, #ffd6e8, #ffc0cb);
            font-family: Arial, sans-serif;
        }

        .card {
            background: white;
            padding: 40px;
            border-radius: 20px;
            text-align: center;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
        }

        h1 {
            color: #ff2e88;
        }

        button {
            padding: 15px 30px;
            border: none;
            border-radius: 30px;
            font-size: 18px;
            cursor: pointer;
            margin: 10px;
            transition: 0.3s;
        }

        .oui {
            background: #ff2e88;
            color: white;
        }

        .non {
            background: #ddd;
        }

        .oui:hover {
            transform: scale(1.1);
        }

    </style>
</head>
<body>

<div class="card">
    <h2>💗 Pour Julie 💗</h2>
    <h1>Veux-tu être ma Valentine ? 💝</h1>
    
    <button class="oui" onclick="oui()">Oui 💖</button>
    <button class="non" onmouseover="fuir()">Non 😢</button>
</div>

<script>
function oui() {
    alert("YEEEEES 💕 Je t’aime trop 😭💖");
}

function fuir() {
    const btn = document.querySelector(".non");
    btn.style.position = "absolute";
    btn.style.top = Math.random() * window.innerHeight + "px";
    btn.style.left = Math.random() * window.innerWidth + "px";
}
</script>

</body>
</html>
