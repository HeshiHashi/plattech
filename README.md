
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My GitHub Pages Test</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            background: #f4f4f9;
            color: #333;
        }

        nav {
            background: #24292e;
            color: white;
            padding: 20px 10%;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        nav a {
            color: white;
            text-decoration: none;
            margin-left: 20px;
        }

        header {
            text-align: center;
            padding: 100px 20px;
            background: #0969da;
            color: white;
        }

        header h1 {
            font-size: 42px;
            margin-bottom: 15px;
        }

        header p {
            margin-bottom: 25px;
        }

        button {
            padding: 12px 25px;
            border: none;
            border-radius: 6px;
            cursor: pointer;
            background: white;
            color: #0969da;
            font-weight: bold;
        }

        button:hover {
            background: #ddd;
        }

        main {
            text-align: center;
            padding: 60px 20px;
        }

        .card {
            background: white;
            padding: 30px;
            max-width: 400px;
            margin: 25px auto;
            border-radius: 10px;
            box-shadow: 0 3px 10px #0001;
        }

        footer {
            text-align: center;
            padding: 25px;
            background: #24292e;
            color: white;
            margin-top: 50px;
        }
    </style>
</head>
<body>

    <nav>
        <h2>My Test Site</h2>
        <div>
            <a href="#home">Home</a>
            <a href="#about">About</a>
        </div>
    </nav>

    <header id="home">
        <h1>It Works!</h1>
        <p>Welcome to my first GitHub Pages website.</p>
        <button onclick="showMessage()">Click Me</button>
    </header>

    <main id="about">
        <h2>GitHub Pages Test</h2>

        <div class="card">
            <h3>Website Status</h3>
            <p style="color: green; margin: 15px 0;">
                ● Website is running!
            </p>
            <p>Clicks: <span id="counter">0</span></p>
            <button onclick="countClick()">Test Counter</button>
        </div>
    </main>

    <footer>
        <p>Hosted with GitHub Pages</p>
    </footer>

    <script>
        let clicks = 0;

        function showMessage() {
            alert("GitHub Pages is working!");
        }

        function countClick() {
            clicks++;
            document.getElementById("counter").textContent = clicks;
        }
    </script>

</body>
</html>
