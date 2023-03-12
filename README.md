<!DOCTYPE html>
<html>
<head>
  <title>Form Validation Demo</title>
  <style>
    .form-group {
      display: flex;
      flex-direction: column;
      margin-bottom: 10px;
    }

    label {
      font-weight: bold;
    }

    .error-message {
      color: red;
      font-size: 14px;
      margin-top: 5px;
      display: none;
    }

     .form-control {
      width: 50%;
    }
  </style>
</head>
<body>

  <h1>Registration Form</h1>

  <form>
    <div class="form-group">
      <label for="username">Username:</label>
      <input type="text" id="username" name="username" class="form-control" />
      <span class="error-message" id="username-error"></span>
    </div>

    <div class="form-group">
      <label for="password">Password:</label>
      <input type="password" id="password" name="password" class="form-control" />
      <span class="error-message" id="password-error"></span>
    </div>

    <button type="submit">Submit</button>
  </form>

  <script>
    const usernameInput = document.getElementById("username");
    const passwordInput = document.getElementById("password");
    const usernameError = document.getElementById("username-error");
    const passwordError = document.getElementById("password-error");

    usernameInput.addEventListener("input", function() {
      if (usernameInput.value.length < 😎 {
        usernameError.textContent = "Username must be at least 8 characters";
        usernameError.style.display = "block";
      } else {
        usernameError.style.display = "none";
      }
    });

    passwordInput.addEventListener("input", function() {
      if (passwordInput.value.length < 😎 {
        passwordError.textContent = "Password must be at least 8 characters";
        passwordError.style.display = "block";
      } else {
        passwordError.style.display = "none";
      }
    });
  </script>

</body>
</html>
