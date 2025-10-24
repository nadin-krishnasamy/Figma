# Ex09 Event Registration Web Application
## Date:15/10/2025

## AIM:
To design, develop and deploy a web application for event registration.

## DESIGN STEPS:

### Step 1:
Create a new frame.

### Step 2:
Select any one preset size of your choice.

### Step 3:
Select the shapes you need.

### Step 4:
Import images as needed.

### Step 5:
Create pages based on your need and link them.

### Step 6:

Validate the HTML and CSS code.

### Step 6:

Publish the website in the given URL.

## DESIGN TOOL:
Figma

## CODE:
'''
<!-- PART 1: LOGIN/HOME SCREEN -->

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Sports Day Events - Login</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      background: linear-gradient(135deg, #9ef6e5 0%, #6b47dc 100%);
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      font-family: 'Montserrat', sans-serif;
    }
    .container {
      background: rgba(255,255,255,0.07);
      padding: 2em 1.5em;
      border-radius: 24px;
      box-shadow: 0 8px 40px rgba(94,63,186,0.16);
      text-align: center;
      width: 290px;
      position: relative;
    }
    .logo {
      width: 78px;
      margin-bottom: 10px;
    }
    h2 {
      font-size: 1.45em;
      color: #2e1c59;
      margin-bottom: 18px;
      margin-top: 10px;
      letter-spacing: 1px;
      font-weight: 800;
      text-shadow: 1px 2px 6px #f5c3ff36;
    }
    .btn {
      width: 100%;
      border: none;
      padding: 12px 0;
      font-size: 1em;
      border-radius: 8px;
      margin-top: 18px;
      background: #ff465b;
      color: #fff;
      cursor: pointer;
      font-weight: 700;
      letter-spacing: 0.8px;
      transition: background 0.2s;
    }
    .btn:nth-child(2) {
      background: #f2af29;
      color: #000;
      margin-top: 10px;
    }
    .bg-illustration {
      position: absolute;
      bottom: -16px;
      left: 0;
      right: 0;
      width: 100%;
      height: 80px;
      background: url('https://i.imgur.com/k7NBpK5.png') bottom center no-repeat;
      background-size: contain;
      pointer-events: none;
    }
  </style>
</head>
<body>
  <div class="container">
    <img class="logo" src="https://i.imgur.com/g8RHtH5.png" alt="Saveetha Engineering College Logo" />
    <h2>SPORTS DAY EVENTS</h2>
    <button class="btn">LOG IN</button>
    <button class="btn">REGISTER NOW</button>
    <div class="bg-illustration"></div>
  </div>
</body>
</html>

<!-- PART 2: EVENTS LIST SCREEN -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Sports Day - Select Event</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      background: linear-gradient(120deg, #0fa3b1 0%, #f4a259 100%);
      display: flex;
      justify-content: center;
      align-items: center;
      font-family: 'Montserrat', sans-serif;
    }
    .container {
      background: rgba(255,255,255,0.09);
      padding: 2em 1.5em 1.2em 1.5em;
      border-radius: 24px;
      box-shadow: 0 4px 32px rgba(15,163,177,0.18);
      width: 290px;
      text-align: left;
      position: relative;
    }
    h2 {
      font-size: 1.27em;
      color: #34495e;
      margin-bottom: 1.2em;
      letter-spacing: 1px;
      font-weight: 800;
    }
    .event-list {
      list-style: none;
      padding: 0;
      margin: 0;
    }
    .event-list li {
      margin-bottom: 16px;
      padding: 12px;
      background: #fff7e6;
      border-radius: 10px;
      color: #12365e;
      font-weight: 600;
      font-size: 1em;
      box-shadow: 0 2px 8px #db7c2610;
      transition: background 0.18s;
      cursor: pointer;
    }
    .event-list li:hover {
      background: #f2d43d;
      color: #3d246c;
    }
    .bg-figures {
      position: absolute;
      bottom: -4px;
      left: 0;
      width: 100%;
      height: 66px;
      background: url('https://i.imgur.com/8T4mfZC.png') bottom left no-repeat;
      background-size: cover;
      pointer-events: none;
    }
  </style>
</head>
<body>
  <div class="container">
    <h2>Choose an Event</h2>
    <ul class="event-list">
      <li>CRICKET</li>
      <li>BADMINTON</li>
      <li>VOLLEY BALL</li>
      <li>FOOTBALL</li>
      <li>ATHLETICS</li>
      <li>A.T.TUN QUBLY</li>
    </ul>
    <div class="bg-figures"></div>
  </div>
</body>
</html>

<!-- PART 3: REGISTRATION FORM SCREEN -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Sports Day Registration</title>
  <style>
    body {
      background: linear-gradient(135deg, #f441a5 0%, #03c8a8 100%);
      margin: 0;
      height: 100vh;
      font-family: 'Montserrat', sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
    }
    .container {
      width: 300px;
      background: rgba(255, 255, 255, 0.10);
      padding: 2em 1.5em 1em 1.5em;
      border-radius: 24px;
      box-shadow: 0 8px 40px rgba(244,65,165,0.12);
      position: relative;
      text-align: left;
    }
    h2 {
      color: #23004d;
      margin-bottom: 16px;
      font-size: 1.25em;
    }
    .form-group {
      margin-bottom: 14px;
    }
    label {
      display: block;
      margin-bottom: 4px;
      font-size: 0.93em;
      font-weight: 600;
      color: #2b093a;
    }
    input, select {
      width: 100%;
      padding: 9px 11px;
      font-size: 1em;
      border: none;
      border-radius: 7px;
      margin-bottom: 2px;
      background: #fff;
    }
    .submit-btn {
      width: 100%;
      padding: 11px;
      background: #ff3b74;
      color: #fff;
      border: none;
      font-size: 1.08em;
      font-weight: 700;
      border-radius: 9px;
      box-shadow: 0 1px 8px #ce53ff16;
      margin-top: 12px;
      cursor: pointer;
      transition: background 0.2s;
    }
    .submit-btn:hover {
      background: #23004d;
      color: #fff;
    }
    .bg-athletes {
      position: absolute;
      bottom: 0;
      left: 0;
      width: 100%;
      height: 80px;
      background: url('https://i.imgur.com/Bmk7Ggw.png') bottom left no-repeat;
      background-size: contain;
      pointer-events: none;
    }
  </style>
</head>
<body>
  <div class="container">
    <h2>Registration</h2>
    <form>
      <div class="form-group">
        <label>Full Name</label>
        <input type="text" required>
      </div>
      <div class="form-group">
        <label>Email ID</label>
        <input type="email" required>
      </div>
      <div class="form-group">
        <label>Register Number</label>
        <input type="text" required>
      </div>
      <div class="form-group">
        <label>Department</label>
        <input type="text" required>
      </div>
      <div class="form-group">
        <label>Mobile Number</label>
        <input type="tel" required>
      </div>
      <div class="form-group">
        <label>About Self</label>
        <input type="text">
      </div>
      <div class="form-group">
        <label>Event to Register</label>
        <select>
          <option>Cricket</option>
          <option>Badminton</option>
          <option>Volley Ball</option>
          <option>Football</option>
          <option>Athletics</option>
          <option>A.T.Tun Qubly</option>
        </select>
      </div>
      <button class="submit-btn" type="submit">SUBMIT</button>
    </form>
    <div class="bg-athletes"></div>
  </div>
</body>
</html>

<!-- PART 4: THANK YOU SCREEN -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Thank You - Sports Day</title>
  <style>
    body {
      margin: 0;
      background: linear-gradient(120deg, #89f7fe 0%, #66a6ff 100%);
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      font-family: 'Montserrat', sans-serif;
    }
    .container {
      width: 300px;
      padding: 2.2em 1.3em 1.1em 1.3em;
      border-radius: 24px;
      background: rgba(255,255,255,0.10);
      text-align: center;
      box-shadow: 0 4px 24px #0084ff12;
      position: relative;
    }
    .logo {
      width: 68px;
      margin-bottom: 10px;
    }
    .thank-title {
      font-size: 1.4em;
      color: #094348;
      font-weight: 850;
      letter-spacing: 1px;
      margin-bottom: 12px;
      margin-top: 0;
    }
    .thank-message {
      margin-bottom: 0;
      color: #2d4962;
      font-size: 1.05em;
      font-weight: 600;
    }
    .bg-thank {
      position: absolute;
      bottom: 0;
      left: 0;
      height: 70px;
      width: 100%;
      background: url('https://i.imgur.com/B1FLkLX.png') bottom center no-repeat;
      background-size: cover;
      pointer-events: none;
    }
  </style>
</head>
<body>
  <div class="container">
    <img class="logo" src="https://i.imgur.com/g8RHtH5.png" alt="Saveetha Engineering College Logo" />
    <h2 class="thank-title">THANK YOU</h2>
    <div class="thank-message">
      We are all eagerly waiting for your participation in the sports events!
    </div>
    <div class="bg-thank"></div>
  </div>
</body>
</html>

'''
## OUTPUT:
<img width="1012" height="581" alt="Screenshot 2025-10-24 092519" src="https://github.com/user-attachments/assets/45a81870-41ad-4fd0-875f-fd5f2a69fee5" />


## RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.
