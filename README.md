<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>KylerGPhotos - KGP</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        header {
            background-color: #333;
            color: white;
            padding: 10px 0;
            text-align: center;
        }
        nav {
            display: flex;
            justify-content: center;
            background-color: #444;
        }
        nav a {
            color: white;
            padding: 15px 20px;
            text-decoration: none;
            text-align: center;
        }
        nav a:hover {
            background-color: #555;
        }
        section {
            padding: 20px;
            margin: 10px 0;
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px 0;
        }
        .photo-of-the-week {
            display: flex;
            justify-content: space-around;
        }
        .photo-of-the-week img {
            max-width: 30%;
            height: auto;
            border: 5px solid #333;
        }
        .portfolio img {
            max-width: 100%;
            height: auto;
            border: 5px solid #333;
        }
        .password-protected {
            max-width: 300px;
            margin: 20px auto;
            text-align: center;
            padding: 20px;
            background-color: #fff;
            border: 1px solid #ccc;
        }
        .password-protected input[type="password"],
        .password-protected input[type="submit"] {
            padding: 10px;
            margin: 10px 0;
            width: 100%;
        }
        .password-protected input[type="submit"] {
            background-color: #444;
            color: white;
            border: none;
        }
        .contact-info {
            text-align: center;
        }
    </style>
</head>
<body>
    <header>
        <h1>KylerGPhotos - KGP</h1>
    </header>
    <nav>
        <a href="#home">Home</a>
        <a href="#portfolio">Portfolio</a>
        <a href="#clients">Clients</a>
        <a href="#contact">Contact</a>
    </nav>
    <section id="home">
        <h2>About Me</h2>
        <p>Hi, I'm Kyler from KylerGPhotos (KGP). I love taking photos and capturing moments. Hit me up at 918-884-4840 to get a shoot free until the fall!</p>
        <h3>Photo of the Week</h3>
        <div class="photo-of-the-week">
            <img src="photo1.jpg" alt="Photo of the Week 1">
            <img src="photo2.jpg" alt="Photo of the Week 2">
            <img src="photo3.jpg" alt="Photo of the Week 3">
        </div>
    </section>
    <section id="portfolio">
        <h2>Portfolio</h2>
        <img src="portfolio1.jpg" alt="Portfolio Photo 1">
        <img src="portfolio2.jpg" alt="Portfolio Photo 2">
        <img src="portfolio3.jpg" alt="Portfolio Photo 3">
    </section>
    <section id="clients">
        <h2>Clients</h2>
        <div class="password-protected">
            <form id="clientForm" onsubmit="return checkPassword();">
                <label for="password">Enter Password:</label>
                <input type="password" id="password" name="password" required>
                <input type="submit" value="Submit">
            </form>
            <div id="clientContent" style="display:none;">
                <p>Welcome to the client area. Here you can view and download your photos.</p>
                <!-- Add client-specific content here -->
            </div>
        </div>
    </section>
    <section id="contact">
        <h2>Contact</h2>
        <p class="contact-info">Phone: 918-884-4840</p>
        <p class="contact-info">Email: kylergphotos@example.com</p>
    </section>
    <footer>
        <p>&copy; 2024 KylerGPhotos. All rights reserved.</p>
    </footer>

    <script>
        function checkPassword() {
            var password = document.getElementById('password').value;
            if (password === 'yourpassword') {
                document.getElementById('clientContent').style.display = 'block';
                return false;
            } else {
                alert('Incorrect password. Please try again.');
                return false;
            }
        }
    </script>
</body>
</html>
