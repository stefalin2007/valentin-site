<!DOCTYPE html>
<html>
<head>
<title>Pentru tine ❤️</title>

<style>
body {
    background: linear-gradient(135deg, #ff9a9e, #fecfef);
    height: 100vh;
    margin: 0;
    font-family: Arial;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
}

.container {
    background: white;
    padding: 40px;
    border-radius: 20px;
    box-shadow: 0 0 20px rgba(0,0,0,0.2);
}

h1 {
    color: #ff4d6d;
}

button {
    font-size: 20px;
    padding: 12px 25px;
    margin: 10px;
    border: none;
    border-radius: 12px;
    cursor: pointer;
    position: relative;
}

#da {
    background-color: #ff4d6d;
    color: white;
}

#nu {
    background-color: gray;
    color: white;
    position: absolute;
}
</style>
</head>

<body>

<div class="container">
    <h1>Am o întrebare importantă ❤️</h1>
    <h2>Ana, vrei să fii partenera mea de Sfântul Valentin?</h2>

    <button id="da" onclick="raspunsDa()">DA ❤️</button>
    <button id="nu" onmouseover="fugi()">NU 😢</button>

    <p id="mesaj"></p>
</div>

<script>

function raspunsDa() {
    document.body.innerHTML = `
        <h1 style="color:white; font-size:40px;">
        ❤️ YEEEEEY ❤️<br>
        Te iubesc! Abia aștept Sfântul Valentin să ne vedem mâine!
        </h1>
    `;
    document.body.style.background = "#ff4d6d";
}

function fugi() {

    var button = document.getElementById("nu");

    var x = Math.random() * (window.innerWidth - 100);
    var y = Math.random() * (window.innerHeight - 50);

    button.style.left = x + "px";
    button.style.top = y + "px";
}

</script>

</body>
</html>
