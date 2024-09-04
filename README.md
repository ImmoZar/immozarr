<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Page Web Mobile</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        body {
            margin: 0;
            padding: 0;
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
        }
        .header {
            background-color: white;
            padding: 0;
            display: flex;
            align-items: center;
            justify-content: space-between;
            position: relative;
        }
        .header img {
            width: 100%;
            height: auto;
        }
        .header .menu-icon {
            position: absolute;
            top: 10px;
            right: 20px;
            font-size: 1.5em;
            color: #007bff;
            z-index: 1000;
            cursor: pointer;
        }
        .menu {
            display: none;
            flex-direction: column;
            position: absolute;
            top: 50px;
            right: 20px;
            width: 50%;
            height: 50vh;
            background-color: #003366;
            box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);
            z-index: 1000;
            border-radius: 10px;
            overflow: hidden;
        }
        .menu.show {
            display: flex;
        }
        .menu a {
            text-decoration: none;
            color: white;
            padding: 10px 20px;
            border-bottom: 1px solid #002244;
            display: block;
        }
        .menu a:hover {
            background-color: #004080;
        }
        .menu a:last-child {
            border-bottom: none;
        }
        .menu .english-link {
            display: flex;
            align-items: center;
            padding: 10px 20px;
        }
        .menu .english-link img {
            width: 20px;
            height: auto;
            margin-left: 10px;
        }
        .content {
            position: relative;
            width: 100%;
            overflow: hidden;
        }
        .content img.background {
            width: 100%;
            height: auto;
        }
        .animated-image {
            width: 100%;
            height: auto;
            display: block;
        }
        .button-container {
            position: absolute;
            bottom: 20px;
            left: 50%;
            transform: translateX(-50%);
        }
        .button-container a {
            display: inline-block;
            padding: 10px 20px;
            background-color: #007bff;
            color: white;
            text-decoration: none;
            font-size: 1.2em;
            border-radius: 5px;
        }
    </style>
</head>
<body>
    <div class="header">
        <img src="https://i.ibb.co/RSp1mzF/Screenshot-20240903-134513.png" alt="Header Image">
        <i class="fas fa-bars menu-icon" onclick="toggleMenu()"></i>
        <div id="menu" class="menu">
            <a href="#se-connecter">Se connecter</a>
            <a href="#immozar">ImmoZar</a>
            <a href="#nos-valeurs">Nos valeurs</a>
            <a href="#nos-services">Nos services</a>
            <a href="#reservation">Réservation</a>
            <a href="#contact">Contact</a>
            <a href="#se-deconnecter">Se déconnecter</a>
            <a href="#english" class="english-link">English
                <img src="https://i.ibb.co/rxNB0DG/Flag-of-the-United-Kingdom.png" alt="British Flag">
            </a>
        </div>
    </div>
    <div class="content">
        <img class="animated-image" src="https://media.giphy.com/media/03L4IdniGVFHFT8iOn/giphy.gif" alt="Animated Image">
        <img class="background" src="https://via.placeholder.com/500x800" alt="Background Image">
        <div class="button-container">
            <a href="#">About us <i class="fas fa-chevron-right"></i></a>
        </div>
    </div>
    <script>
        function toggleMenu() {
            var menu = document.getElementById("menu");
            menu.classList.toggle("show");
        }
    </script>
</body>
</html>
