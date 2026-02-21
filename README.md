# homework
<!DOCTYPE html>
<html>
<head>
    <title>My Website</title>

    <style>
        body {
            margin: 0;
            font-family: Arial;
            background-color: #f4f4f4;
        }

        .menu {
            background-color: #333;
            padding: 15px;
            text-align: center;
        }

        .menu a {
            color: white;
            text-decoration: none;
            margin: 15px;
            font-size: 18px;
        }

        .menu a:hover {
            color: yellow;
        }

        .container {
            display: flex;
            height: 90vh;
        }

        .left {
            width: 50%;
            padding: 50px;
        }

        .right {
            width: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
        }

        .right img {
            width: 80%;
        }

        .btn {
            display: inline-block;
            margin-top: 20px;
            padding: 10px 20px;
            background-color: #333;
            color: white;
            text-decoration: none;
            cursor: pointer;
        }

        .btn:hover {
            background-color: #555;
        }

        .login-section {
            display: none;
            width: 300px;
            margin: 100px auto;
            padding: 30px;
            background: white;
            box-shadow: 0 0 10px gray;
        }

        .login-section input {
            width: 100%;
            padding: 8px;
            margin: 10px 0;
        }

        .login-section button {
            width: 100%;
            padding: 10px;
            background: #333;
            color: white;
            border: none;
            cursor: pointer;
        }

        .login-section button:hover {
            background: #555;
        }
    </style>

    <script>
        function showLogin() {
            document.querySelector(".container").style.display = "none";
            document.querySelector(".login-section").style.display = "block";
        }

        function showHome() {
            document.querySelector(".container").style.display = "flex";
            document.querySelector(".login-section").style.display = "none";
        }
    </script>

</head>

<body>

    <div class="menu">
        <a href="#" onclick="showHome()">Home</a>
        <a href="#" onclick="showLogin()">Login</a>
    </div>

    <!-- Home Section -->
    <div class="container">
        <div class="left">
            <h1>Welcome</h1>
            <p>This is my simple website.</p>
            <p>My name is Raghad Qwasmii</p>
            <div class="btn" onclick="showLogin()">Go to Login</div>
        </div>

        <div class="right">
            <img src="https://via.placeholder.com/300" alt="Image">
        </div>
    </div>

    <!-- Login Section -->
    <div class="login-section">
        <h2>Login</h2>

        <label>Username</label>
        <input type="text" placeholder="Enter username">

        <label>Password</label>
        <input type="password" placeholder="Enter password">

        <button>Login</button>
    </div>

</body>
</html>
