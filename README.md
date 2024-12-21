# Ex.07 Restaurant Website
# Date:
# AIM:
To develop a static Restaurant website to display the food items and services provided by them.

# DESIGN STEPS:
## Step 1:
Requirement collection.

## Step 2:
Creating the layout using HTML and CSS.

## Step 3:
Updating the sample content.

## Step 4:
Choose the appropriate style and color scheme.

## Step 5:
![Screenshot 2024-12-21 152414](https://github.com/user-attachments/assets/fb99d0b9-abce-4a81-9585-ba66e0aeab73)
![Screenshot 2024-12-21 152423](https://github.com/user-attachments/assets/bbc5c1a6-f8db-49cd-bc98-6c2a1290654c)
![Screenshot 2024-12-21 152454](https://github.com/user-attachments/assets/10b3f872-61e3-4792-b7ee-f85bc7ad0b84)
![Screenshot 2024-12-21 152506](https://github.com/user-attachments/assets/e85acb38-0664-493d-ba56-e6704b9e580d)

Validate the layout in various browsers.

## Step 6:
Validate the HTML code.
# administration.html
```html
{% load static %}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Little Lemon - Administration</title>
    <link rel="stylesheet" href="{% static 'css/style.css' %}">
</head>
<body>
    <header>
        <div class="logo">LITTLE LEMON</div>
        <nav>
            <ul>
                <li><a href="{% url 'home' %}">Home</a></li>
                <li><a href="{% url 'menu' %}">Menu</a></li>
                <li><a href="{% url 'administration' %}">Administration</a></li>
                <li><a href="{% url 'contact' %}">Contact Us</a></li>
            </ul>
        </nav>
    </header>
    <section class="administration">
        <h1>Meet Our Team</h1>
        <p class="team-intro">Our talented team works tirelessly to provide the best service and food experience. Here's a glimpse at the people who make Little Lemon extraordinary.</p>

        <div class="team">
            <div class="team-member">
                <img src="https://media.istockphoto.com/id/1216130801/photo/smiling-man-with-hands-in-pockets.jpg?s=612x612&w=0&k=20&c=wi3IYW8vH3_NSgRIjZSmrwvA7nrW_GZzAMSkz7HmWmo=" alt="John Doe">
                <h3>John Doe</h3>
                <p>Manager</p>
            </div>
            <div class="team-member">
                <img src="https://media.istockphoto.com/id/186591832/photo/master-chef.jpg?s=612x612&w=is&k=20&c=7_Ov2X8R04TtjR4aM6OWdRLu5jZAXho2RChYk1MHuXk=" alt="Jane Smith">
                <h3>Jane Smith</h3>
                <p>Chef</p>
            </div>
            <div class="team-member">
                <img src="https://media.istockphoto.com/id/1253466968/photo/full-length-of-handsome-young-african-man-in-casual-wear.jpg?s=612x612&w=0&k=20&c=J3QNZecx7xJ5Q3MNlQ2vtf-5ZvEMiZBusFfsFMiMfAg=" alt="Mike Brown">
                <h3>Mike Brown</h3>
                <p>Assistant Chef</p>
            </div>
            <div class="team-member">
                <img src="https://media.istockphoto.com/id/1303500951/photo/full-length-portrait-of-a-smiling-asian-businesswoman.jpg?s=612x612&w=0&k=20&c=28JulKaoJqMJVEycPXpAEXPwJKxXwULwhnY63nBcM_E=" alt="Sarah Wilson">
                <h3>Sarah Wilson</h3>
                <p>Host</p>
            </div>
            <div class="team-member">
                <img src="https://media.istockphoto.com/id/1130450215/photo/full-length-portrait-of-handsome-smiling-young-man.jpg?s=612x612&w=0&k=20&c=I_wjJdwchejrYyGXYd5lUN_LeeeRTcwhoWTmHgni9Dc=" alt="Emily Davis">
                <h3>Emily Davis</h3>
                <p>Waiter</p>
            </div>
            <div class="team-member">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSJU_Kol3UIeRWXI6NUw_nd1qgpblONCZ7vU63HAlZLE4p4z7-zCThGf1MLaaCqXwDPWOM&usqp=CAU" alt="Chris Johnson">
                <h3>Chris Johnson</h3>
                <p>Barista</p>
            </div>
        </div>
    </section>

    <footer>
        <p>Designed by kelvin</p>
    </footer>
</body>
</html>
```
# index.html
```html
{% load static %}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Little Lemon - Home</title>
    <link rel="stylesheet" href="{% static 'css/style.css' %}">
</head>
<body>
    <header>
        <div class="logo">HOTEL PARADISE</div>
        <nav>
            <ul>
                <li><a href="{% url 'home' %}">Home</a></li>
                <li><a href="{% url 'menu' %}">Menu</a></li>
                <li><a href="{% url 'administration' %}">Administration</a></li>
                <li><a href="{% url 'contact' %}">Contact Us</a></li>
            </ul>
        </nav>
    </header>
    <section class="banner">
        <h1>30% Off This Weekend</h1>
        <p>Don't miss out on our delicious offers and amazing food!</p>
    </section>
    <section class="content">
        <div class="card">
            <h2>Our New Menu</h2>
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQGuuxg5971YN5Ar3ypLOqLvFbB9rwVTVAK_A&s" alt="Menu">
            <p>Explore our delicious new menu items, crafted with love.</p>
            <a href="{% url 'menu' %}">Check out the menu</a>
        </div>
        <div class="card">
            <h2>Book a Table</h2>
            <img src="https://cdn.textstudio.com/output/sample/normal/6/9/0/5/book-logo-73-5096.png" alt="Book a Table">
            <p>Reserve your spot at our restaurant today.</p>
            <a href="{% url 'contact' %}">Book Now</a>
        </div>
        <div class="card">
            <h2>Opening Hours</h2>
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQRgxy4LC3j-fg9irjdc6JiR2v6nJJUL1nkpg&s" alt="Opening Hours">
            <p>Mon-Fri: 2 PM - 10 PM<br>Sat: 2 PM - 11 PM<br>Sun: 2 PM - 9 PM</p>
        </div>
    </section>
    <footer>
        <p>Designed by KELVIN</p>
    </footer>
</body>
</html>
```
# menu.html
```html
{% load static %}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Little Lemon - Menu</title>
    <link rel="stylesheet" href="{% static 'css/style.css' %}">
</head>
<body>
    <header>
        <div class="logo">HOTEL PARADISE</div>
        <nav>
            <ul>
                <li><a href="{% url 'home' %}">Home</a></li>
                <li><a href="{% url 'menu' %}">Menu</a></li>
                <li><a href="{% url 'administration' %}">Administration</a></li>
                <li><a href="{% url 'contact' %}">Contact Us</a></li>
            </ul>
        </nav>
    </header>
    <section class="menu">
        <h1>Our Menu</h1>

        
        <h2>Breakfast</h2>
        <div class="menu-grid">
            <div class="menu-item">
                <img src="https://madhurasrecipe.com/wp-content/uploads/2023/01/Ration-Rice-Idli-Featured.jpg" alt="1">
                <h3>IDLY</h3>
                <p>₹10.00</p>
            </div>
            <div class="menu-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT7P9-ECimzMDQMWGiu2XnSWErvEqRmz5rTaw&s" alt="2">
                <h3>DOSA</h3>
                <p>₹50.00</p>
            </div>
            <div class="menu-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS_zVio1zG-MW2sC0KPOespltgpO4yYtgkJyA&s" alt="3">
                <h3>PAROTTA</h3>
                <p>₹30.00</p>
            </div>
        </div>

        
        <h2>Lunch</h2>
        <div class="menu-grid">
            <div class="menu-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcToMozkkZv6pQonP3nn1BlXT2uLTWJxeshxYA&s" alt="Grilled Chicken Salad">
                <h3>Grilled Chicken</h3>
                <p>$12.99</p>
            </div>
            <div class="menu-item">
                <img src="https://www.indianhealthyrecipes.com/wp-content/uploads/2022/02/hyderabadi-biryani-recipe-chicken.jpg" alt="Club Sandwich">
                <h3>chicken-biryani</h3>
                <p>$10.99</p>
            </div>
            <div class="menu-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQknZsQQ2VkMRxF1b8sxIWtxkx4ZrM_OoijXw&s" alt="Soup and Bread">
                <h3>MUTTON BIRIYANI</h3>
                <p>$8.99</p>
            </div>
        </div>

        
        <h2>Dinner</h2>
        <div class="menu-grid">
            <div class="menu-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSB2lwVjot29yqsbGP4ec474gSG6yyM9Dyn6w&s" alt="Steak">
                <h3>FRIED RICE</h3>
                <p>₹199.99</p>
            </div>
            <div class="menu-item">
                <img src="https://www.chilipeppermadness.com/wp-content/uploads/2023/06/Gochujang-Noodles-Recipe1.jpg" alt="Pasta">
                <h3>NOODLES</h3>
                <p>₹149.99</p>
            </div>
            <div class="menu-item">
                <img src="https://hillstreetgrocer.com/application/files/1116/6563/4670/Recipe-image5.jpg" alt="Seafood Platter">
                <h3>Seafood Platter</h3>
                <p>₹120</p>
            </div>
        </div>
    </section>
    <footer>
        <p>Designed by KELVIN</p>
    </footer>
</body>
</html>
```
# contact.html
```html
{% load static %}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Little Lemon - Contact Us</title>
    <link rel="stylesheet" href="{% static 'css/style.css' %}">
</head>
<body>
    <header>
        <div class="logo">LITTLE LEMON</div>
        <nav>
            <ul>
                <li><a href="{% url 'home' %}">Home</a></li>
                <li><a href="{% url 'menu' %}">Menu</a></li>
                <li><a href="{% url 'administration' %}">Administration</a></li>
                <li><a href="{% url 'contact' %}">Contact Us</a></li>
            </ul>
        </nav>
    </header>
    <section class="contact">
        <h1>Contact Us</h1>
        <div class="contact-info">
            <p><strong>Address:</strong> India, Thandalam, Tamil Nadu</p>
            <p><strong>Phone:</strong> 9876543210</p>
            <p><strong>Email:</strong> contact@hotelparadise.com</p>
        </div>
        <form method="POST" action="{% url 'contact' %}">
            {% csrf_token %}
            <h2>Send Us a Message</h2>
            <div class="form-group">
                <label for="name">Name:</label>
                <input type="text" id="name" name="name" required>
            </div>
            <div class="form-group">
                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required>
            </div>
            <div class="form-group">
                <label for="message">Message:</label>
                <textarea id="message" name="message" rows="5" required></textarea>
            </div>
            <button type="submit">Submit</button>
        </form>
    </section>
    <footer>
        <p>Designed by KELVIN</p>
    </footer>
</body>
</html>
```
# style.css
```css
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
}

header {
    background-color: #4CAF50;
    color: white;
    padding: 10px 20px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

header .logo {
    font-size: 24px;
    font-weight: bold;
}

header nav ul {
    list-style: none;
    margin: 0;
    padding: 0;
    display: flex;
}

header nav ul li {
    margin-left: 20px;
}

header nav ul li a {
    text-decoration: none;
    color: white;
    font-size: 16px;
}

header nav ul li a:hover {
    text-decoration: underline;
}

.banner {
    background: url('banner.jpg') no-repeat center center/cover;
    color: white;
    text-align: center;
    padding: 50px 20px;
}

.banner h1 {
    font-size: 36px;
}

.content {
    display: flex;
    justify-content: space-around;
    margin: 20px;
}

.card {
    background: #f9f9f9;
    border-radius: 10px;
    padding: 20px;
    text-align: center;
    width: 30%;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.card img {
    max-width: 100%;
    border-radius: 10px;
}

.card a {
    display: block;
    margin-top: 10px;
    color: #4CAF50;
    text-decoration: none;
    font-weight: bold;
}


footer {
    text-align: center;
    padding: 10px;
    background-color: #4CAF50;
    color: white;
    margin-top: 30px;
}


.menu h1, .menu h2 {
    text-align: center;
    color: #333;
    margin-bottom: 20px;
}

.menu-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;
    max-width: 1200px;
    margin: 0 auto 40px auto;
}

.menu-item {
    background: #f9f9f9;
    border-radius: 10px;
    text-align: center;
    padding: 20px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s;
}

.menu-item:hover {
    transform: translateY(-5px);
}

.menu-item img {
    max-width: 100%;
    height: auto;
    border-radius: 10px;
    margin-bottom: 15px;
}

.menu-item h3 {
    font-size: 18px;
    color: #4CAF50;
    margin-bottom: 10px;
}

.menu-item p {
    font-size: 16px;
    color: #777;
}

.administration {
    padding: 50px 20px;
    background-color: #f9f9f9;
}

.administration h1 {
    text-align: center;
    color: #333;
    margin-bottom: 10px;
}

.team-intro {
    text-align: center;
    color: #777;
    margin-bottom: 30px;
    font-size: 18px;
    max-width: 800px;
    margin: 0 auto 30px auto;
}

.team {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;
    max-width: 1200px;
    margin: 0 auto;
}

.team-member {
    background: #ffffff;
    border-radius: 10px;
    text-align: center;
    padding: 20px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s, box-shadow 0.3s;
}

.team-member:hover {
    transform: translateY(-5px);
    box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
}

.team-member img {
    width: 100%;
    height: auto;
    border-radius: 50%;
    margin-bottom: 15px;
}

.team-member h3 {
    font-size: 18px;
    color: #333;
    margin-bottom: 5px;
}

.team-member p {
    font-size: 16px;
    color: #555;
}


.contact {
    max-width: 600px;
    margin: 0 auto;
    padding: 20px;
    background-color: #f9f9f9;
    border-radius: 5px;
}

.form-group {
    margin-bottom: 15px;
}

label {
    display: block;
    font-weight: bold;
    margin-bottom: 5px;
}

input, textarea {
    width: 100%;
    padding: 10px;
    margin-bottom: 10px;
    border: 1px solid #ccc;
    border-radius: 5px;
}

button {
    background-color: #4CAF50;
    color: white;
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}

button:hover {
    background-color: #45a049;
}
```

## Step 7:
Publish the website in the given URL.

# PROGRAM:
# OUTPUT:
# RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
