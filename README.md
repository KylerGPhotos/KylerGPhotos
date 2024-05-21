/* styles.css */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
    line-height: 1.6;
}

header {
    background-color: #333;
    color: white;
    padding: 20px 0;
    text-align: center;
}

nav {
    display: flex;
    justify-content: center;
    background-color: #444;
    padding: 10px 0;
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
    margin: 10px auto;
    max-width: 800px;
    background: #fff;
    border-radius: 8px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
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
    border-radius: 8px;
}

.portfolio img {
    max-width: 100%;
    height: auto;
    border: 5px solid #333;
    border-radius: 8px;
    margin-bottom: 20px;
}

.password-protected {
    max-width: 300px;
    margin: 20px auto;
    text-align: center;
    padding: 20px;
    background-color: #fff;
    border: 1px solid #ccc;
    border-radius: 8px;
}

.password-protected input[type="password"],
.password-protected input[type="submit"] {
    padding: 10px;
    margin: 10px 0;
    width: 100%;
    border-radius: 8px;
    border: 1px solid #ccc;
}

.password-protected input[type="submit"] {
    background-color: #444;
    color: white;
    border: none;
    cursor: pointer;
}

.password-protected input[type="submit"]:hover {
    background-color: #555;
}

.contact-info {
    text-align: center;
}

