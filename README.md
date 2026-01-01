# My-new-project-
My name 

<!DOCTYPE html>
<html lang="eu">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Biko Profile - Front-End Developer</title>

  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }

    body {
      background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      min-height: 100vh;
      gap: 40px;
      padding: 20px;
      color: #333;
    }

    /* ===== Animation Box ===== */
    .profile-container {
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 20px;
    }

    .ani {
      background: linear-gradient(135deg, #ff416c 0%, #ff4b2b 100%);
      width: 320px;
      height: 160px;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      position: relative;
      overflow: hidden;
      color: #fff;
      text-align: center;
      box-shadow: 0 10px 30px rgba(255, 75, 43, 0.3);
      transition: transform 0.5s ease;
    }

    .ani:hover {
      transform: scale(1.05);
    }

    .ani p {
      position: absolute;
      margin: 0;
      font-weight: 600;
      text-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
      padding: 0 20px;
      line-height: 1.4;
    }

    .ani0 {
      animation: opt 6s infinite;
      font-size: 22px;
    }

    .ani1 {
      animation: gio 6s infinite;
      font-size: 20px;
    }

    @keyframes opt {
      0% { opacity: 1; }
      40% { opacity: 1; }
      50% { opacity: 0; }
      100% { opacity: 0; }
    }

    @keyframes gio {
      0% { opacity: 0; }
      50% { opacity: 0; }
      60% { opacity: 1; }
      100% { opacity: 1; }
    }

    /* Developer title */
    .developer-title {
      font-size: 18px;
      color: #555;
      text-align: center;
      font-weight: 500;
      padding: 8px 20px;
      background: rgba(255, 255, 255, 0.8);
      border-radius: 30px;
      box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
    }

    /* ===== Login Box ===== */
    .bixi {
      width: 350px;
      background: #ffffff;
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
      border-radius: 20px;
      padding: 25px;
      text-align: center;
      border: 1px solid rgba(255, 255, 255, 0.3);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }

    .bixi:hover {
      box-shadow: 0 15px 40px rgba(0, 0, 0, 0.15);
      transform: translateY(-5px);
    }

    .log {
      font-size: 28px;
      font-weight: 700;
      margin-bottom: 20px;
      color: #ff4b2b;
      position: relative;
      padding-bottom: 10px;
    }

    .log::after {
      content: '';
      position: absolute;
      bottom: 0;
      left: 50%;
      transform: translateX(-50%);
      width: 60px;
      height: 3px;
      background: #ff4b2b;
      border-radius: 2px;
    }

    .input-container {
      position: relative;
      margin-bottom: 20px;
    }

    .inp {
      width: 100%;
      padding: 14px 20px;
      padding-left: 45px;
      margin: 8px 0;
      border-radius: 50px;
      border: 1px solid #ddd;
      font-size: 16px;
      transition: all 0.3s ease;
      background-color: #f9f9f9;
    }

    .inp:focus {
      outline: none;
      border-color: #ff4b2b;
      box-shadow: 0 0 0 3px rgba(255, 75, 43, 0.1);
      background-color: #fff;
    }

    .input-icon {
      position: absolute;
      left: 15px;
      top: 50%;
      transform: translateY(-50%);
      color: #999;
      font-size: 18px;
    }

    .button-container {
      display: flex;
      justify-content: space-between;
      margin-top: 25px;
      gap: 15px;
    }

    button {
      flex: 1;
      padding: 14px;
      border: none;
      border-radius: 50px;
      font-size: 16px;
      font-weight: 600;
      cursor: pointer;
      transition: all 0.3s ease;
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 8px;
    }

    .submit-btn {
      background: linear-gradient(to right, #ff416c, #ff4b2b);
      color: white;
    }

    .submit-btn:hover {
      background: linear-gradient(to right, #ff4b2b, #ff416c);
      box-shadow: 0 5px 15px rgba(255, 75, 43, 0.4);
    }

    .clear-btn {
      background: #f1f1f1;
      color: #555;
    }

    .clear-btn:hover {
      background: #e0e0e0;
      box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
    }

    .Ac {
      display: inline-block;
      margin-top: 20px;
      text-decoration: none;
      background: linear-gradient(to right, #4776E6, #8E54E9);
      color: white;
      padding: 12px 25px;
      border-radius: 50px;
      font-weight: 600;
      transition: all 0.3s ease;
      box-shadow: 0 5px 15px rgba(142, 84, 233, 0.2);
    }

    .Ac:hover {
      transform: translateY(-3px);
      box-shadow: 0 8px 20px rgba(142, 84, 233, 0.3);
    }

    .footer-text {
      margin-top: 25px;
      font-size: 14px;
      color: #777;
      text-align: center;
      line-height: 1.5;
    }

    /* ===== Media Query ===== */

    /* موبايل */
    @media (max-width: 600px) {
      body {
        gap: 30px;
        padding: 15px;
      }
      
      .ani {
        width: 250px;
        height: 125px;
      }
      
      .ani0 {
        font-size: 18px;
      }
      
      .ani1 {
        font-size: 16px;
      }
      
      .bixi {
        width: 100%;
        padding: 20px;
      }
      
      .button-container {
        flex-direction: column;
      }
      
      button {
        width: 100%;
      }
      
      .developer-title {
        font-size: 16px;
      }
    }

    /* تابلت */
    @media (min-width: 601px) and (max-width: 900px) {
      .ani {
        width: 280px;
        height: 140px;
      }
      
      .bixi {
        width: 80%;
        max-width: 400px;
      }
    }
  </style>
</head>

<body>

  <div class="profile-container">
    <div class="ani">
      <p class="ani0">
        Welcome <br>
        to Biko World
      </p>

      <p class="ani1">
        I am Front-End Developer
      </p>
    </div>
    
    <div class="developer-title">
      HTML • CSS • JavaScript • Astudy Reactjs
    </div>
  </div>

  <div class="bixi">
    <p class="log">Login</p>
    
    <div class="input-container">
      <span class="input-icon">👤</span>
      <input type="text" placeholder="Your name" id="cl" class="inp">
    </div>
    
    <div class="input-container">
      <span class="input-icon">🔒</span>
      <input type="password" placeholder="Your password" id="cl2" class="inp">
    </div>

    <div class="button-container">
      <button class="submit-btn" onclick="submitForm()">
        <span>📨</span> Submit
      </button>
      <button class="clear-btn" onclick="cle()">
        <span>✕</span> Clear
      </button>
    </div>

    <a href="#" id="ri" class="Ac" onclick="unv()">Create New Account</a>
    
    <div class="footer-text">
      Forgot your password? <a href="#" onclick="forgotPassword()" style="color: #ff4b2b; text-decoration: none;">Click here</a>
    </div>
  </div>

  <script>
    function cle() {
      document.getElementById("cl").value = "";
      document.getElementById("cl2").value = "";
      document.getElementById("cl").focus();
      showMessage("Fields cleared successfully", "info");
    }
    
    function submitForm() {
      const name = document.getElementById("cl").value;
      const password = document.getElementById("cl2").value;
      
      if (!name || !password) {
        showMessage("Please fill in all fields", "error");
        return;
      }
      
      if (password.length < 6) {
        showMessage("Password must be at least 6 characters", "error");
        return;
      }
      
      showMessage(`Welcome back, ${name}! Redirecting...`, "success");
      
      // Simulate login process
      setTimeout(() => {
        showMessage("Login successful! Welcome to Biko World.", "success");
      }, 1000);
    }
    
    function unv() {
      showMessage("Account creation is currently unavailable. Please try again later.", "info");
      document.getElementById("ri").href = "#";
    }
    
    function forgotPassword() {
      showMessage("Password reset feature coming soon!", "info");
    }
    
    function showMessage(message, type) {
      // Remove existing message if any
      const existingMsg = document.querySelector(".message-box");
      if (existingMsg) existingMsg.remove();
      
      // Create message element
      const messageBox = document.createElement("div");
      messageBox.className = "message-box";
      messageBox.textContent = message;
      
      // Style based on type
      const styles = `
        position: fixed;
        top: 20px;
        right: 20px;
        padding: 15px 25px;
        border-radius: 10px;
        font-weight: 600;
        box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        z-index: 1000;
        animation: fadeIn 0.3s ease;
        color: white;
        max-width: 300px;
      `;
      
      if (type === "success") {
        messageBox.style.cssText = styles + "background: linear-gradient(to right, #00b09b, #96c93d);";
      } else if (type === "error") {
        messageBox.style.cssText = styles + "background: linear-gradient(to right, #ff416c, #ff4b2b);";
      } else {
        messageBox.style.cssText = styles + "background: linear-gradient(to right, #4776E6, #8E54E9);";
      }
      
      // Add to page
      document.body.appendChild(messageBox);
      
      // Remove after 3 seconds
      setTimeout(() => {
        messageBox.style.animation = "fadeOut 0.5s ease";
        setTimeout(() => {
          if (messageBox.parentNode) {
            messageBox.parentNode.removeChild(messageBox);
          }
        }, 500);
      }, 3000);
    }
    
    // Add CSS for animations
    const styleSheet = document.createElement("style");
    styleSheet.textContent = `
      @keyframes fadeIn {
        from { opacity: 0; transform: translateY(-20px); }
        to { opacity: 1; transform: translateY(0); }
      }
      @keyframes fadeOut {
        from { opacity: 1; transform: translateY(0); }
        to { opacity: 0; transform: translateY(-20px); }
      }
    `;
    document.head.appendChild(styleSheet);
    
    // Focus on name field when page loads
    document.getElementById("cl").focus();
  </script>

</body>
</html>
