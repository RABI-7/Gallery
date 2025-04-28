# Ex.08 Design of Interactive Image Gallery
# Date:27/04/2025
# AIM:
To design a web application for an inteactive image gallery with minimum five images.

# DESIGN STEPS:
## Step 1:
Clone the github repository and create Django admin interface.

## Step 2:
Change settings.py file to allow request from all hosts.

## Step 3:
Use CSS for positioning and styling.

## Step 4:
Write JavaScript program for implementing interactivity.

## Step 5:
Validate the HTML and CSS code.

## Step 6:
Publish the website in the given URL.

# PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>GOAT Bites Restaurant</title>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #fdfdfd;
    }
    header {
      background-color: #ff6f61 ;
      color: white;
      padding: 20px;
      text-align: center;
    }
    nav {
      display: flex;
      justify-content: center;
      background-color: #333;
    }
    nav a {
      color: white;
      padding: 14px 20px;
      text-decoration: none;
      text-align: center;
    }
    nav a:hover {
      background-color: #575757;
    }
    section {
      padding: 40px;
    }
    .dishes, .chefs {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }
    .card {
      background-color: white;
      border-radius: 10px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
      padding: 20px;
      text-align: center;
    }
    .card img {
      width: 100%;
      height: 200px;
      object-fit: cover;
      border-radius: 8px;
    }
    h2 {
      text-align: center;
      color: #000000;
      margin-bottom: 20px;
    }
    footer {
      background-color: #333;
      color: white;
      text-align: center;
      padding: 15px;
      margin-top: 30px;
    }
    form {
      max-width: 500px;
      margin: auto;
    }
    input, textarea {
      width: 100%;
      padding: 10px;
      margin: 8px 0;
      border-radius: 5px;
      border: 1px solid #ccc;
    }
    button {
      background-color: #17ebdd;
      color: white;
      border: none;
      padding: 10px 20px;
      border-radius: 5px;
      cursor: pointer;
    }
    button:hover {
      background-color: #16b698;
    }
  </style>
</head>
<body>

<header>
  <h1>GOAT Bites</h1>
  <p>Fresh. Delicious. Made with Love.</p>
</header>

<nav>
  <a href="#home">Home</a>
  <a href="#food">Foods</a>
  <a href="#administration">Administration</a>
  <a href="#contact">Contact</a>
</nav>

<section id="home">
  <h2>Home</h2>
  <p style="text-align:center;">Welcome to Delish Bites, where passion meets flavor! Indulge in a culinary adventure with our exquisitely crafted dishes, made with fresh, high-quality ingredients and a whole lot of love. Come, savor the moment and explore a world of delicious possibilities! </p>
</section>

<section id="food">
  <h2>Our Food Menu</h2>
  <div class="dishes">
    <div class="card">
      <img src="Pizza Margherita Recipe.jpeg" alt="Margherita Pizza">
      <h3>Margherita Pizza</h3>
      <p>Tomatoes, mozzarella, and basil on crispy crust.</p>
    </div>
    <div class="card">
      <img src="Spaghetti Carbonara.jpg" alt="Spaghetti Carbonara">
      <h3>Spaghetti Carbonara</h3>
      <p>Rich and creamy with pancetta and parmesan.</p>
    </div>
    <div class="card">
      <img src="Cheeseburge.jpg" alt="Cheeseburger">
      <h3>Cheeseburger Deluxe</h3>
      <p>Juicy beef patty, cheese, and lettuce.</p>
    </div>
    <div class="card">
      <img src="Sushi Platter.jpg" alt="Sushi Platter">
      <h3>Sushi Platter</h3>
      <p>Fresh selection of sushi rolls and sashimi.</p>
    </div>
    <div class="card">
      <img src="Caesar Salad.jpg" alt="Caesar Salad">
      <h3>Caesar Salad</h3>
      <p>Classic salad with creamy dressing.</p>
    </div>
    <div class="card">
      <img src="Grilled Steak.jpg" alt="Grilled Steak">
      <h3>Grilled Steak</h3>
      <p>Perfectly grilled tender steak.</p>
    </div>
    <div class="card">
      <img src="Chocolate Lava Cake.jpg" alt="Chocolate Lava Cake">
      <h3>Chocolate Lava Cake</h3>
      <p>Melting chocolate goodness inside.</p>
    </div>
    <div class="card">
      <img src="Fluffy Pancakes.jpg" alt="Fluffy Pancakes">
      <h3>Fluffy Pancakes</h3>
      <p>Soft pancakes with maple syrup.</p>
    </div>
    <div class="card">
      <img src="Mexican Tacos.jpg" alt="Mexican Tacos">
      <h3>Mexican Tacos</h3>
      <p>Spiced meat and fresh toppings.</p>
    </div>
  </div>
</section>

<section id="administration">
  <h2>Our Chefs</h2>
  <div class="chefs">
    <div class="card">
      <img src="Chef Mario Rossi.jpg" alt="Chef Mario">
      <h3>Chef Mario Rossi</h3>
      <p>Master of Italian cuisine.</p>
    </div>
    <div class="card">
      <img src="sydney sweeney.jpg" alt="Sydney Sweeney">
      <h3>Chef Sydney Sweeney</h3>
      <p>Japanese sushi and traditional food expert.</p>
    </div>
    <div class="card">
      <img src="Amninder Sandhu.jpg" alt="Amninder Sandhu">
      <h3>Chef Amninder Sandhu</h3>
      <p>American grill and dessert innovator.</p>
    </div>
  </div>
</section>

<section id="contact">
  <h2>Contact Us</h2>
  <div class="contact-grid">
    <div class="card contact-box">
      <div class="contact-icon"><i class="fab fa-instagram"></i></div>
      <p><strong>Instagram</strong></p>
      <a href="https://www.instagram.com/_rabii.___" target="_blank">@goatbites</a>
    </div>
    <div class="card contact-box">
      <div class="contact-icon"><i class="fas fa-phone-alt"></i></div>
      <p><strong>Mobile</strong></p>
      <a href="tel:6969">+123 696</a>
    </div>
    <div class="card contact-box">
      <div class="contact-icon"><i class="fas fa-envelope"></i></div>
      <p><strong>Email</strong></p>
      <a href="mailto:your.email@goatbites.com">@goatbites.com</a>
    </div>
  </div>
</section>

<footer>
  <p>&copy; 2025 Delish Bites. All rights reserved.</p>
</footer>

<!-- JavaScript -->
<script>
  const form = document.getElementById('contactForm');
  form.addEventListener('submit', function(event) {
    event.preventDefault();
    const name = document.getElementById('name').value.trim();
    const email = document.getElementById('email').value.trim();
    const message = document.getElementById('message').value.trim();
    
    if(name && email && message) {
      alert(`Thank you, ${name}! We have received your message.`);
      form.reset();
    } else {
      alert('Please fill in all fields before submitting.');
    }
  });
</script>

</body>
</html>

```
# OUTPUT:
![Screenshot (89)](https://github.com/user-attachments/assets/32478e0f-5f94-45e5-a5cb-76c9a31c1e29)
![Screenshot (90)](https://github.com/user-attachments/assets/60277793-32a4-4490-8aed-6b1aa52a3b34)
![Screenshot (91)](https://github.com/user-attachments/assets/90769f0f-dbb4-4a16-b7fa-f06e4c68b1ea)
![Screenshot (92)](https://github.com/user-attachments/assets/789f62c5-152c-4ba6-a0b3-d4a2b4dc9fbb)


# RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
