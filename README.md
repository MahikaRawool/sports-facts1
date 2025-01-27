# sports-facts1
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sports Facts</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }

        .container {
            text-align: center;
            background: white;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        button {
            padding: 10px 20px;
            font-size: 16px;
            border: none;
            border-radius: 5px;
            background-color: #007BFF;
            color: white;
            cursor: pointer;
        }

        button:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Random Sports Fact</h1>
        <p id="fact">Press the button to see a fact!</p>
        <button id="factButton">Show Fact</button>
    </div>
    <script>
        const facts = [
            "The earliest recorded sports date back to ancient civilizations.",
            "Soccer (football) is the most popular sport in the world.",
            "The modern Olympic Games were revived in 1896 in Athens, Greece.",
            "Basketball was invented in 1891 by Dr. James Naismith.",
            "The longest tennis match in history lasted 11 hours and 5 minutes.",
            "Baseball's origins can be traced back to bat-and-ball games in England.",
            "The fastest recorded animal is the peregrine falcon.",
            "The World Series in baseball has been held annually since 1903.",
            "Extreme sports have gained popularity since the late 20th century.",
            "Women's sports have gained significant recognition over the past few decades."
        ];

        const factButton = document.getElementById('factButton');
        const factDisplay = document.getElementById('fact');

        factButton.addEventListener('click', () => {
            const randomIndex = Math.floor(Math.random() * facts.length);
            factDisplay.textContent = facts[randomIndex];
        });
    </script>
</body>
</html>
