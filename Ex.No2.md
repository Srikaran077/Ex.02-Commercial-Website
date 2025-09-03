# Ex02 Commercial Website
## Date:03/09/25
## Reg no - 212223040206
## Name - Srikaran M
## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
commercial.html
```
<html>
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Football Academy</title>
    <link rel="stylesheet" href="style.css" />
</head>
<body>
    <header>
        <nav>
            <div class="logo">SANTIAGO BERNABEU FOOTBALL CLUB</div>
            <ul class="nav-menu">
                <li><a href="#home">Home</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
                <li><a href="#account">Account</a></li>
            </ul>
        </nav>
    </header>

    <section id="home" class="home">
        <h1>Welcome to madrid football coaching Academy</h1>
        <p>Learn football skills with professional coaches</p>
        <a href="#services" class="btn">Join Now</a>
    </section>

    <section id="services">
        <h2>Our Training Programs</h2>
        <div class="services-container">
            <div class="service-box">
                <div class="service-icon"></div>
                <h3>Kids Training</h3>
                <p>Fun football lessons for children aged 6-12 years</p>
                <div class="price">5000/month</div>
                <a href="#contact" class="btn">Sign Up</a>
            </div>
            <div class="service-box">
                <div class="service-icon"></div>
                <h3>Teen Training</h3>
                <p>Advanced skills for teenagers aged 13-18 years</p>
                <div class="price">8000/month</div>
                <a href="#contact" class="btn">Sign Up</a>
            </div>
            <div class="service-box">
                <div class="service-icon"></div>
                <h3>Private Lessons</h3>
                <p>One-on-one coaching sessions</p>
                <div class="price">400/hour</div>
                <a href="#contact" class="btn">Book Now</a>
            </div>
        </div>
    </section>

    <section id="about" class="about">
        <h2>About Us</h2>
        <div class="about-content">
            <div class="about-text">
                <p>Football Academy has been teaching football skills for over 10 years. We have the best coaches and training facilities.</p>
                <p>Our students have won many competitions and some have joined professional teams.</p>
                <p>We welcome players of all skill levels, from beginners to advanced players.</p>
            </div>
            <div class="about-image">
                <div class="stadium-image"></div>
            </div>
        </div>
    </section>

    <section id="contact">
        <h2>Contact Us</h2>
        <div class="contact-container">
            <div class="contact-info">
                <div class="contact-item">
                    <strong>📍 Address</strong>
                    madrid street<br />
                    Spain
                </div>
                <div class="contact-item">
                    <strong>📞 Phone</strong>
                    +919047385377
                </div>
                <div class="contact-item">
                    <strong>✉️ Email</strong>
                    info@santiagobernabeu.com
                </div>
                <div class="contact-item">
                    <strong>🕒 Hours</strong>
                    Monday - Friday: 9 AM - 8 PM<br />
                    Saturday - Sunday: 10 AM - 6 PM
                </div>
            </div>
            <div class="contact-form">
                <form>
                    <div class="form-group">
                        <label for="name">Your Name</label>
                        <input type="text" id="name" required />
                    </div>
                    <div class="form-group">
                        <label for="email">Email</label>
                        <input type="email" id="email" required />
                    </div>
                    <div class="form-group">
                        <label for="phone">Phone</label>
                        <input type="tel" id="phone" />
                    </div>
                    <div class="form-group">
                        <label for="message">Message</label>
                        <textarea id="message" rows="4"></textarea>
                    </div>
                    <button type="submit" class="btn">Send Message</button>
                </form>
            </div>
        </div>
    </section>

    <section id="account" class="account">
        <h2>Student Portal</h2>
        <div class="account-features">
            <div class="feature-box">
                <div class="feature-icon">📊</div>
                <h3>Track Progress</h3>
                <p>See your improvement and skills development</p>
            </div>
            <div class="feature-box">
                <div class="feature-icon">📅</div>
                <h3>Schedule</h3>
                <p>View and book your training sessions</p>
            </div>
            <div class="feature-box">
                <div class="feature-icon">👥</div>
                <h3>Community</h3>
                <p>Connect with other students and coaches</p>
            </div>
        </div>
        <div class="account-buttons">
            <a href="#" class="btn">Create Account</a>
            <a href="#" class="btn btn-outline">Login</a>
        </div>
    </section>

    <footer>
        <div class="footer-content">
            <div class="social-links">
                <a href="#">📘</a>
                <a href="#">🐦</a>
                <a href="#">📷</a>
                <a href="#">📺</a>
            </div>
            <p>&copy; 2025 Football Academy. All rights reserved.</p>
        </div>
    </footer>
</body>
</html>
```
style.css
```
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    color: #120202;
}

header {
    background-color: #0b0c0d;
    color: white;
    padding: 1rem 0;
}

nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

.logo {
    font-size: 24px;
    font-weight: bold;
}

.nav-menu {
    display: flex;
    list-style: none;
    gap: 30px;
}

.nav-menu a {
    color: white;
    text-decoration: none;
    padding: 10px 15px;
    border-radius: 5px;
}

.nav-menu a:hover {
    background-color: #0a3380;
}

section {
    padding: 60px 20px;
    max-width: 1200px;
    margin: 0 auto;
}

h1, h2 {
    text-align: center;
    margin-bottom: 30px;
    color: #042a62;
}

h1 {
    font-size: 48px;
}

h2 {
    font-size: 36px;
}

.home {
    background: linear-gradient(rgba(167, 117, 17, 0.8), rgba(11, 15, 19, 0.8)), url('images.jpeg') center/cover;
    color: white;
    text-align: center;
    min-height: 500px;
    display: flex;
    flex-direction: column;
    justify-content: center;
}

.home h1 {
    color: white;
}

.home p {
    font-size: 20px;
    margin-bottom: 30px;
}

.btn {
    background-color: #35b2ff;
    color: white;
    padding: 15px 30px;
    text-decoration: none;
    border-radius: 25px;
    font-size: 18px;
    font-weight: bold;
    display: inline-block;
}

.btn:hover {
    background-color: #2ba7e5;
}

.services-container {
    display: flex;
    gap: 30px;
    flex-wrap: wrap;
    justify-content: center;
}

.service-box {
    background-color: #f9f9f9;
    padding: 30px;
    border-radius: 10px;
    text-align: center;
    width: 300px;
    border: 2px solid #ddd;
}

.service-box:hover {
    border-color: #2c5aa0;
}

.service-icon {
    width: 100%;
    height: 150px;
    background-size: cover;
    background-position: center;
    border-radius: 8px;
    margin-bottom: 20px;
}

.service-box:nth-child(1) .service-icon {
    background-image: url('kids.jpg');
}

.service-box:nth-child(2) .service-icon {
    background-image: url('https://images.unsplash.com/photo-1574629810360-7efbbe195018?w=300&h=150&fit=crop');
}

.service-box:nth-child(3) .service-icon {
    background-image: url('https://images.unsplash.com/photo-1606107557195-0e29a4b5b4aa?w=300&h=150&fit=crop');
}

.service-box h3 {
    color: #2c5aa0;
    margin-bottom: 15px;
}

.price {
    font-size: 24px;
    color: #3589ff;
    font-weight: bold;
    margin: 15px 0;
}

.about {
    background: linear-gradient(rgba(245, 244, 244, 0.95), rgba(17, 10, 10, 0.95)), url('IMG-20250718-WA0017.jpg') center/cover;
}

.about-content {
    display: flex;
    gap: 40px;
    align-items: center;
}

.about-text {
    flex: 1;
}

.about-text p {
    margin-bottom: 20px;
    font-size: 16px;
}

.about-image {
    flex: 1;
    text-align: center;
}

.stadium-image {
    width: 400px;
    height: 250px;
    background-image: url('IMG-20250718-WA0017.jpg');
    background-size: cover;
    background-position: center;
    border-radius: 15px;
    box-shadow: 0 5px 15px rgba(230, 220, 72, 0.3);
}

.contact-container {
    display: flex;
    gap: 40px;
}

.contact-info {
    flex: 1;
}

.contact-item {
    margin-bottom: 25px;
    padding: 20px;
    background-color: #f9f9f9;
    border-radius: 8px;
}

.contact-item strong {
    color: #2c5aa0;
    display: block;
    margin-bottom: 5px;
}

.contact-form {
    flex: 1;
}

.form-group {
    margin-bottom: 20px;
}

label {
    display: block;
    margin-bottom: 5px;
    color: #2c5aa0;
    font-weight: bold;
}

input, textarea {
    width: 100%;
    padding: 12px;
    border: 2px solid #ddd;
    border-radius: 5px;
    font-size: 16px;
}

input:focus, textarea:focus {
    border-color: #2c5aa0;
    outline: none;
}

.account {
    background-color: #f5f5f5;
}

.account-features {
    display: flex;
    gap: 30px;
    justify-content: center;
    flex-wrap: wrap;
}

.feature-box {
    background-color: #2c5aa0;
    color: white;
    padding: 30px;
    border-radius: 10px;
    text-align: center;
    width: 250px;
}

.feature-icon {
    font-size: 50px;
    margin-bottom: 15px;
}

.account-buttons {
    text-align: center;
    margin-top: 40px;
}

.btn-outline {
    background-color: transparent;
    color: #2c5aa0;
    border: 2px solid #2c5aa0;
    margin-left: 15px;
}

.btn-outline:hover {
    background-color: #2c5aa0;
    color: white;
}

footer {
    background-color: #110a0a;
    color: white;
    padding: 40px 20px 20px;
    text-align: center;
}

.footer-content {
    max-width: 1200px;
    margin: 0 auto;
}

.social-links {
    margin-bottom: 20px;
}

.social-links a {
    color: white;
    font-size: 30px;
    margin: 0 15px;
    text-decoration: none;
}

.social-links a:hover {
    color: #353cff;
}

@media (max-width: 768px) {
    .nav-menu {
        flex-direction: column;
        gap: 10px;
    }

    .services-container,
    .about-content,
    .contact-container,
    .account-features {
        flex-direction: column;
    }

    h1 {
        font-size: 36px;
    }

    h2 {
        font-size: 28px;
    }
}
```

## OUTPUT

<img width="1920" height="1200" alt="Screenshot 2025-08-29 234752" src="https://github.com/user-attachments/assets/9f55145f-15ef-4bb7-8a65-81df715336f8" />

<img width="1920" height="1200" alt="Screenshot 2025-08-29 234805" src="https://github.com/user-attachments/assets/79f20210-9b91-4b82-b050-f9ccd030f57a" />

<img width="1920" height="1200" alt="Screenshot 2025-08-29 234817" src="https://github.com/user-attachments/assets/efa44ea3-e7a7-4ff9-b290-eb2ea806e42c" />

<img width="1920" height="1200" alt="Screenshot 2025-08-29 234900" src="https://github.com/user-attachments/assets/998f1ef0-5940-4f7f-8666-d99ae83726b2" />

<img width="1920" height="1200" alt="Screenshot 2025-08-29 234912" src="https://github.com/user-attachments/assets/cbb10953-0fd0-4472-8914-9dbce6e9725b" />

## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
