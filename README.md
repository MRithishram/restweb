# Ex.06 Restaurant Website
## Date:04.01.2026

## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:

Include your program

contact.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Savory Bistro - Contact Us</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <nav>
        <ul>
            <li><a href="index.html">Home</a></li>
            <li><a href="menu.html">Menu</a></li>
            <li><a href="contact.html">Contact</a></li>
            <li><a href="login.html">Login</a></li>
        </ul>
    </nav>

    <div class="contact-page">
        <div class="contact-header">
            <h1>Get In Touch</h1>
            <p>We'd love to hear from you</p>
        </div>

        <div class="contact-container">
            <div class="contact-info">
                <div class="info-card">
                    <div class="info-icon">📍</div>
                    <h3>Visit Us</h3>
                    <p>123 Culinary Avenue<br>Food District, City 12345</p>
                </div>

                <div class="info-card">
                    <div class="info-icon">📞</div>
                    <h3>Call Us</h3>
                    <p>+1 (555) 123-4567<br>+1 (555) 987-6543</p>
                </div>

                <div class="info-card">
                    <div class="info-icon">✉️</div>
                    <h3>Email Us</h3>
                    <p>info@crfoods.com<br>reservations@crfoods.com</p>
                </div>

                <div class="info-card">
                    <div class="info-icon">🕒</div>
                    <h3>Opening Hours</h3>
                    <p>Mon - Fri: 11:00 AM - 10:00 PM<br>
                    Sat - Sun: 10:00 AM - 11:00 PM</p>
                </div>
            </div>

            <div class="contact-form-container">
                <h2>Send Us a Message</h2>
                <form onsubmit="handleContact(event)" class="contact-form">
                    <div class="form-row">
                        <div class="form-group">
                            <label for="name">Full Name</label>
                            <input type="text" id="name" placeholder="John Doe" required>
                        </div>

                        <div class="form-group">
                            <label for="email">Email Address</label>
                            <input type="email" id="email" placeholder="john@example.com" required>
                        </div>
                    </div>

                    <div class="form-row">
                        <div class="form-group">
                            <label for="phone">Phone Number</label>
                            <input type="tel" id="phone" placeholder="+1 (555) 123-4567">
                        </div>

                        <div class="form-group">
                            <label for="subject">Subject</label>
                            <select id="subject" required>
                                <option value="">Select a topic</option>
                                <option value="reservation">Reservation</option>
                                <option value="feedback">Feedback</option>
                                <option value="catering">Catering</option>
                                <option value="other">Other</option>
                            </select>
                        </div>
                    </div>

                    <div class="form-group">
                        <label for="message">Message</label>
                        <textarea id="message" rows="6" placeholder="Tell us how we can help you..." required></textarea>
                    </div>

                    <button type="submit" class="submit-button">Send Message</button>
                </form>
            </div>
        </div>

        <div class="map-container">
            <h2>Find Us Here</h2>
            <div class="map-placeholder">
                <div class="map-icon">🗺️</div>
                <p>Map Location</p>
            </div>
        </div>
    </div>

    <footer>
        <p>&copy; 2025 CR Foods. All rights reserved.</p>
    </footer>

    <script>
        function handleContact(e) {
            e.preventDefault();
            const name = document.getElementById('name').value;
            const email = document.getElementById('email').value;
            const subject = document.getElementById('subject').value;
            alert('Thank you for contacting us, ' + name + '! We will get back to you soon at ' + email);
        }
    </script>
</body>
</html>

index.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CR Restaurant - Home</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <nav>
        <ul>
            <li><a href="index.html">Home</a></li>
            <li><a href="menu.html">Menu</a></li>
            <li><a href="contacts.html">Contact</a></li>
            <li><a href="login.html">Login</a></li>
        </ul>
    </nav>

    <section class="hero">
        <div class="hero-content">
            <h1>The One Piece</h1>
            <p>The real life One Piece at your taste buds</p>
            <a href="menu.html" class="cta-button">Explore Our Menu</a>
        </div>
    </section>

    <section class="features">
        <div class="feature-card">
            <div class="feature-icon">🍽️</div>
            <h3>Fresh Ingredients</h3>
            <p>We source only the finest, locally-grown ingredients to create dishes that burst with authentic flavors and nutrition.</p>
        </div>
        <div class="feature-card">
            <div class="feature-icon">👨‍🍳</div>
            <h3>Expert Chefs</h3>
            <p>Our award-winning culinary team brings decades of experience and passion to every plate they create.</p>
        </div>
        <div class="feature-card">
            <div class="feature-icon">⭐</div>
            <h3>5-Star Service</h3>
            <p>From the moment you arrive until your last bite, our dedicated staff ensures an unforgettable dining experience.</p>
        </div>
    </section>

    <footer>
        <p>&copy; 2025 CR Foods. All rights reserved.</p>
    </footer>
</body>
</html>

login.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Savory Bistro - Login</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <nav>
        <ul>
            <li><a href="index.html">Home</a></li>
            <li><a href="menu.html">Menu</a></li>
            <li><a href="contact.html">Contact</a></li>
            <li><a href="login.html">Login</a></li>
        </ul>
    </nav>

    <div class="login-page">
        <div class="login-container">
            <div class="login-header">
                <h1>Welcome Back</h1>
                <p>Login to your account</p>
            </div>

            <form onsubmit="handleLogin(event)">
                <div class="form-group">
                    <label for="email">Email Address</label>
                    <input type="email" id="email" placeholder="Enter your email" required>
                </div>

                <div class="form-group">
                    <label for="password">Password</label>
                    <input type="password" id="password" placeholder="Enter your password" required>
                </div>

                <button type="submit" class="login-button">Login</button>

                <div class="login-footer">
                    <p>Don't have an account? <a href="#">Sign up</a></p>
                    <p><a href="#">Forgot password?</a></p>
                </div>
            </form>
        </div>
    </div>

    <script>
        function handleLogin(e) {
            e.preventDefault();
            const email = document.getElementById('email').value;
            alert('Login functionality would be connected to backend. Email: ' + email);
        }
    </script>
</body>
</html>

menu.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Savory Bistro - Menu</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <nav>
        <ul>
            <li><a href="index.html">Home</a></li>
            <li><a href="menu.html">Menu</a></li>
            <li><a href="contact.html">Contact</a></li>
            <li><a href="login.html">Login</a></li>
        </ul>
    </nav>
    
    <div class="menu-page">
        <div class="menu-header">
            <h1>Our Signature Dishes</h1>
            <p>Crafted by world renowned chefs</p>
        </div>

        <div class="menu-grid">
            <div class="menu-item">
                <div class="menu-item-image">
                    <img src="images.jpg">
                </div>
                <div class="menu-item-content">
                    <h3>Beef Wellington</h3>
                    <p>beef tenderloin coated in mushroom duxelles, pâté (optional), and prosciutto or ham, all wrapped in flaky puff pastry and baked until golden brown, revealing tender meat and savory layers when sliced</p>
                    <div class="price">$32.99</div>
                </div>
            </div>

            <div class="menu-item">
                <div class="menu-item-image menu-item-2">
                    <img src="alfredo.jpg">
                </div>
                <div class="menu-item-content">
                    <h3>Fettuccine Alfredo</h3>
                    <p>Fettuccine Alfredo with Romano and Parmesan cheeses, cream, and butter</p>
                    <div class="price">$24.99</div>
                </div>
            </div>

            <div class="menu-item">
                <div class="menu-item-image menu-item-3">
                    <img src="Hawaiian-Pizza-7.jpg">
                </div>
                <div class="menu-item-content">
                    <h3>Hawaiian Pizza</h3>
                    <p> topped with pineapple, tomato sauce, mozzarella cheese and bacon</p>
                    <div class="price">$45.99</div>
                </div>
            </div>

            <div class="menu-item">
                <div class="menu-item-image menu-item-4">
                    <img src="soba.webp">
                </div>
                <div class="menu-item-content">
                    <h3>Japanese Soba Noodles</h3>
                    <p>strong broth with porkbelly slices and half boield egg</p>
                    <div class="price">$38.99</div>
                </div>
            </div>

            <div class="menu-item">
                <div class="menu-item-image menu-item-5">
                    <img src="mousse.jpg">
                </div>
                <div class="menu-item-content">
                    <h3>Chocolate itallian mousse</h3>
                    <p>Thick soft dark chocoloate,with amazing texture </p>
                    <div class="price">$12.99</div>
                </div>
            </div>

            <div class="menu-item">
                <div class="menu-item-image menu-item-6">
                    <img src="Tiramisu_1200x800.jpg">
                </div>
                <div class="menu-item-content">
                    <h3>Thiramisu</h3>
                    <p>an Italian dessert made with coffee-soaked ladyfingers covered with a cream of egg yolks, sugar, and mascarpone and topped with cocoa powder. </p>
                    <div class="price">$15-65</div>
                </div>
            </div>
        </div>
    </div>

    <footer>
        <p>&copy; 2025 CR Foods. All rights reserved.</p>
    </footer>
</body>
</html>
## OUTPUT:
Include the Screenshot

<img width="1041" height="524" alt="Screenshot 2026-01-04 232337" src="https://github.com/user-attachments/assets/cd4962af-c3b0-4dcd-ba2c-34c6903fdebc" />

<img width="998" height="815" alt="Screenshot 2026-01-04 232427" src="https://github.com/user-attachments/assets/72da465f-142c-4464-a010-c5c8315a5acd" />
<img width="1030" height="493" alt="Screenshot 2026-01-04 232437" src="https://github.com/user-attachments/assets/a67e4df9-4f98-45bc-9329-26b70d82eccb" />

## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
