# TikiBb
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Happy Birthday Tiki 💕</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            background: linear-gradient(135deg, #ff9a9e, #fad0c4);
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            font-family: 'Segoe UI', sans-serif;
            overflow: hidden;
        }

        .card {
            background: white;
            padding: 40px;
            border-radius: 20px;
            text-align: center;
            box-shadow: 0 10px 30px rgba(0,0,0,0.3);
            animation: pop 1.5s ease;
            max-width: 350px;
        }

        @keyframes pop {
            0% { transform: scale(0.5); opacity: 0; }
            100% { transform: scale(1); opacity: 1; }
        }

        h1 {
            color: #ff4081;
            font-size: 28px;
        }

        p {
            font-size: 16px;
            color: #444;
            margin-top: 15px;
        }

        .heart {
            position: absolute;
            color: red;
            font-size: 20px;
            animation: float 6s linear infinite;
        }

        @keyframes float {
            0% { transform: translateY(100vh); opacity: 1; }
            100% { transform: translateY(-10vh); opacity: 0; }
        }

        button {
            margin-top: 20px;
            padding: 12px 25px;
            background: #ff4081;
            border: none;
            border-radius: 25px;
            color: white;
            font-size: 16px;
            cursor: pointer;
        }

        button:hover {
            background: #e91e63;
        }
    </style>
</head>
<body>

<div class="card">
    <h1>🎂 Happy Birthday 🎂</h1>
    <h2>💫 tiki samantaray 💕</h2>
    <p>
        On this special day, I just want to remind you  
        how amazing, beautiful, and precious you are 💖  
        May your life be filled with happiness, love,  
        and endless smiles 🌸✨
    </p>
    <p>Forever grateful to have you 💞</p>
    <button onclick="alert('You are my favorite person 💕')">
        Click for Surprise 💝
    </button>
</div>

<script>
    function createHeart() {
        const heart = document.createElement("div");
        heart.classList.add("heart");
        heart.innerHTML = "❤️";
        heart.style.left = Math.random() * 100 + "vw";
        heart.style.animationDuration = (Math.random() * 3 + 3) + "s";
        document.body.appendChild(heart);

        setTimeout(() => {
            heart.remove();
        }, 6000);
    }

    setInterval(createHeart, 300);
</script>

</body>
</html>
