<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sundar Sewa - Quality Services</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        /* CSS Styles */
        :root {
            --primary-color: #2c3e50;
            --secondary-color: #e74c3c;
            --text-color: #333;
            --light-color: #f8f9fa;
            --dark-color: #343a40;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            color: var(--text-color);
            line-height: 1.6;
        }

        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 15px;
        }

        .btn {
            display: inline-block;
            background: var(--secondary-color);
            color: #fff;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            text-decoration: none;
            font-weight: bold;
            transition: all 0.3s ease;
        }

        .btn:hover {
            background: #c0392b;
            transform: translateY(-2px);
        }

        .section-title {
            text-align: center;
            margin-bottom: 40px;
            color: var(--primary-color);
            position: relative;
            padding-bottom: 15px;
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 3px;
            background: var(--secondary-color);
        }

        /* Top Header */
        .top-header {
            background: var(--primary-color);
            color: #fff;
            padding: 8px 0;
            font-size: 14px;
        }

        .top-header .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .contact-info span {
            margin-right: 20px;
        }

        .contact-info i {
            margin-right: 5px;
        }

        .social-links a {
            color: #fff;
            margin-left: 15px;
            font-size: 16px;
            transition: color 0.3s ease;
        }

        .social-links a:hover {
            color: var(--secondary-color);
        }

        /* Main Header */
        .main-header {
            padding: 15px 0;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            position: sticky;
            top: 0;
            background: #fff;
            z-index: 1000;
        }

        .main-header .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            display: flex;
            align-items: center;
        }

        .logo img {
            height: 50px;
            margin-right: 10px;
        }

        .logo-text h1 {
            font-size: 1.5rem;
            color: var(--primary-color);
        }

        .logo-text span {
            color: var(--secondary-color);
        }

        .main-nav ul {
            display: flex;
            list-style: none;
        }

        .main-nav ul li a {
            text-decoration: none;
            color: var(--text-color);
            padding: 10px 15px;
            font-weight: 600;
            transition: all 0.3s ease;
        }

        .main-nav ul li a:hover,
        .main-nav ul li a.active {
            color: var(--primary-color);
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.6)), url('https://images.unsplash.com/photo-1600880292203-757bb62b4baf?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80');
            background-size: cover;
            background-position: center;
            height: 80vh;
            display: flex;
            align-items: center;
            text-align: center;
            color: #fff;
        }

        .hero-content {
            width: 100%;
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
        }

        .hero-content h1 {
            font-size: 2.5rem;
            margin-bottom: 20px;
            text-transform: uppercase;
        }

        .hero-content p {
            font-size: 1.2rem;
            margin-bottom: 30px;
        }

        /* Welcome Section */
        .welcome-section {
            padding: 80px 0;
            background: #fff;
        }

        .welcome-section .container {
            display: flex;
            align-items: center;
            gap: 40px;
        }

        .welcome-content {
            flex: 1;
        }

        .welcome-content h2 {
            color: var(--primary-color);
            margin-bottom: 20px;
            font-size: 2rem;
        }

        .welcome-content p {
            margin-bottom: 15px;
        }

        .welcome-image {
            flex: 1;
        }

        .welcome-image img {
            width: 100%;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }

        /* Services Section */
        .services-section {
            padding: 80px 0;
            background: var(--light-color);
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .service-card {
            background: #fff;
            padding: 30px;
            border-radius: 10px;
            text-align: center;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s ease;
        }

        .service-card:hover {
            transform: translateY(-10px);
        }

        .service-card i {
            font-size: 3rem;
            color: var(--primary-color);
            margin-bottom: 20px;
        }

        .service-card h3 {
            margin-bottom: 15px;
            color: var(--primary-color);
        }

        /* Testimonials Section */
        .testimonials-section {
            padding: 80px 0;
            background: #fff;
        }

        .testimonials-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .testimonial-card {
            background: var(--light-color);
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
        }

        .testimonial-card .quote {
            font-style: italic;
            margin-bottom: 20px;
        }

        .testimonial-author {
            display: flex;
            align-items: center;
        }

        .testimonial-author img {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            margin-right: 15px;
            object-fit: cover;
        }

        .author-info h4 {
            color: var(--primary-color);
            margin-bottom: 5px;
        }

        .author-info p {
            font-size: 0.9rem;
            color: #666;
        }

        /* Footer */
        .main-footer {
            background: var(--primary-color);
            color: #fff;
            padding: 60px 0 0;
        }

        .footer-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin-bottom: 40px;
        }

        .footer-col h3 {
            margin-bottom: 20px;
            font-size: 1.3rem;
            position: relative;
            padding-bottom: 10px;
        }

        .footer-col h3::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 50px;
            height: 2px;
            background: var(--secondary-color);
        }

        .footer-col p {
            margin-bottom: 15px;
        }

        .footer-col ul {
            list-style: none;
        }

        .footer-col ul li {
            margin-bottom: 10px;
        }

        .footer-col ul li a {
            color: #fff;
            text-decoration: none;
            transition: color 0.3s ease;
        }

        .footer-col ul li a:hover {
            color: var(--secondary-color);
        }

        .footer-col i {
            margin-right: 10px;
            color: var(--secondary-color);
        }

        .footer-bottom {
            background: rgba(0, 0, 0, 0.1);
            padding: 20px 0;
            text-align: center;
        }

        /* Responsive Styles */
        @media (max-width: 992px) {
            .welcome-section .container {
                flex-direction: column;
            }
            
            .welcome-content,
            .welcome-image {
                flex: none;
                width: 100%;
            }
        }

        @media (max-width: 768px) {
            .main-header .container {
                flex-direction: column;
            }
            
            .logo {
                margin-bottom: 15px;
            }
            
            .hero-content h1 {
                font-size: 2rem;
            }
            
            .top-header .container {
                flex-direction: column;
                text-align: center;
            }
            
            .contact-info {
                margin-bottom: 10px;
            }
            
            .main-nav ul {
                flex-wrap: wrap;
                justify-content: center;
            }
            
            .main-nav ul li {
                margin: 5px 0;
            }
        }

        @media (max-width: 576px) {
            .hero {
                height: 60vh;
            }
            
            .hero-content h1 {
                font-size: 1.8rem;
            }
            
            .section-title {
                font-size: 1.5rem;
            }
        }
    </style>
</head>
<body>
    <!-- Top Header -->
    <div class="top-header">
        <div class="container">
            <div class="contact-info">
                <span><i class="fas fa-phone"></i> +977-1-1234567</span>
                <span><i class="fas fa-envelope"></i> info@sundarsewa.com</span>
            </div>
            <div class="social-links">
                <a href="#"><i class="fab fa-facebook-f"></i></a>
                <a href="#"><i class="fab fa-twitter"></i></a>
                <a href="#"><i class="fab fa-instagram"></i></a>
                <a href="#"><i class="fab fa-linkedin-in"></i></a>
            </div>
        </div>
    </div>

    <!-- Main Header -->
    <header class="main-header">
        <div class="container">
            <div class="logo">
                <img src="https://drive.google.com/file/d/1ex88nfhT4QZI9bWxSavTj2q18bdeYh5P/view?usp=drive_link" alt="Sundar Sewa Logo">
                <div class="logo-text">
                    <h1><span>Sundar</span> Sewa</h1>
                </div>
            </div>
            <nav class="main-nav">
                <ul>
                    <li><a href="#" class="active">Home</a></li>
                    <li><a href="#">About Us</a></li>
                    <li><a href="#">Services</a></li>
                    <li><a href="#">Projects</a></li>
                    <li><a href="#">Testimonials</a></li>
                    <li><a href="#">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="hero-content">
            <h1>Your Trusted Service Partner</h1>
            <p>Quality services with reliability and professionalism</p>
            <a href="#" class="btn">Our Services</a>
        </div>
    </section>

    <!-- Welcome Section -->
    <section class="welcome-section">
        <div class="container">
            <div class="welcome-content">
                <h2>Welcome to Sundar Sewa</h2>
                <p>Sundar Sewa is a leading service provider committed to delivering excellence in every project we undertake. With years of experience and a team of dedicated professionals, we ensure customer satisfaction at every step.</p>
                <p>Our mission is to provide reliable, efficient, and high-quality services that meet the diverse needs of our clients while maintaining the highest standards of professionalism.</p>
                <a href="#" class="btn">Learn More</a>
            </div>
            <div class="welcome-image">
                <img src="https://images.unsplash.com/photo-1552664730-d307ca884978?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="Sundar Sewa Team">
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section class="services-section">
        <div class="container">
            <h2 class="section-title">Our Services</h2>
            <div class="services-grid">
                <div class="service-card">
                    <i class="fas fa-home"></i>
                    <h3>Home Services</h3>
                    <p>Comprehensive home maintenance and repair services to keep your living space in perfect condition.</p>
                </div>
                <div class="service-card">
                    <i class="fas fa-building"></i>
                    <h3>Commercial Services</h3>
                    <p>Professional services for businesses including maintenance, cleaning, and facility management.</p>
                </div>
                <div class="service-card">
                    <i class="fas fa-tools"></i>
                    <h3>Repair & Maintenance</h3>
                    <p>Expert repair services for electrical, plumbing, and other household systems.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials Section -->
    <section class="testimonials-section">
        <div class="container">
            <h2 class="section-title">What Our Clients Say</h2>
            <div class="testimonials-grid">
                <div class="testimonial-card">
                    <div class="quote">
                        "Sundar Sewa provided excellent service at a reasonable price. Their team was professional and completed the work ahead of schedule."
                    </div>
                    <div class="testimonial-author">
                        <img src="https://randomuser.me/api/portraits/women/45.jpg" alt="Client">
                        <div class="author-info">
                            <h4>Rita Sharma</h4>
                            <p>Kathmandu Resident</p>
                        </div>
                    </div>
                </div>
                <div class="testimonial-card">
                    <div class="quote">
                        "I've been using Sundar Sewa for all my maintenance needs for 3 years now. They're reliable and always do quality work."
                    </div>
                    <div class="testimonial-author">
                        <img src="https://randomuser.me/api/portraits/men/32.jpg" alt="Client">
                        <div class="author-info">
                            <h4>Rajesh Thapa</h4>
                            <p>Business Owner</p>
                        </div>
                    </div>
                </div>
                <div class="testimonial-card">
                    <div class="quote">
                        "The team went above and beyond to solve our plumbing emergency. Highly recommended for their quick response and expertise."
                    </div>
                    <div class="testimonial-author">
                        <img src="https://randomuser.me/api/portraits/women/68.jpg" alt="Client">
                        <div class="author-info">
                            <h4>Sunita Gurung</h4>
                            <p>Homeowner</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="main-footer">
        <div class="container">
            <div class="footer-grid">
                <div class="footer-col">
                    <h3>About Sundar Sewa</h3>
                    <p>Sundar Sewa is committed to providing quality services with reliability and professionalism since 2010.</p>
                </div>
                <div class="footer-col">
                    <h3>Quick Links</h3>
                    <ul>
                        <li><a href="#">Home</a></li>
                        <li><a href="#">About Us</a></li>
                        <li><a href="#">Services</a></li>
                        <li><a href="#">Projects</a></li>
                        <li><a href="#">Contact</a></li>
                    </ul>
                </div>
                <div class="footer-col">
                    <h3>Contact Us</h3>
                    <p><i class="fas fa-map-marker-alt"></i> New Baneshwor, Kathmandu, Nepal</p>
                    <p><i class="fas fa-phone"></i> +977-1-1234567, +977-9876543210</p>
                    <p><i class="fas fa-envelope"></i> info@sundarsewa.com</p>
                </div>
            </div>
        </div>
        <div class="footer-bottom">
            <div class="container">
                <p>&copy; 2023 Sundar Sewa. All Rights Reserved.</p>
            </div>
        </div>
    </footer>
</body>
</html>
