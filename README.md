<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title> Will You Be My Valentine?</title>
    <style>
        body {
            background-color: #ffe6f2;
            color: #ff3366;
            font-family: 'Arial', sans-serif;
            text-align: center;
            padding: 50px;
        }
        h1 {
            font-size: 40px;
        }
        button {
            background-color: #ff3366;
            color: white;
            border: none;
            padding: 15px 30px;
            font-size: 20px;
            cursor: pointer;
            margin: 10px;
        }
        button:hover {
            background-color: #ff6699;
        }
    </style>
</head>
<body>
    <h1>Hi, MJ. Will You Be My Valentine?</h1>
    <button id="yesButton">Yes</button>
    <button id="noButton">No</button>

    <p id="response" style="font-size: 24px; margin-top: 20px;"></p>

    <script>
        document.getElementById('yesButton').onclick = function() {
            document.getElementById('response').innerText = "Yay! I'm so happy! ❤️";
        };

        document.getElementById('noButton').onclick = function() {
            document.getElementById('response').innerText = "Oh no! Are you sure? 😢";
            setTimeout(() => {
                document.getElementById('response').innerText = "You're breaking my heart! 💔";
            }, 2000);
        };
    </script>
</body>
</html>
