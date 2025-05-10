 <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Shania Tiongson's Professional Website</title>
    <link rel="stylesheet" href="styles.css">
    <style>
        body {
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background: linear-gradient(135deg, #ff99cc, #ff66b2, #ffb3e6, #ff80d5);
            color: #fff;
            font-family: 'Arial', sans-serif;
            text-align: center;
        }
        .home-button {
            position: absolute;
            top: 10px;
            left: 10px;
            padding: 10px;
            background: linear-gradient(135deg, #ffd1dc, #ffdde1);
            border-radius: 5px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }
        .home-button a {
            text-decoration: none;
            color: #ff69b4;
            font-weight: bold;
        }
        h1 {
            font-size: 2.5em;
            color: #dda0dd;
            text-shadow: 2px 2px 5px #ba55d3;
        }
        .name {
            font-size: 3em;
            font-weight: bold;
            font-family: 'Pacifico', cursive;
            color: #ffb6c1;
            text-shadow: 3px 3px 10px #ff69b4;
        }
        .intro, .certificates {
            margin-top: 20px;
            padding: 20px;
            background: linear-gradient(135deg, #fbc2eb, #a6c1ee);
            border-radius: 10px;
            font-family: 'Courier New', monospace;
            color: #333;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            display: none;
        }
        .folder {
            margin: 20px auto;
            padding: 15px;
            background: linear-gradient(135deg, #ffccf9, #ffb3ff);
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            cursor: pointer;
            color: #fff;
            font-weight: bold;
            text-align: center;
            width: 250px;
            transition: transform 0.2s, background 0.3s;
        }
        .folder:hover {
            background: #ff99ff;
            transform: scale(1.05);
        }
        .folder:active {
            background: #ff66cc;
        }
        button {
            margin-top: 20px;
            padding: 10px 20px;
            font-size: 1.2em;
            background: linear-gradient(135deg, #e6ccff, #d9b3ff);
            border: none;
            border-radius: 5px;
            cursor: pointer;
            color: #fff;
            transition: background 0.3s;
        }
        button:hover {
            background: #c799ff;
        }
    </style>
</head>
<body>
    <div class="home-button">
        <a href="#">Home</a>
    </div>
    <div>
        <h1>Welcome to My Professional Website</h1>
        <div class="name">Hi! I'm Shania Tiongson</div>
        <button onclick="toggleIntro()">Click Here To Know Me Well</button>
        <div class="intro" id="intro">
            <p>Hello! I’m Shania, an IT student passionate about technology and learning new things. I’m exploring the world of web development, eager to build beautiful and functional websites. I love coding, problem-solving, and constantly improving my skills to become a well-rounded tech professional. Let’s create something amazing together!</p>
            <button onclick="showCertificates()">Click Here to See My Certificates</button>
            <div class="certificates" id="certificates">
                <p>Here are my certificates!</p>
                <div class="folder" onclick="window.open('https://www.sololearn.com/certificates/CC-XGK6KBUV', '_blank')">Certificate in HTML</div>
                <div class="folder" onclick="window.open('https://www.sololearn.com/certificates/CC-YMECIW7R', '_blank')">Certificate in CSS</div>
                <div class="folder" onclick="window.open('https://www.sololearn.com/certificates/CC-MNWVRXJF', '_blank')">Certificate in JavaScript</div>
                <div class="folder" onclick="window.open('https://www.sololearn.com/certificates/CC-TCKUMUMB', '_blank')">Certificate in Python</div>
                <div class="folder" onclick="window.open('https://www.sololearn.com/certificates/CC-A2WRLTU9', '_blank')">Certificate in C</div>
            </div>
        </div>
    </div>

    <script>
        function toggleIntro() {
            const intro = document.getElementById('intro');
            intro.style.display = intro.style.display === 'none' || intro.style.display === '' ? 'block' : 'none';
        }
        
        function showCertificates() {
            const certificates = document.getElementById('certificates');
            certificates.style.display = certificates.style.display === 'none' || certificates.style.display === '' ? 'block' : 'none';
        }
    </script>
</body>
</html>
