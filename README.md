[service_website (1).html](https://github.com/user-attachments/files/23899882/service_website.1.html)
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Ashika Academy Services</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <style>
    :root {
      --gold: #d4af37;
      --dark-gold: #b28b2e;
      --black: #0c0c0c;
      --charcoal: #1a1a1a;
      --soft-gold: #f7e7b1;
    }

    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background: var(--charcoal);
      color: var(--soft-gold);
    }

    header {
      background: linear-gradient(135deg, var(--black), var(--dark-gold));
      color: var(--soft-gold);
      padding: 40px 20px;
      text-align: center;
      letter-spacing: 1px;
      box-shadow: 0 4px 20px rgba(0,0,0,0.6);
    }

    nav {
      background: var(--black);
      padding: 15px;
      text-align: center;
      position: sticky;
      top: 0;
      z-index: 200;
      border-bottom: 1px solid var(--gold);
    }
    nav a {
      color: var(--soft-gold);
      margin: 0 12px;
      text-decoration: none;
      font-weight: 600;
      transition: 0.3s;
    }
    nav a:hover { color: var(--gold); }

    .hero {
      padding: 60px 20px;
      background: linear-gradient(135deg, var(--black), var(--gold)20%, var(--charcoal));
      text-align: center;
      animation: fadeIn 2s ease;
      color: var(--soft-gold);
    }
    .hero h1 { font-size: 36px; margin-bottom: 10px; color: var(--gold); }

    .services {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 20px;
      padding: 40px 20px;
      background: var(--black);
    }
    .card {
      background: linear-gradient(145deg, var(--charcoal), var(--black));
      padding: 20px;
      border-radius: 14px;
      border: 1px solid var(--dark-gold);
      box-shadow: 0 4px 15px rgba(0,0,0,0.5);
      color: var(--soft-gold);
      text-align: center;
      transition: 0.3s;
    }
    .card h3::before {
      font-family: 'Font Awesome 6 Free';
      font-weight: 900;
      display: inline-block;
      margin-right: 10px;
    }
    .card:nth-child(1) h3::before { content: '\f485'; }
    .card:nth-child(2) h3::before { content: '\f19d'; }
    .card:nth-child(3) h3::before { content: '\f21b'; }
    .card:nth-child(4) h3::before { content: '\f06e'; }
    .card:hover { transform: translateY(-6px); border-color: var(--gold); box-shadow: 0 6px 25px rgba(212,175,55,0.4); }

    .service-details {
      padding: 40px 20px;
      background: linear-gradient(135deg, var(--charcoal), var(--black));
      color: var(--gold);
    }
    .service-details h2 {
      color: var(--gold);
      text-align: center;
      font-size: 28px;
      margin-bottom: 20px;
    }

    .pricing, .booking, .contact {
      background: var(--black);
      padding: 40px 20px;
      color: var(--soft-gold);
      border-top: 1px solid var(--gold);
      text-align: center;
    }
    .pricing .card { border:1px solid var(--dark-gold); }

    form {
      background: var(--charcoal);
      max-width: 100%;
      margin: auto;
      padding: 20px;
      border-radius: 12px;
      border: 1px solid var(--dark-gold);
      box-shadow: 0 4px 15px rgba(0,0,0,0.5);
    }
    input, textarea, select {
      width: 100%; padding: 10px; margin: 10px 0;
      background: var(--black); color: var(--soft-gold);
      border: 1px solid var(--gold); border-radius: 6px;
    }
    button {
      background: var(--gold); color: var(--black);
      border: none; padding: 12px; width: 100%; border-radius: 8px;
      font-size: 16px; font-weight: 700; cursor: pointer; transition: 0.3s;
    }
    button:hover { background: var(--soft-gold); color: var(--black); }

    footer {
      background: var(--black); color: var(--gold);
      text-align: center; padding: 20px; margin-top: 20px;
      border-top: 1px solid var(--gold);
    }

    @media (max-width: 768px) {
      .hero h1 { font-size: 28px; }
      nav a { margin: 0 8px; font-size: 14px; }
      .service-details h2 { font-size: 24px; }
      .pricing h1 { font-size: 24px; }
    }

    @keyframes fadeIn { from {opacity: 0;} to {opacity: 1;} }
  </style>
</head>
<body>
  <header>
    <h1>Ashika Academy Services</h1>
    <p>Empowering learners with quality education and services.</p>
  </header>

  <nav>
    <a href="#home">Home</a>
    <a href="#services">Services</a>
    <a href="#details">Details</a>
    <a href="#pricing">Pricing</a>
    <a href="#booking">Booking</a>
    <a href="#contact">Contact</a>
  </nav>

  <section class="hero" id="home">
    <h1>Welcome to Ashika Academy</h1>
    <p>We provide the best academic guidance and professional services.</p>
  </section>

  <section class="services" id="services">
    <div class="card">
      <h3>Nails</h3>
      <p>Professional nail art, manicure, pedicure, and premium nail care services.</p>
    </div>
    <div class="card">
      <h3>Beauty Course</h3>
      <p>Complete beauty training designed to build real skills for your career.</p>
    </div>
    <div class="card">
      <h3>Full Body Makeup</h3>
      <p>High-quality bridal, party, and full-body makeup with expert techniques.</p>
    </div>
    <div class="card">
      <h3>Lashes</h3>
      <p>Premium eyelash extensions, lifting, and styling services.</p>
    </div>
  </section>

  <section class="pricing" id="pricing">
    <h2>Pricing</h2>
    <div style="display:grid; grid-template-columns:repeat(auto-fit,minmax(220px,1fr)); gap:20px; max-width:1000px; margin:auto;">
      <div class="card">
        <h3>Nails</h3>
        <p>Starting From</p>
        <h1 style="color:var(--gold);">Rs. 800</h1>
      </div>
      <div class="card">
        <h3>Beauty Course</h3>
        <p>Complete Course</p>
        <h1 style="color:var(--gold);">Rs. 15,000</h1>
      </div>
      <div class="card">
        <h3>Full Body Makeup</h3>
        <p>Starting From</p>
        <h1 style="color:var(--gold);">Rs. 5,000</h1>
      </div>
      <div class="card">
        <h3>Lashes</h3>
        <p>Starting From</p>
        <h1 style="color:var(--gold);">Rs. 1,500</h1>
      </div>
    </div>
  </section>

  <section class="booking" id="booking">
    <h2>Book an Appointment</h2>
    <form>
      <input type="text" placeholder="Full Name" required />
      <input type="text" placeholder="Phone Number" required />
      <select required>
        <option selected>Select Service</option>
        <option>Nails</option>
        <option>Beauty Course</option>
        <option>Full Body Makeup</option>
        <option>Lashes</option>
      </select>
      <input type="date" required />
      <textarea placeholder="Any special request..." rows="4"></textarea>
      <button type="submit">Book Now</button>
    </form>
  </section>

  <section class="contact" id="contact">
    <h2>Customer Care</h2>
    <p>For any queries or support, contact us at:</p>
    <h3 style="color:var(--gold);">Phone: 9818330123</h3>
  </section>

  <footer>
    © 2025 Ashika Academy. All rights reserved.
  </footer>
</body>
</html>
