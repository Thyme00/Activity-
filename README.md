#Die Randomizer 
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Die Randomizer</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #f4f4f4;
            font-family: Arial, sans-serif;
        }
        .container {
            text-align: center;
        }
        .die {
            width: 100px;
            height: 100px;
            background-color: #fff;
            border: 2px solid #333;
            border-radius: 10px;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 2em;
            margin-bottom: 20px;
        }
        button {
            padding: 10px 20px;
            font-size: 1em;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="die" id="die">1</div>
        <button id="rollButton">Roll the Die</button>
    </div>
    <script>
        document.getElementById('rollButton').addEventListener('click', function() {
            const randomNumber = Math.floor(Math.random() * 6) + 1;
            document.getElementById('die').textContent = randomNumber;
        });
    </script>
</body>
</html>
