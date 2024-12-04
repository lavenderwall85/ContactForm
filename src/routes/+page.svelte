  <style>
    body {
      background-color: #f0f9f4;
      font-family: Arial, sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
    }
  
    .form-container {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      background: white;
      padding: 1.5rem;
      border-radius: 8px;
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
      width: 90%;
      max-width: 450px;
    }
  
    .form-container h1 {
      font-size: 1.4rem;
      margin-bottom: 1rem;
      color: #333;
      text-align: center;
    }
  
    .form-group {
      margin-bottom: 0.75rem;
    }
  
    .form-group label {
      display: block;
      margin-bottom: 0.4rem;
      font-size: 0.9rem;
      font-weight: bold;
      color: #555;
    }
  
    .form-group input,
    .form-group textarea {
      width: 100%;
      padding: 0.6rem;
      border: 1px solid #ccc;
      border-radius: 4px;
      font-size: 0.95rem;
    }
  
    .form-group textarea {
      resize: none;
      height: 80px;
    }
  
    .form-group input[type="radio"] {
      margin-right: 0.4rem;
    }
  
    .form-group .radio-group {
      display: flex;
      gap: 1rem;
    }
  
    .form-group input[type="checkbox"] {
      margin-right: 0.5rem;
    }
  
    .submit-btn {
      width: 100%;
      padding: 0.6rem;
      background-color: #059669;
      color: white;
      border: none;
      border-radius: 4px;
      font-size: 1rem;
      font-weight: bold;
      cursor: pointer;
      margin-top: 1rem;
    }
  
    .submit-btn:hover {
      background-color: #047857;
    }
  </style>
  
  <div class="form-container">
    <h1>Contact Us</h1>
    <div class="form-group">
      <label for="firstName">First Name *</label>
      <input type="text" id="firstName" name="firstName" placeholder="Enter your first name">
    </div>
    <div class="form-group">
      <label for="lastName">Last Name *</label>
      <input type="text" id="lastName" name="lastName" placeholder="Enter your last name">
    </div>
    <div class="form-group">
      <label for="email">Email Address *</label>
      <input type="email" id="email" name="email" placeholder="Enter your email">
    </div>
    <div class="form-group">
      <label>Query Type *</label>
      <div class="radio-group">
        <label><input type="radio" name="queryType" value="general"> General Enquiry</label>
        <label><input type="radio" name="queryType" value="support"> Support Request</label>
      </div>
    </div>
    <div class="form-group">
      <label for="message">Message *</label>
      <textarea id="message" name="message" placeholder="Write your message"></textarea>
    </div>
    <div class="form-group">
      <label><input type="checkbox" name="consent"> I consent to being contacted *</label>
    </div>
    <button class="submit-btn">Submit</button>
  </div>
  