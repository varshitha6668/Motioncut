<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <style>
      :root {
        --primary-color: #fead53;
        --text-dark: #333333;
        --text-light: #ffffff33;
        --extra-light: #f3f4f6;
        --max-width: 1300px;
      }

      * {
        padding: 0;
        margin: 0;
        box-sizing: border-box;
      }

      a {
        text-decoration: none;
      }

      input::placeholder {
        color: var(--text-dark); 
      }

      body {
        font-family: "Open Sans", sans-serif;
        min-height: 100vh;
        background-image: linear-gradient(
            rgba(0, 0, 0, 0.25),
            rgba(0, 0, 0, 0.25)
          ),
          url("download.jpg");
        background-position: center center;
        background-size: cover;
        background-repeat: no-repeat;
        display: flex;
        justify-content: center;
        align-items: center;
      }

      .container {
        display: flex;
        max-width: var(--max-width);
        margin: auto;
        padding: 2rem;
        position: relative;
      }

      .container__center {
        display: flex;
        justify-content: center;
        align-items: center;
        width: 100%;
      }

      form {
        width: 350px;
        display: grid;
        border-radius: 5px;
        background-color: var(--text-light);
        color: var(--extra-light);
        padding: 2rem;
      }

      form h4 {
        font-size: 1.2rem;
        font-weight: 600;
        margin-bottom: 1rem;
        color: #000000;
        text-align: center;
      }

      .logo {
        display: flex;
        justify-content: center;
        margin-bottom: 1rem;
      }

      .logo img {
        width: 100px;
        height: auto;
      }

      .form__group {
        display: grid;
        margin-bottom: 1rem;
      }

      .form__group label {
        display: none; 
      }

      .form__group input {
        padding: 0.5rem;
        font-size: 1rem;
        color: var(--text-dark);
        background-color: #FFE5EC;
        outline: none;
        border: 1px solid var(--extra-light);
        border-radius: 5px;
      }

      .form__group input:last-child {
        margin-bottom: 0;
      }

      .form__button-group {
        display: flex;
        flex-direction: column;
        align-items: center;
        margin-top: 1rem;
      }

      .form__button-group button {
        width: 100%;
        padding: 1rem;
        font-size: 1rem;
        font-weight: 600;
        outline: none;
        border: none;
        border-radius: 5px;
        background-color: #FFB3C6;
        color: var(--extra-light);
        cursor: pointer;
      }

      .button-group {
        display: flex;
        justify-content: space-between;
        margin-top: 1rem;
      }

      .button-group button {
        background: none;
        border: none;
        font-size: 0.9rem;
        font-weight: 600;
        color: var(--text-dark);
        cursor: pointer;
        display: flex;
        align-items: center;
        justify-content: center;
      }

      .button-group button img {
        margin-right: 0.5rem;
      }

      .button-group button:focus {
        text-decoration: underline;
      }

      .bottom__tracker {
        position: absolute;
        bottom: 2rem;
        left: 50%;
        transform: translateX(-50%);
        display: flex;
        gap: 1rem;
      }

      .bottom__tracker span {
        display: inline-block;
        height: 4px;
        width: 100px;
        background-color: var(--text-light);
      }

      .bottom__tracker span:nth-child(2) {
        background-color: var(--extra-light);
      }
    </style>
  </head>
  <body>
    <div class="container">
      <div class="container__center">
        <form>
          <div class="logo">
            <a href="#signup-button">
                         </a>
          </div>
          <h4>Sign In</h4>
          <div class="form__group">
            <input type="text" name="Username" id="Username" placeholder="Username" />
          </div>
          <div class="form__group">
            <input type="password" name="Password" id="Password" placeholder="Password" />
          </div>
          <div class="form__button-group">
            <button type="button">Login</button>
          </div>
          <div class="button-group">
            <button type="button">
             Forget Password
            </button>
            <button type="button" id="signup-button">
              Signup
            </button>
          </div>
        </form>
      </div>
    </div>
  </body>
</html>
