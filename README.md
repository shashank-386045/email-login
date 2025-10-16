## email login using HTML and CSS
## aim:
using the coding languages HTML and CSS to create a email web page login
## algorithm:
Set up the HTML structure: Begin the document as an HTML file and define the character encoding and viewport for responsiveness.

Add a descriptive title: The browser tab displays the form's title using the <title> tag.

Link external CSS: Reference an external CSS file (style.css) to style the login form components.

Create a section container: Use the <section> tag to wrap the login form and help with layout and styling.

Build the login box: Create a <div> with the class login-box to contain and center the login form on the page.

Construct the form: Inside the login box, use a <form> element to group input fields and controls for user authentication.

Construct the form: Inside the login box, use a <form> element to group input fields and controls for user authentication.

Design input fields: Add form fields for the user to enter their email and password, each inside a .input-box div for styling, with an associated icon and label.

Add remember and forgot controls: Include a 'Remember me' checkbox and a 'Forgot Password?' link for user convenience and account recovery.

Insert the login and register controls: Place a 'Login' button for form submission and a link underneath for users to register if they do not have an account.

Include icon scripts: Load the Ionicons JavaScript libraries at the bottom so the icon components render properly within input boxes.

## program:
##   HTML

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Animated Login form using HTML CSS only | codehal</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <section>
    <div class="login-box">
        <form action="">
            <h2>Login</h2>
            <div class="input-box">
                <span class="icon"><ion-icon name="mail"></ion-icon></span>
                <input type="email" required>
                <label>Email</label>
            </div>
                <div class="input-box">
                <span class="icon"><ion-icon name="lock-closed"></ion-icon></span>
                <input type="password" required>
                <label>password</label>

            </div>
            <div class="remember-forgot">
                <label><input type="checkbox">Remember me</label>
                <a href="#">Forgot Password?</a>
            <div>
                <button type="submit" class="btn">Login</button>
                <div class="register-link">
                    <p>Don't have an account? <a href="#">Register</a></p>
            </div>
        </form>
    </div>
</section>
    <script type="module" src="https://unpkg.com/ionicons@7.1.0/dist/ionicons/ionicons.esm.js"></script>
    <script nomodule src="https://unpkg.com/ionicons@7.1.0/dist/ionicons/ionicons.js"></script>
    
</body>
</html>
```
## CSS
```
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400;500;600;700&display=swap');
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'times new roman', sans-serif;
}
section{
    display:flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    height: 100vh;
    background: url('Screenshot\ 2025-10-02\ 161013.png')no-repeat;
    background-size: cover;
    background-position: center;

}
.login-box{
    position: relative;
    width: 400px;
    height: 450px;
    background: transparent;
    border: 2px solid rgba(255,255,255,.5);
    border-radius: 20px;
    align-items: center;
    justify-content: center;
    display: flex;
    backdrop-filter: blur(15px);
    
    
}
.login-box h2{
    position: relative;
    color: #4070f4;
    text-align: center;
    text-transform: uppercase;
    margin-bottom: 30px;
}
.input-box{
    position: relative;
    width: 100%;
    margin: 30px;  
    border-bottom:  2px solid #0a0400;
}
.input-box label{
    position: absolute;
    top: 50%;
    left: 5px;
    color: #333;
    transform: translateY(-50%);
    font-size: 16px;
    font-weight: 400;
    pointer-events: none;
    transition: .5s;
}
.input-box input:focus~label,
.input-box input:valid~label{
    top: -5px;

}
.input-box input{
    width: 100%;
    padding: 0 35px 0 5px;
    font-size: 16px;
    color: #000;
    margin-top: 10px;
    border: none;
    border-bottom: 2px solid #333;
    outline: none;
    background: transparent;
}
.input-box.icon{
    position: absolute;
    right: 8px;
    color:#000;
    font-size: 1.2em;
    line-height: 57px;
}
.remember-forgot{
    margin: -15px 0 15px;
    font-size: .9em;
    color: #000;
    display:flex;
    justify-content: space-between;
}
.remember-forgot label input{
    margin-right:5px;
}
.remember-forgot a{
    color:#000;
    text-decoration: none;
}
.remember-forgot a:hover{
    text-decoration: underline;
}
button{
    width:100%;
    height: 40px;
    background:#000;
    border: none;
    outline: none;
    border-radius: 40px;
    cursor: pointer;
    font-size: 1em;
    color: #fff;
    font-weight: 500;
}
.register-link{
    font-size: .9em;
    color:#fff;
    text-align:center;
    margin: 25px 0 10px;
}
.register-link p a{
    color: #000;
    text-decoration: none;
    font-weight: 600;
}
```
## output:
<img width="1917" height="919" alt="Screenshot 2025-10-16 191622" src="https://github.com/user-attachments/assets/b6bc84a3-e80e-47ca-9438-d75fcae32541" />

## result:
the above code gives a web page email login and code is executed successfully.
