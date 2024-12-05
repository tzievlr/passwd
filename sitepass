<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Enregistrement et vérification du mot de passe</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
        }
        .form-section {
            margin-bottom: 20px;
        }
        .form-section label {
            display: block;
            margin-bottom: 8px;
        }
        .form-section input {
            padding: 10px;
            width: 100%;
            box-sizing: border-box;
        }
        .form-section button {
            margin-top: 10px;
            padding: 10px 20px;
            background-color: #007BFF;
            color: white;
            border: none;
            cursor: pointer;
        }
        .form-section button:hover {
            background-color: #0056b3;
        }
        .message {
            margin-top: 10px;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <h1>Enregistrement et vérification du mot de passe</h1>

    <!-- Section d'enregistrement -->
    <div class="form-section">
        <label for="set-password">Entrez un mot de passe à enregistrer :</label>
        <input type="password" id="set-password" placeholder="Saisissez votre mot de passe">
        <button onclick="savePassword()">Enregistrer le mot de passe</button>
        <div id="save-message" class="message"></div>
    </div>

    <!-- Section de vérification -->
    <div class="form-section">
        <label for="verify-password">Ressaisissez votre mot de passe :</label>
        <input type="password" id="verify-password" placeholder="Ressaisissez votre mot de passe">
        <button onclick="verifyPassword()">Vérifier le mot de passe</button>
        <div id="verify-message" class="message"></div>
    </div>

    <script>
        let savedPassword = ""; // Variable pour stocker temporairement le mot de passe

        // Fonction pour enregistrer le mot de passe
        function savePassword() {
            const passwordInput = document.getElementById("set-password").value;
            if (passwordInput) {
                savedPassword = passwordInput; // Stocke le mot de passe
                document.getElementById("save-message").textContent = "Mot de passe enregistré avec succès !";
                document.getElementById("save-message").style.color = "green";
            } else {
                document.getElementById("save-message").textContent = "Veuillez entrer un mot de passe valide.";
                document.getElementById("save-message").style.color = "red";
            }
        }

        // Fonction pour vérifier le mot de passe
        function verifyPassword() {
            const passwordInput = document.getElementById("verify-password").value;
            if (passwordInput === savedPassword) {
                document.getElementById("verify-message").textContent = "Mot de passe correct !";
                document.getElementById("verify-message").style.color = "green";
            } else {
                document.getElementById("verify-message").textContent = "Mot de passe incorrect.";
                document.getElementById("verify-message").style.color = "red";
            }
        }
    </script>
</body>
</html>
