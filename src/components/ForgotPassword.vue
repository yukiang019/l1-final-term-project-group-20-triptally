<template>
    <div class="login-card"> <!-- Apply .login-card class here -->
      <h1>Forgot Password</h1>
      <text>Enter the email address associated with your account and click the button below to receive an email to reset this account’s password. </text>
      <form>
        <input type="email" placeholder="Enter Email" />
        <button type="submit">Reset My Password</button>
        <router-link to="/" class="go-login-link">← Back to Login.</router-link>
      </form>
    </div>
  </template>
  
<script>
  export default {
    name: 'ForgotPassword'
  }
</script>
  
<style>
/* Centered card layout */
.login-card {
  background: rgba(255, 255, 255, 0.7); /* semi-transparent white background */
  padding: 40px;
  border-radius: 15px;
  width: 600px; /* Adjust width as needed */
  margin: 0 auto; /* Center the card horizontally */
  position: relative;
  top: 50%; /* Push down by half the viewport height */
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3); /* subtle shadow */
  display: flex;
  flex-direction: column;
  align-items: center; /* Centers flex children horizontally */
  top: 60%; /* Adjust this value to control the vertical position */
  transform: translateY(50%);
}

/* Use a full-screen background image */
body, html {
  height: 100%;
  margin: 0;
  font-family: 'MontserratBold', Montserrat,sans-serif;
  background: url('src/assets/singapore.jpg') no-repeat center center fixed;
  background-size: cover;
}

/* Forgot password link */
.go-login-link {
  color: #16697A;
  position: absolute;
  left: 40px;
  bottom: 23px; /* Position it 20px above bottom of card */
  text-decoration: underline;
  font-size: medium;
}

button {
  width: 250px;
  padding: 15px;
  border: none;
  border-radius: 35px;
  background-color: #16697A;
  color: #EDE7E3;
  font-size:large;
  margin-top: 20px;
  font-weight: 600;
}

text {
  text-align: center;
  color: #7A7474;
  margin-top: 0px;
  margin-bottom: 25px;
  width: 70%;
  font-size: medium;
}

h1 {
  text-align: center;
  color: #16697a;
  margin-bottom: 40px;
}

</style>
  