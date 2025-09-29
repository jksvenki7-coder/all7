# all7<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>JKS Group All in One Website</title>
<style>
  body {
    font-family: Arial, sans-serif;
    background: #f7fafc;
    margin: 0;
    color: #205081;
  }
  .header {
    display: flex;
    justify-content: space-between;
    padding: 16px 36px;
    background: #e3effa;
    font-weight: 600;
    color: #2e6aa7;
    border-bottom: 3px solid #7fd0f0;
  }
  .main-menu {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 18px;
    margin: 20px auto 30px;
    width: 92%;
  }
  .menu-box {
    background: #f4fafe;
    border: 2px solid #85bbeb;
    border-radius: 10px;
    min-width: 140px;
    padding: 25px 14px;
    text-align: center;
    font-size: 1em;
    font-weight: 600;
    color: #205081;
    box-shadow: 0 2px 8px #dde8f9;
    cursor: pointer;
    transition: background 0.3s ease;
  }
  .menu-box:hover {
    background: #d0e6fb;
  }
  .section-container {
    max-width: 980px;
    margin: 0 auto 40px;
    background: #fff;
    border-radius: 10px;
    box-shadow: 0 3px 14px #d3d7dbcc;
    padding: 20px 32px 30px;
    display: none;
  }
  .section-container.active {
    display: block;
  }
  h2.section-title {
    color: #295bb6;
    text-align: center;
    margin-bottom: 20px;
    font-weight: 700;
    font-size: 1.6em;
  }
  .sections-grid {
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
    gap: 28px;
  }
  .box {
    background: #fcfdff;
    border: 2px solid #6eb7e7;
    border-radius: 11px;
    padding: 20px 14px;
    min-width: 300px;
    max-width: 340px;
    box-shadow: 0 2px 14px #daeefd60;
  }
  .box-title {
    background: #479ede;
    color: white;
    font-size: 1.15em;
    font-weight: 600;
    padding: 12px 0;
    border-radius: 8px;
    text-align: center;
    margin-bottom: 16px;
  }
  ul {
    list-style-type: disc;
    padding-left: 22px;
    color: #273965;
    font-size: 1.06em;
  }
  ul li {
    margin-bottom: 8px;
  }
  /* Form Styling */
  form {
    max-width: 520px;
    margin: 0 auto;
  }
  label {
    font-weight: 600;
    margin-top: 20px;
    display: block;
    font-size: 1.05em;
  }
  input, textarea {
    width: 100%;
    padding: 12px 12px;
    border-radius: 6px;
    border: 1.6px solid #85bbeb;
    font-size: 1em;
  }
  textarea { min-height: 90px; resize: vertical; }
  button.submit-btn {
    background-color: #205081;
    border: none;
    color: white;
    padding: 14px 30px;
    border-radius: 10px;
    font-weight: 700;
    font-size: 1.12em;
    margin-top: 28px;
    width: 100%;
    cursor: pointer;
    transition: background-color 0.3s;
  }
  button.submit-btn:hover {
    background-color: #2e6aa7;
  }
  .success-message {
    margin-top: 18px;
    color: #0a6a33;
    font-weight: 600;
    text-align: center;
    display: none;
  }
  /* Courier & Ride tabs */
  .tabs {
    display: flex;
    justify-content: center;
    gap: 12px;
    margin-bottom: 18px;
  }
  .tabs button {
    background: white;
    border: 2px solid #87ceeb;
    border-radius: 6px;
    cursor: pointer;
    color: #87ceeb;
    font-weight: bold;
    padding: 10px 18px;
  }
  .tabs button.active, .tabs button:hover {
    background: #87ceeb;
    color: white;
  }
  .tab-content {
    display: none;
    margin-top: 12px;
  }
  .tab-content.active {
    display: block;
  }
  label.switch-label {
    margin: 10px 10px 10px 0;
    font-weight: normal;
  }
  label.switch-label input {
    margin-right: 6px;
  }
  /* Tours Tabs */
  nav.tours-nav {
    background: #87ceeb;
    display: flex;
    justify-content: center;
    gap: 20px;
    padding: 10px 0;
    margin-bottom: 25px;
  }
  nav.tours-nav button {
    background: white;
    border: none;
    border-radius: 5px;
    color: #87ceeb;
    padding: 8px 18px;
    font-weight: bold;
    cursor: pointer;
  }
  nav.tours-nav button:hover, nav.tours-nav button.active {
    background: #b0e0ff;
    color: #235e84;
  }
  /* Footer */
  footer {
    background: #87ceeb;
    color: white;
    font-weight: 600;
    padding: 14px 0;
    text-align: center;
  }
  footer a {
    color: white;
    text-decoration: none;
  }
  footer a:hover {
    text-decoration: underline;
  }
</style>
</head>
<body>

<div class="header">
  <span>Profile</span>
  <span>Add Cash</span>
</div>

<div class="main-menu">
  <div class="menu-box" onclick="showSection('dashboard')">Dashboard Home</div>
  <div class="menu-box" onclick="showSection('ecommerce')">My E-commerce</div>
  <div class="menu-box" onclick="showSection('eventsCatering')">Events & Catering</div>
  <div class="menu-box" onclick="showSection('courierRide')">Courier & Ride Booking</div>
  <div class="menu-box" onclick="showSection('loansInsurance')">Loans & Insurance</div>
  <div class="menu-box" onclick="showSection('toursTravel')">Tours & Travels</div>
  <div class="menu-box" onclick="showSection('homeService')">Home Service & Accessories</div>
  <div class="menu-box" onclick="showSection('jobService')">Job Consultancy & Services</div>
  <div class="menu-box" onclick="showSection('investmentBusiness')">Investments & Business</div>
</div>

<!-- Dashboard -->
<div id="dashboard" class="section-container active">
  <h2 class="section-title">JKS Group Dashboard</h2>
  <div class="display-bar">Add (or) product display</div>
  <div class="sections-grid">
    <div class="box" onclick="showSection('ecommerce')">My E-commerce</div>
    <div class="box" onclick="showSection('eventsCatering')">Events & Catering</div>
    <div class="box" onclick="showSection('courierRide')">Courier & Ride Booking</div>
    <div class="box" onclick="showSection('jobService')">Job Consultancy & Services</div>
    <div class="box">Recharge & Pay Bills</div>
    <div class="box" onclick="showSection('toursTravel')">Tours & My Travels</div>
    <div class="box">Real Estate & Construction</div>
    <div class="box" onclick="showSection('investmentBusiness')">Investments & Business</div>
    <div class="box">My Franchise & My Micro Money</div>
    <div class="box" onclick="showSection('loansInsurance')">My Loans & My Insurance</div>
    <div class="box">My Games & My Entertainment</div>
  </div>
</div>

<!-- E-commerce -->
<div id="ecommerce" class="section-container">
  <h2 class="section-title">My E-commerce Order Form</h2>
  <form id="orderForm">
    <label for="name">Full Name</label>
    <input id="name" name="name" type="text" placeholder="Enter your full name" required />
    <label for="mobile">Mobile Number</label>
    <input id="mobile" type="tel" pattern="[0-9]{10,15}" name="mobile" placeholder="Enter mobile number" required />
    <label for="orderDetails">Order Details</label>
    <textarea id="orderDetails" name="orderDetails" placeholder="Enter order details" required></textarea>
    <label for="address">Delivery Address</label>
    <textarea id="address" name="address" placeholder="Enter delivery address" required></textarea>
    <button type="submit" class="submit-btn">Submit Order via WhatsApp</button>
    <p id="successMsg" class="success-message">Your order message has been prepared in WhatsApp.</p>
  </form>
</div>

<!-- Events & Catering -->
<div id="eventsCatering" class="section-container">
  <h2 class="section-title">Events & Catering</h2>
  <div class="box-title">Packages</div>
  <p>Details of catering packages and customization options will go here.</p>
</div>

<!-- Courier & Ride Booking -->
<div id="courierRide" class="section-container">
  <h2 class="section-title">Courier & Ride Booking</h2>
  <div class="tabs">
    <button id="courierBtn" class="active" onclick="activateCourierTabs('courierBtn','courier')">Courier</button>
    <button id="rideBtn" onclick="activateCourierTabs('rideBtn','ride')">Ride Booking</button>
    <button id="rentBtn" onclick="activateCourierTabs('rentBtn','rent')">Rental Vehicle</button>
  </div>
  <div id="courier" class="tab-content active">
    <label>Select Location:</label>
    <select>
      <option>Send</option>
      <option>Receive</option>
    </select>
    <label>Vehicle Type:</label>
    <label><input type="radio" name="courierVehicle" checked /> Bike</label>
    <label><input type="radio" name="courierVehicle" /> Auto</label>
    <label><input type="radio" name="courierVehicle" /> Car</label>
  </div>
  <div id="ride" class="tab-content">
    <label>Ride Type:</label>
    <label><input type="radio" name="rideType" checked /> Bike</label>
    <label><input type="radio" name="rideType" /> Auto</label>
    <label><input type="radio" name="rideType" /> Car</label>
  </div>
  <div id="rent" class="tab-content">
    <label>Rental Mode:</label>
    <label><input type="radio" name="rentMode" checked onchange="toggleRentOptions(true)" /> Self</label>
    <label><input type="radio" name="rentMode" onchange="toggleRentOptions(false)" /> With Driver</label>
  <div id="selfVehicleOptions">
    <label>Vehicle:</label>
    <label><input type="radio" name="selfVehicle" checked /> Bike</label>
    <label><input type="radio" name="selfVehicle" /> Car</label>
    <label><input type="radio" name="selfVehicle" /> Auto</label>
  </div>
  <div id="driverVehicleOptions" style="display:none">
    <label>Vehicle:</label>
    <label><input type="radio" name="driverVehicle" /> Bike</label>
    <label><input type="radio" name="driverVehicle" /> Car</label>
    <label><input type="radio" name="driverVehicle" /> Auto</label>
    <label><input type="radio" name="driverVehicle" /> Bolero</label>
    <label><input type="radio" name="driverVehicle" /> Volvo</label>
    <label><input type="radio" name="driverVehicle" /> Jeep</label>
  </div>
  </div>
</div>

<!-- Loans & Insurance -->
<div id="loansInsurance" class="section-container">
  <h2 class="section-title">Loans & Insurance</h2>
  <div class="sections-grid">
    <div class="box">
      <div class="box-title">Loans</div>
      <ul>
        <li>Loan</li><li>Car</li><li>Bike</li><li>House</li>
        <li>Personal</li><li>Business</li><li>etc</li>
      </ul>
    </div>
    <div class="box">
      <div class="box-title">Insurance</div>
      <ul>
        <li>Health</li><li>Mobile</li><li>Car</li><li>Bike</li><li>etc</li>
      </ul>
    </div>
  </div>
</div>

<!-- Tours & Travels -->
<div id="toursTravel" class="section-container">
  <h2 class="section-title">Tours & Travels</h2>
  <nav class="tours-nav">
    <button onclick="showTourTab('tours')" class="active">Tours</button>
    <button onclick="showTourTab('rooms')">Rooms</button>
    <button onclick="showTourTab('travel')">Travel</button>
  </nav>
  <div id="tours" class="tab-content active">
    <h3>My Tours</h3>
    <ul>
      <li>Kerala</li><li>Goa</li><li>Mumbai</li><li>Others</li>
    </ul>
  </div>
  <div id="rooms" class="tab-content">
    <h3>Rooms (Homestay)</h3>
    <p>Location based rooms display here.</p>
  </div>
  <div id="travel" class="tab-content">
    <h3>Travel</h3>
    <ul>
      <li>Car</li><li>Van</li><li>Volvo Bus</li><li>Mini Bus</li>
    </ul>
  </div>
</div>

<!-- Home Services & Accessories -->
<div id="homeService" class="section-container">
  <h2 class="section-title">Home Service & Accessories</h2>
  <div>
    <h3>Car & Vehicle</h3>
    <ul>
      <li>Car wash & repair</li><li>Bike wash & repair</li><li>Barber shop (male & female)</li><li>16th boundary service</li><li>Car driver (lease)</li><li>General car driver</li>
    </ul>
    <h3>Home & Technical Services</h3>
    <ul>
      <li>Computer tailor</li><li>Electrician</li><li>Helpers</li><li>Home cleaning & shifting</li><li>Plumber (tools & equipment)</li><li>Painter (brushes & paint)</li><li>Technician (wiring/tools)</li>
    </ul>
    <h3>Technology Repairs</h3>
    <ul>
      <li>CC camera installation</li><li>Computer repair</li><li>Mobile repair</li>
    </ul>
    <h3>Culinary Services</h3>
    <ul>
      <li>Chefs / Cooking specialists</li>
    </ul>
  </div>
</div>

<!-- Job Consultancy & Services -->
<div id="jobService" class="section-container">
  <h2 class="section-title">Job Consultancy & Services</h2>
  <p>Content for jobs and services here...</p>
</div>

<!-- Investments & Business -->
<div id="investmentBusiness" class="section-container">
  <h2 class="section-title">Investments & Business</h2>
  <p>Content for investments and business here...</p>
</div>

<footer>
  Contact us: <a href="tel:+918977143043">+91 89771 43043</a> | WhatsApp: <a href="https://wa.me/918977143043" target="_blank">+91 89771 43043</a>
</footer>

<script>
  function showSection(id) {
    document.querySelectorAll('.section-container').forEach(s => s.classList.remove('active'));
    document.getElementById(id).classList.add('active');
    clearSuccessMsg();
    if(id === 'ecommerce') {
      document.getElementById('orderForm').reset();
    }
  }

  function activateCourierTabs(btnId, contentId) {
    ['courierBtn', 'rideBtn', 'rentBtn'].forEach(id => document.getElementById(id).classList.remove('active'));
    ['courier', 'ride', 'rent'].forEach(id => document.getElementById(id).classList.remove('active'));
    document.getElementById(btnId).classList.add('active');
    document.getElementById(contentId).classList.add('active');
  }

  function showTourTab(id) {
    ['tours', 'rooms', 'travel'].forEach(i => document.getElementById(i).classList.remove('active'));
    document.querySelectorAll('nav.tours-nav button').forEach(b => b.classList.remove('active'));
    document.getElementById(id).classList.add('active');
    event.target.classList.add('active');
  }

  function toggleRentOptions(isSelf) {
    document.getElementById("selfVehicleOptions").style.display = isSelf ? "block" : "none";
    document.getElementById("driverVehicleOptions").style.display = isSelf ? "none" : "block";
  }

  // E-Commerce Order Form
  const orderForm = document.getElementById('orderForm');
  const successMsg = document.getElementById('successMsg');
  successMsg.style.display = "none";

  orderForm.addEventListener('submit', e => {
    e.preventDefault();
    const name = e.target.name.value.trim();
    const mobile = e.target.mobile.value.trim();
    const details = e.target.orderDetails.value.trim();
    const address = e.target.address.value.trim();

    if(!name || !mobile || !details || !address){
      alert("Please fill all fields!");
      return;
    }
    const message = `Hello, I want to place order.%0AName: ${name}%0AMobile: ${mobile}%0AOrder Details: ${details}%0ADelivery Address: ${address}`;
    const whatsappNumber = '918977143043';
    window.open(`https://wa.me/${whatsappNumber}?text=${message}`, '_blank');
    successMsg.style.display = "block";
    orderForm.reset();
  });

  function clearSuccessMsg() {
    successMsg.style.display = "none";
  }

  // Initialize with dashboard visible
  showSection('dashboard');
  activateCourierTabs('courierBtn', 'courier');
  showTourTab('tours');
  toggleRentOptions(true);
</script>

</body>
</html>
