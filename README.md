<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>RunSmartX | Premium Facebook Advertising Agency</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        :root {
            --primary: #4361ee;
            --secondary: #3f37c9;
            --accent: #4cc9f0;
            --light: #f8f9fa;
            --dark: #212529;
            --success: #4bb543;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: var(--light);
            color: var(--dark);
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Header & Logo */
        header {
            background-color: white;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            position: sticky;
            top: 0;
            z-index: 100;
        }
        
        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
        }
        
        .logo {
            display: flex;
            align-items: center;
            text-decoration: none;
        }
        
        .logo-icon {
            width: 40px;
            height: 40px;
            background-color: var(--primary);
            border-radius: 8px;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-right: 10px;
            color: white;
            font-weight: bold;
            font-size: 20px;
        }
        
        .logo-text {
            font-size: 24px;
            font-weight: 700;
            color: var(--dark);
        }
        
        .logo-text span {
            color: var(--primary);
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 30px;
        }
        
        nav ul li a {
            text-decoration: none;
            color: var(--dark);
            font-weight: 500;
            transition: color 0.3s;
        }
        
        nav ul li a:hover {
            color: var(--primary);
        }
        
        /* Hero Section */
        .hero {
            padding: 80px 0;
            background: linear-gradient(135deg, rgba(67, 97, 238, 0.1) 0%, rgba(76, 201, 240, 0.1) 100%);
        }
        
        .hero-content {
            display: flex;
            align-items: center;
            justify-content: space-between;
        }
        
        .hero-text {
            flex: 1;
            padding-right: 40px;
        }
        
        .hero-image {
            flex: 1;
            text-align: center;
        }
        
        .hero-image img {
            max-width: 100%;
            border-radius: 10px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
        }
        
        h1 {
            font-size: 48px;
            margin-bottom: 20px;
            color: var(--dark);
        }
        
        h1 span {
            color: var(--primary);
        }
        
        .subtitle {
            font-size: 20px;
            color: #555;
            margin-bottom: 30px;
        }
        
        .cta-button {
            display: inline-block;
            background-color: var(--primary);
            color: white;
            padding: 15px 30px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            transition: background-color 0.3s, transform 0.3s;
            margin-right: 15px;
            margin-bottom: 15px;
        }
        
        .cta-button:hover {
            background-color: var(--secondary);
            transform: translateY(-3px);
        }
        
        .secondary-button {
            background-color: transparent;
            color: var(--primary);
            border: 2px solid var(--primary);
        }
        
        .secondary-button:hover {
            background-color: var(--primary);
            color: white;
        }
        
        /* Features Section */
        .features {
            padding: 80px 0;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 60px;
        }
        
        .section-title h2 {
            font-size: 36px;
            color: var(--dark);
            margin-bottom: 15px;
        }
        
        .section-title p {
            color: #666;
            max-width: 700px;
            margin: 0 auto;
        }
        
        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .feature-card {
            background-color: white;
            border-radius: 10px;
            padding: 30px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s, box-shadow 0.3s;
        }
        
        .feature-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.1);
        }
        
        .feature-icon {
            width: 60px;
            height: 60px;
            background-color: rgba(67, 97, 238, 0.1);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 20px;
            color: var(--primary);
            font-size: 24px;
        }
        
        .feature-card h3 {
            font-size: 22px;
            margin-bottom: 15px;
            color: var(--dark);
        }
        
        /* Contact Form */
        .contact {
            padding: 80px 0;
            background-color: white;
        }
        
        .contact-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .contact-text {
            flex: 1;
            padding-right: 40px;
        }
        
        .contact-form {
            flex: 1;
            background-color: var(--light);
            padding: 40px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
        }
        
        .form-group {
            margin-bottom: 20px;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-weight: 500;
            color: var(--dark);
        }
        
        .form-control {
            width: 100%;
            padding: 12px 15px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 16px;
            transition: border-color 0.3s;
        }
        
        .form-control:focus {
            outline: none;
            border-color: var(--primary);
        }
        
        textarea.form-control {
            min-height: 120px;
            resize: vertical;
        }
        
        .submit-btn {
            background-color: var(--primary);
            color: white;
            border: none;
            padding: 15px 30px;
            border-radius: 5px;
            font-size: 16px;
            font-weight: 600;
            cursor: pointer;
            transition: background-color 0.3s;
            width: 100%;
        }
        
        .submit-btn:hover {
            background-color: var(--secondary);
        }
        
        /* Testimonials */
        .testimonials {
            padding: 80px 0;
            background: linear-gradient(135deg, rgba(67, 97, 238, 0.1) 0%, rgba(76, 201, 240, 0.1) 100%);
        }
        
        .testimonials-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .testimonial-card {
            background-color: white;
            border-radius: 10px;
            padding: 30px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
        }
        
        .testimonial-text {
            font-style: italic;
            margin-bottom: 20px;
            color: #555;
        }
        
        .testimonial-author {
            display: flex;
            align-items: center;
        }
        
        .author-avatar {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            background-color: #eee;
            margin-right: 15px;
            overflow: hidden;
        }
        
        .author-info h4 {
            font-size: 18px;
            margin-bottom: 5px;
            color: var(--dark);
        }
        
        .author-info p {
            color: #777;
            font-size: 14px;
        }
        
        /* Footer */
        footer {
            background-color: var(--dark);
            color: white;
            padding: 60px 0 20px;
        }
        
        .footer-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 40px;
            margin-bottom: 40px;
        }
        
        .footer-logo {
            display: flex;
            align-items: center;
            margin-bottom: 20px;
        }
        
        .footer-logo-icon {
            width: 40px;
            height: 40px;
            background-color: var(--accent);
            border-radius: 8px;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-right: 10px;
            color: var(--dark);
            font-weight: bold;
            font-size: 20px;
        }
        
        .footer-logo-text {
            font-size: 20px;
            font-weight: 700;
            color: white;
        }
        
        .footer-logo-text span {
            color: var(--accent);
        }
        
        .footer-about p {
            color: #bbb;
            margin-bottom: 20px;
        }
        
        .social-links a {
            display: inline-block;
            width: 40px;
            height: 40px;
            background-color: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            color: white;
            text-align: center;
            line-height: 40px;
            margin-right: 10px;
            transition: background-color 0.3s;
        }
        
        .social-links a:hover {
            background-color: var(--accent);
            color: var(--dark);
        }
        
        .footer-links h3 {
            font-size: 18px;
            margin-bottom: 20px;
            color: white;
        }
        
        .footer-links ul {
            list-style: none;
        }
        
        .footer-links ul li {
            margin-bottom: 10px;
        }
        
        .footer-links ul li a {
            color: #bbb;
            text-decoration: none;
            transition: color 0.3s;
        }
        
        .footer-links ul li a:hover {
            color: var(--accent);
        }
        
        .footer-contact p {
            display: flex;
            align-items: center;
            color: #bbb;
            margin-bottom: 15px;
        }
        
        .footer-contact p i {
            margin-right: 10px;
            color: var(--accent);
        }
        
        .copyright {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            color: #bbb;
            font-size: 14px;
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            .hero-content, .contact-container {
                flex-direction: column;
            }
            
            .hero-text, .contact-text {
                padding-right: 0;
                margin-bottom: 40px;
                text-align: center;
            }
            
            h1 {
                font-size: 36px;
            }
            
            .subtitle {
                font-size: 18px;
            }
            
            .cta-buttons {
                display: flex;
                flex-direction: column;
                align-items: center;
            }
            
            .cta-button {
                margin-right: 0;
                margin-bottom: 15px;
                width: 100%;
                text-align: center;
            }
            
            nav ul {
                display: none;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container header-container">
            <a href="#" class="logo">
                <div class="logo-icon">RX</div>
                <div class="logo-text">Run<span>SmartX</span></div>
            </a>
            <nav>
                <ul>
                    <li><a href="#features">Why Us</a></li>
                    <li><a href="#testimonials">Results</a></li>
                    <li><a href="#contact">Get Started</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="container hero-content">
            <div class="hero-text">
                <h1>Grow Your Business With <span>Facebook Ads</span> That Actually Work</h1>
                <p class="subtitle">Trusted by 500+ businesses to increase leads and sales through strategic Facebook advertising campaigns.</p>
                <div class="cta-buttons">
                    <a href="#contact" class="cta-button">Get Your Free Audit</a>
                    <a href="#features" class="cta-button secondary-button">Learn More</a>
                </div>
            </div>
            <div class="hero-image">
                <img src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?ixlib=rb-1.2.1&auto=format&fit=crop&w=600&q=80" alt="Facebook Advertising">
            </div>
        </div>
    </section>

    <!-- Features Section -->
    <section class="features" id="features">
        <div class="container">
            <div class="section-title">
                <h2>Why Choose RunSmartX?</h2>
                <p>We combine data-driven strategies with creative excellence to deliver Facebook ad campaigns that convert.</p>
            </div>
            <div class="features-grid">
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-chart-line"></i>
                    </div>
                    <h3>Proven Results</h3>
                    <p>Our campaigns consistently deliver 3-5x ROAS for our clients across various industries.</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-user-shield"></i>
                    </div>
                    <h3>Transparent Reporting</h3>
                    <p>Get real-time access to your campaign performance with our easy-to-understand dashboards.</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-lightbulb"></i>
                    </div>
                    <h3>Strategic Approach</h3>
                    <p>We don't just run ads - we build comprehensive marketing funnels tailored to your business.</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-headset"></i>
                    </div>
                    <h3>Dedicated Support</h3>
                    <p>Your success manager is always available to answer questions and optimize campaigns.</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-fingerprint"></i>
                    </div>
                    <h3>Custom Audiences</h3>
                    <p>We leverage advanced targeting to reach your ideal customers at the right moment.</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-money-bill-wave"></i>
                    </div>
                    <h3>Risk-Free Trial</h3>
                    <p>Try our services with our 30-day money-back guarantee if we don't deliver results.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Form -->
    <section class="contact" id="contact">
        <div class="container contact-container">
            <div class="contact-text">
                <h2>Ready to Scale Your Business?</h2>
                <p>Fill out the form and one of our Facebook ad experts will contact you within 24 hours to discuss how we can help grow your business.</p>
                <ul style="margin-top: 30px; list-style-type: none;">
                    <li style="margin-bottom: 15px; display: flex; align-items: center;">
                        <i class="fas fa-check-circle" style="color: var(--primary); margin-right: 10px; font-size: 20px;"></i>
                        <span>Free Facebook ad account audit</span>
                    </li>
                    <li style="margin-bottom: 15px; display: flex; align-items: center;">
                        <i class="fas fa-check-circle" style="color: var(--primary); margin-right: 10px; font-size: 20px;"></i>
                        <span>Custom strategy session</span>
                    </li>
                    <li style="margin-bottom: 15px; display: flex; align-items: center;">
                        <i class="fas fa-check-circle" style="color: var(--primary); margin-right: 10px; font-size: 20px;"></i>
                        <span>No obligation quote</span>
                    </li>
                </ul>
            </div>
            <div class="contact-form">
                <form id="leadForm">
                    <div class="form-group">
                        <label for="name">Your Name</label>
                        <input type="text" id="name" class="form-control" required>
                    </div>
                    <div class="form-group">
                        <label for="email">Email Address</label>
                        <input type="email" id="email" class="form-control" required>
                    </div>
                    <div class="form-group">
                        <label for="phone">Phone Number</label>
                        <input type="tel" id="phone" class="form-control" required>
                    </div>
                    <div class="form-group">
                        <label for="business">Business Name</label>
                        <input type="text" id="business" class="form-control" required>
                    </div>
                    <div class="form-group">
                        <label for="message">How Can We Help You?</label>
                        <textarea id="message" class="form-control"></textarea>
                    </div>
                    <button type="submit" class="submit-btn">Get Your Free Strategy Call</button>
                </form>
            </div>
        </div>
    </section>

    <!-- Testimonials -->
    <section class="testimonials" id="testimonials">
        <div class="container">
            <div class="section-title">
                <h2>What Our Clients Say</h2>
                <p>Don't just take our word for it - here's what our clients have to say about working with RunSmartX.</p>
            </div>
            <div class="testimonials-grid">
                <div class="testimonial-card">
                    <div class="testimonial-text">
                        "RunSmartX transformed our Facebook ad performance. We went from spending $5k/month with mediocre results to $20k/month with 4.5x ROAS consistently. Their team is worth every penny."
                    </div>
                    <div class="testimonial-author">
                        <div class="author-avatar">
                            <img src="https://randomuser.me/api/portraits/women/45.jpg" alt="Sarah Johnson" style="width: 100%; height: 100%; object-fit: cover;">
                        </div>
                        <div class="author-info">
                            <h4>Sarah Johnson</h4>
                            <p>CEO, Beauty Essentials</p>
                        </div>
                    </div>
                </div>
                <div class="testimonial-card">
                    <div class="testimonial-text">
                        "After wasting money with other agencies, we finally found RunSmartX. They took the time to understand our business and built campaigns that actually convert. Our sales are up 300% in 6 months."
                    </div>
                    <div class="testimonial-author">
                        <div class="author-avatar">
                            <img src="https://randomuser.me/api/portraits/men/32.jpg" alt="Michael Chen" style="width: 100%; height: 100%; object-fit: cover;">
                        </div>
                        <div class="author-info">
                            <h4>Michael Chen</h4>
                            <p>Founder, TechGadgets</p>
                        </div>
                    </div>
                </div>
                <div class="testimonial-card">
                    <div class="testimonial-text">
                        "The transparency and communication from RunSmartX is unmatched. We know exactly where every dollar is spent and see the results in real-time. They've become an extension of our marketing team."
                    </div>
                    <div class="testimonial-author">
                        <div class="author-avatar">
                            <img src="https://randomuser.me/api/portraits/women/68.jpg" alt="Emily Rodriguez" style="width: 100%; height: 100%; object-fit: cover;">
                        </div>
                        <div class="author-info">
                            <h4>Emily Rodriguez</h4>
                            <p>Marketing Director, FitLife</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-container">
                <div class="footer-about">
                    <div class="footer-logo">
                        <div class="footer-logo-icon">RX</div>
                        <div class="footer-logo-text">Run<span>SmartX</span></div>
                    </div>
                    <p>We help businesses of all sizes maximize their Facebook advertising ROI through data-driven strategies and creative excellence.</p>
                    <div class="social-links">
                        <a href="#"><i class="fab fa-facebook-f"></i></a>
                        <a href="#"><i class="fab fa-instagram"></i></a>
                        <a href="#"><i class="fab fa-linkedin-in"></i></a>
                        <a href="#"><i class="fab fa-twitter"></i></a>
                    </div>
                </div>
                <div class="footer-links">
                    <h3>Quick Links</h3>
                    <ul>
                        <li><a href="#features">Our Services</a></li>
                        <li><a href="#testimonials">Case Studies</a></li>
                        <li><a href="#contact">Get Started</a></li>
                        <li><a href="#">Blog</a></li>
                        <li><a href="#">Careers</a></li>
                    </ul>
                </div>
                <div class="footer-links">
                    <h3>Services</h3>
                    <ul>
                        <li><a href="#">Facebook Ads Management</a></li>
                        <li><a href="#">Instagram Ads</a></li>
                        <li><a href="#">Audience Research</a></li>
                        <li><a href="#">Creative Production</a></li>
                        <li><a href="#">Funnel Optimization</a></li>
                    </ul>
                </div>
                <div class="footer-contact">
                    <h3>Contact Us</h3>
                    <p><i class="fas fa-map-marker-alt"></i> 123 Business Ave, Suite 200, San Francisco, CA</p>
                    <p><i class="fas fa-phone-alt"></i> (555) 123-4567</p>
                    <p><i class="fas fa-envelope"></i> hello@runsmartx.com</p>
                    <p><i class="fas fa-clock"></i> Mon-Fri: 9AM - 6PM</p>
                </div>
            </div>
            <div class="copyright">
                <p>&copy; 2023 RunSmartX. All Rights Reserved. | <a href="#" style="color: var(--accent);">Privacy Policy</a> | <a href="#" style="color: var(--accent);">Terms of Service</a></p>
            </div>
        </div>
    </footer>

    <script>
        // Form submission handling
        document.getElementById('leadForm').addEventListener('submit', function(e) {
            e.preventDefault();
            
            // Get form values
            const name = document.getElementById('name').value;
            const email = document.getElementById('email').value;
            
            // Here you would typically send the data to your server
            // For this example, we'll just show an alert
            alert(`Thank you, ${name}! We've received your information and will contact you at ${email} shortly.`);
            
            // Reset the form
            this.reset();
            
            // Scroll to top for better UX
            window.scrollTo({
                top: 0,
                behavior: 'smooth'
            });
        });
        
        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>
