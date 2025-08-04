<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>IIM Jammu Admissions</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <div class="container">
    <h1>IIM Jammu Admission Portal</h1>
    <p>Login to check your admission status</p>
    <a href="login.html" class="button">Login</a>
  </div>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Login - IIM Jammu</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <div class="login-container">
    <h2>Login to Check Admission Status</h2>
    <form onsubmit="return validateLogin()">
      <input type="text" id="jipmat_id" placeholder="Enter JIPMAT ID" required><br>
      <input type="date" id="dob" required><br>
      <button type="submit">Login</button>
    </form>
    <p id="error-msg"></p>
  </div>
  <script src="script.js"></script>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Admission Offer - IIM Jammu</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <div class="container">
    <h2>Subject: Offer of Admission to the Five-Year Integrated Programme in Management (IPM) ISSUED ON 9 AUGUST 2025.</h2>
    <p>Dear <strong>AYAAN CHAUDHARY</strong>,</p>
    <p>
      We are pleased to inform you that, based on your performance in the Joint Integrated Programme in Management Admission Test (JIPMAT) 2025,
      you have been provisionally selected for admission to the Five-Year Integrated Programme in Management (IPM) at IIM Jammu for the academic session 2025–2030 under the OBC-NCL (Male) category.
    </p>
    <p>
      Please note that this offer is provisional and subject to verification of all the academic and category documents at the time of registration.
      Any discrepancy or misrepresentation of facts may lead to immediate cancellation of admission without further notice.
    </p>
    <p>
      To confirm your acceptance of this offer and secure your seat in the programme, you are required to remit a non-refundable Offer Acceptance Amount (OAA) of INR 50,000 (Fifty Thousand Only) on or before 23:59 hours, 12th August 2025.
    </p>
    <p>
      <strong>Payment Details:</strong><br>
      • Amount: ₹50,000<br>
      • Payment Deadline: 12th August 2025, 23:59 IST (strictly non-extendable)<br>
      • Mode of Payment: The payment must be made through the online admission portal, <a href="#">CLICK HERE</a> to PAY.
    </p>
    <p>
      Failure to remit the Offer Acceptance Amount by the specified deadline will be construed as non-acceptance of this offer,
      and your candidature will stand cancelled automatically without any further communication from our side. The seat so vacated will be offered to the next eligible candidate on the waiting list.
    </p>
    <p>
      Upon successful payment and subsequent verification of documents, you will receive further communication regarding the registration,
      orientation schedule, hostel allocation, and commencement of academic activities.
    </p>
    <p>
      We take this opportunity to congratulate you and extend a warm welcome to the IIM Jammu community.
      We are confident that your journey with us will be intellectually enriching and personally rewarding.
    </p>
    <p>
      Should you require any clarification regarding this admission offer, please feel free to reach out to us at <a href="mailto:ipm.admissions@iimj.ac.in">ipm.admissions@iimj.ac.in</a>.
    </p>
    <p>
      With best wishes,<br><br>
      Yours sincerely,<br>
      <strong>Chairperson – Admissions<br>Indian Institute of Management Jammu</strong>
    </p>
  </div>
</body>
</html>
body {
  font-family: Arial, sans-serif;
  background-color: #e0f0ff; /* light blue */
  text-align: center;
  padding-top: 50px;
}

.container, .login-container {
  background-color: #ffffff;
  border: 2px solid red;
  width: 90%;
  max-width: 800px;
  margin: auto;
  padding: 30px;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(255, 0, 0, 0.2);
  text-align: left;
}

input {
  width: 90%;
  padding: 10px;
  margin: 10px auto;
  display: block;
  border: 1px solid red;
  border-radius: 4px;
}

button, .button {
  background-color: red;
  color: white;
  padding: 10px 20px;
  border: 2px solid red;
  border-radius: 4px;
  text-decoration: none;
  display: inline-block;
  margin-top: 10px;
  cursor: pointer;
  font-size: 16px;
}

button:hover, .button:hover {
  background-color: darkred;
}

#error-msg {
  color: red;
  font-size: 14px;
}
function validateLogin() {
  const id = document.getElementById("jipmat_id").value.trim();
  const dob = document.getElementById("dob").value;

  if (id === "250410000035" && dob === "2006-09-15") {
    window.location.href = "dashboard.html";
    return false;
  } else {
    document.getElementById("error-msg").textContent = "Invalid JIPMAT ID or Date of Birth.";
    return false;
  }
}
