<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Login</title>
    <link rel="stylesheet" href="css/stylesheet.css">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-T3c6CoIi6uLrA9TneNEoa7RxnatzjcDSCmG1MXxSR1GAsXEV/Dwwykc2MPK8M2HN" crossorigin="anonymous">
</head>
<body>
    <nav class="navbar navbar-expand-lg bg-primary-subtle border-bottom border-body fixed-top" data-bs-theme="light">
        <div class="container">
            <a class="navbar-brand ms-5" href="#"><img src="https://s0.hfdstatic.com/sites/the_hartford/img/logo.svg" alt="logo" width="40" height="40">The Hartford</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                    <li class="nav-item">
                        <a class="nav-link active" aria-current="page" href="#">Home</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Login</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
    <div class="container border shadow-lg custom-top-margin">
        <div class="row text-center mt-3 ">
            <form id="loginForm">
                <div>
                    <label for="username"></label>
                    <input type="text" name="username" placeholder="Username" class="w-100-sm w-25-other text-center fs-4" id="username">
                </div>
            </form>
        </div>
        <div class="row text-center mt-3 ">
            <form>
                <div>
                    <label for="password"></label>
                    <input type="password" name="password" placeholder="Password" class="w-100-sm w-25-other text-center fs-4" id="password">
                </div>
            </form>
        </div>
        <div class="row text-center my-3">
            <form>
                <div>
                    <label for="login"></label>
                    <input type="button" name="login-button" value="Login" class="w-25-sm w-15-other text-center fs-4 mb" id="login" onclick="validateLogin()">
                </div>
            </form>
        </div>
    </div>
     <script>
        function validateLogin() {
            var username = document.getElementById("username").value;
            var password = document.getElementById("password").value;

            // Check the login credentials
            if (username === "Riley" && password === "password") {
                // If Riley logs in, navigate to Riley's page
                window.location.href = "riley_page.html";
            } else if (username === "Admin" && password === "1234") {
                // If Admin logs in, navigate to Admin's page
                window.location.href = "admin_page.html";
            } else {
                // Display an error message (you can customize this part)
                alert("Invalid username or password. Please try again.");
            }
        }
    </script>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-C6RzsynM9kWDrMNeT87bh95OGNyZPhcTNXj1NW7RuBCsyN/o0jlpcV8Qyq46cDfL" crossorigin="anonymous"></script>
    <script src="https://cdn.jsdelivr.net/npm/jquery@3.7.1/dist/jquery.min.js"></script>
    <script src="js/hartfordjs.js"></script>

  
</body>
</html>
