<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AK47</title>
</head>
<style>
        body {
            margin: 0%;
            background-image: radial-gradient(circle , #e48cce, #f1cae8);
            background-repeat: no-repeat;
            background-attachment: fixed;

            


            
        }
        .heart {
            position: absolute;
            font-size: 1.5rem;
            opacity: 0.7;
            pointer-events: none;
            user-select: none;
            animation: sparkle 2s infinite alternate;
        }
        @keyframes sparkle {
            0% {transform: scale(1) rotate(0deg);}
            100% {transform: scale(1.2) rotate(15deg);}
        }
       
        h1 {
            text-align: center;
            font-size: 300%;
            font-style: italic;
            font-variant: initial;
            text-decoration: underline wavy rgb(245, 165, 219);
            text-decoration: double;

            image-orientation: from-image;
        
        }
        .abhi {
            animation: colorchange 5s infinite;
        }
        @keyframes colorchange {
        0% {color: aliceblue;}
        50% {color: #f1cae8;}
        100% {color: #11010d;}
        }
    .thank-you-box {
        position: fixed;
        bottom: 0;
        left: 0;
        width: 100%;
        background-color: rgba(0, 0, 0, 0.8); /* Semi-transparent black */
        color: white;
        text-align: center;
        padding: 15px;
        font-size: 20px;
        font-family: Arial, sans-serif;
        box-shadow: 0 -2px 10px rgba(0, 0, 0, 0.3);
    }

    /* Optional: Add a nice fade animation to the text */
    .thank-you-text {
        animation: fadeInOut 2s infinite;
    }

    @keyframes fadeInOut {
        0%, 100% { opacity: 0.8; }
        50% { opacity: 1; }
    }    
    #password-overlay {
            position: fixed;
            top: 0; left: 0;
            width: 100vw; height: 100vh;
            background: rgba(0,0,0,0.85);
            display: flex;
            align-items: center;
            justify-content: center;
            z-index: 9999;
        }
        #password-form {
            background: #222;
            padding: 30px 40px;
            border-radius: 10px;
            box-shadow: 0 0 20px #000;
            text-align: center;
        }
        #password-form input[type="password"] {
            padding: 10px;
            font-size: 1rem;
            border-radius: 5px;
            border: none;
            margin-bottom: 10px;
        }
        #password-form button {
            padding: 10px 20px;
            font-size: 1rem;
            border-radius: 5px;
            border: none;
            background: #1E90FF;
            color: #fff;
            cursor: pointer;
        }
        #password-error {
            color: #ff6b6b;
            margin-top: 10px;
            min-height: 20px;
        }
        
</style>
<body>
<h1>
    <span class="abhi">My Family!!!</span>
</h1>
<span class="heart" style="top: 10%; left: 20%;">💖</span>
<span class="heart" style="top: 30%; left: 70%;">💖</span>
<span class="heart" style="top: 60%; left: 40%;">💖</span>
<span class="heart" style="top: 80%; left: 80%;">💖</span>
<span class="heart" style="top: 70%; left: 10%;">💖</span>
<span class="heart" style="top: 80%; left: 40%;">💖</span>
<span class="heart" style="top: 90%; left: 50%;">💖</span>
<span class="heart" style="top: 10%; left: 20%;">💖</span>
<span class="heart" style="top: 10%; left: 10%;">💖</span>
<span class="heart" style="top: 60%; left: 60%;">💖</span>
<span class="heart" style="top: 60%; left: 40%;">💖</span>
<span class="heart" style="top: 50%; left: 60%;">💖</span>
<span class="heart" style="top: 25%; left: 80%;">💕</span>
<span class="heart" style="top: 50%; left: 50%;">💕</span>
<span class="heart" style="top: 20%; left: 30%;">💕</span>
<span class="heart" style="top: 10%; left: 90%;">💕</span>

<img src="abhik.jpg" alt="The Authors Of My Life" width="400" height="225" style="display: block;margin:0% auto;">
<h2>
    <img src="abhikk.gif" alt="cat" width="50" height="40" style="display: block;margin: 0% auto;">
</h2>
<div class="thank-you-box">
        <span class="thank-you-text">Thank You For Visiting My Page...😘</span>
    </div>
<div id="password-overlay">
        <form id="password-form" onsubmit="return false;">
            <h2 style="color:white;">Enter Password to Access</h2>
            <input type="password" id="password-input" placeholder="Password" autofocus>
            <br>
            <button onclick="checkPassword()">Unlock</button>
            <div id="password-error"></div>
        </form>
</div>
<script>
        // Change this to your desired password
        const CORRECT_PASSWORD = "abhi";

        function checkPassword() {
            const input = document.getElementById('password-input').value;
            const errorDiv = document.getElementById('password-error');
            if (input === CORRECT_PASSWORD) {
                document.getElementById('password-overlay').style.display = 'none';
                document.getElementById('protected-content').style.display = 'block';
            } else {
                errorDiv.textContent = "Incorrect password. Try again.";
                document.getElementById('password-input').value = "";
            }
        }

        // Allow pressing Enter to submit
        document.getElementById('password-input').addEventListener('keydown', function(e) {
            if (e.key === 'Enter') {
                checkPassword();
            }
        });
    </script>
</body>
</html>
