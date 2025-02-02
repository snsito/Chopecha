<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>San Valentín</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #ffcccc;
            font-family: Arial, sans-serif;
            flex-direction: column;
            margin: 0;
            overflow: hidden;
        }
        .container {
            text-align: center;
            background: white;
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.2);
            max-width: 80%;
        }
        button {
            margin: 10px;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 18px;
        }
        #yes {
            background-color: #ff6699;
            color: white;
        }
        #no {
            background-color: #666;
            color: white;
            position: absolute;
        }
        #linkButton {
            background-color: #ff3300;
            color: white;
            display: none;
            text-decoration: none;
            padding: 10px 20px;
            border-radius: 5px;
        }
        #extraContent {
            display: none;
            text-align: center;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h2>¿Quieres ser mi San Valentín?</h2>
        <button id="yes" onclick="showLink()">Sí</button>
        <button id="no" onmouseover="moveNoButton()" ontouchstart="moveNoButton()">No</button>
    </div>
    <div id="extraContent">
        <div style="position: relative; width: 100%; height: 0; padding-top: 177.7778%;
         padding-bottom: 0; box-shadow: 0 2px 8px 0 rgba(63,69,81,0.16); margin-top: 1.6em; margin-bottom: 0.9em; overflow: hidden;
         border-radius: 8px; will-change: transform;">
          <iframe loading="lazy" style="position: absolute; width: 100%; height: 100%; top: 0; left: 0; border: none; padding: 0;margin: 0;"
            src="https://www.canva.com/design/DAGd7NG4EmA/fhv6Pn2JAJ0qyTBH7Bo5YQ/view?embed" allowfullscreen="allowfullscreen" allow="fullscreen">
          </iframe>
        </div>
        <a href="https://www.canva.com/design/DAGd7NG4EmA/fhv6Pn2JAJ0qyTBH7Bo5YQ/view?utm_content=DAGd7NG4EmA&amp;utm_campaign=designshare&amp;utm_medium=embeds&amp;utm_source=link" target="_blank" rel="noopener">un dia nos conocimos...</a> de sean uwu
    </div>

    <script>
        function moveNoButton() {
            let noButton = document.getElementById("no");
            let x = Math.random() * (window.innerWidth - 100);
            let y = Math.random() * (window.innerHeight - 50);
            noButton.style.left = x + "px";
            noButton.style.top = y + "px";
        }
        
        function showLink() {
            let extraContent = document.getElementById("extraContent");
            extraContent.style.display = "block";
        }
    </script>
</body>
</html>
