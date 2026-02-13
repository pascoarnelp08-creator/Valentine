# Valentine
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Be My Valentine 💘</title>

<style>
body {
    text-align: center;
    font-family: Arial, sans-serif;
    background-color: #ffe6f0;
    padding-top: 100px;
}

h1 {
    color: #d63384;
    font-size: 40px;
}

button {
    padding: 15px 30px;
    font-size: 20px;
    margin: 20px;
    border: none;
    border-radius: 10px;
    cursor: pointer;
}

#yesBtn {
    background-color: #ff4d6d;
    color: white;
}

#noBtn {
    background-color: #999;
    color: white;
    position: absolute;
}
</style>
</head>

<body>

<h1>Ma. Ida, will you be my Valentine? 💖</h1>

<button id="yesBtn" onclick="sayYes()">YES 💕</button>
<button id="noBtn" onmouseover="moveNo()">NO 😢</button>

<script>
function sayYes() {
    document.body.innerHTML = "<h1>Yaaay! 💖 I can't wait for our date! 🌹</h1>";
}

function moveNo() {
    let x = Math.random() * (window.innerWidth - 100);
    let y = Math.random() * (window.innerHeight - 100);
    document.getElementById("noBtn").style.left = x + "px";
    document.getElementById("noBtn").style.top = y + "px";
}
</script>

</body>
</html>