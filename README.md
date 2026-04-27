<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lumina Gems | Handcrafted Jewelry</title>
    <style>
        /* General Styles */
        :root {
            --primary: #d4af37; /* Gold */
            --dark: #1a1a1a;
            --light: #f9f9f9;
            --text: #333;
            --font-main: 'Helvetica Neue', sans-serif;
            --font-serif: 'Georgia', serif;
        }

        body {
            margin: 0;
            font-family: var(--font-main);
            color: var(--text);
            background-color: var(--light);
            line-height: 1.6;
        }

        h1, h2, h3 {
            font-family: var(--font-serif);
            color: var(--dark);
        }

        a { text-decoration: none; color: inherit; transition: 0.3s; }
        a:hover { color: var(--primary); }

        /* Navigation */
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1.5rem 5%;
            background: white;
            box-shadow: 0 2px 10px rgba(0,0,0,0.05);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .logo { font-size: 1.5rem; font-weight: bold; letter-spacing: 2px; }
        .nav-links a { margin-left: 2rem; font-size: 0.9rem; text-transform: uppercase; letter-spacing: 1px; }

        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(0,0,0,0.3), rgba(0,0,0,0.3)), url('https://images.unsplash.com/photo-1515562141207-7a88fb7ce338?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&q=80');
            background-size: cover;
            background-position: center;
            height: 80vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            color: white;
            padding: 0 20px;
        }

        .hero h1 { font-size: 3.5rem; margin-bottom: 1rem; color: white; }
        .hero p { font-size: 1.2rem; max-width: 600px; margin-bottom: 2rem; }
        
        .btn {
            padding: 12px 30px;
            background: var(--primary);
            color: white;
            border: none;
            font-size: 1rem;
            cursor: pointer;
            text-transform: uppercase;
            letter-spacing: 1px;
        }
        .btn:hover { background: #b8962e; }

        /* Products Section */
        .section { padding: 4rem 5%; }
        .section-title { text-align: center; margin-bottom: 3rem; font-size: 2.5rem; }

        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }

        .product-card {
            background: white;
            padding: 1rem;
            text-align: center;
            transition: transform 0.3s;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
        }

        .product-card:hover { transform: translateY(-5px); }
        
        .product-img {
            width: 100%;
            height: 250px;
            object-fit: cover;
            margin-bottom: 1rem;
        }

        .price { color: var(--primary); font-weight: bold; font-size: 1.1rem; }

        /* About & Contact */
        .about { background: white; text-align: center; }
        .contact { background: var(--dark); color: white; text-align: center; }
        .contact h2 { color: white; }
        .contact-form { max-width: 500px; margin: 0 auto; display: flex; flex-direction: column; gap: 1rem; }
        input, textarea { padding: 10px; border: none; width: 100%; box-sizing: border-box; }
        
        /* Footer */
        footer { text-align: center; padding: 2rem; background: #111; color: #888; font-size: 0.9rem; }

        /* Mobile */
        @media (max-width: 768px) {
            .hero h1 { font-size: 2.5rem; }
            .nav-links { display: none; } /* Simplified for demo */
        }
    </style>
</head>
<body>

    <!-- Navigation -->
    <nav>
        <div class="logo">LUMINA GEMS</div>
        <div class="nav-links">
            <a href="#home">Home</a>
            <a href="#collection">Collection</a>
            <a href="#about">About</a>
            <a href="#contact">Contact</a>
        </div>
    </nav>

    <!-- Hero -->
    <header class="hero" id="home">
        <h1>Timeless Elegance</h1>
        <p>Handcrafted jewelry designed to tell your unique story. Discover the perfect piece for every moment.</p>
        <a href="#collection" class="btn">Shop Collection</a>
    </header>

    <!-- Collection -->
    <section class="section" id="collection">
        <h2 class="section-title">New Arrivals</h2>
        <div class="product-grid">
            <!-- Product 1 -->
            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1599643478518-17488fbbcd75?auto=format&fit=crop&w=500&q=80" alt="Gold Necklace" class="product-img">
                <h3>Solaris Gold Necklace</h3>
                <p class="price">$145.00</p>
                <button class="btn" style="padding: 8px 15px; font-size: 0.8rem;">View Details</button>
            </div>
            <!-- Product 2 -->
            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1535632066927-ab7c9ab60908?auto=format&fit=crop&w=500&q=80" alt="Diamond Ring" class="product-img">
                <h3>Starlight Diamond Ring</h3>
                <p class="price">$299.00</p>
                <button class="btn" style="padding: 8px 15px; font-size: 0.8rem;">View Details</button>
            </div>
            <!-- Product 3 -->
            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1611591437281-460bfbe1220a?auto=format&fit=crop&w=500&q=80" alt="Pearl Earrings" class="product-img">
                <h3>Ocean Pearl Earrings</h3>
                <p class="price">$89.00</p>
                <button class="btn" style="padding: 8px 15px; font-size: 0.8rem;">View Details</button>
            </div>
            <!-- Product 4 -->
            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1602751584552-8ba73d60f8e1?auto=format&fit=crop&w=500&q=80" alt="Silver Bracelet" class="product-img">
                <h3>Midnight Silver Bracelet</h3>
                <p class="price">$120.00</p>
                <button class="btn" style="padding: 8px 15px; font-size: 0.8rem;">View Details</button>
            </div>
        </div>
    </section>

    <!-- About -->
    <section class="section about" id="about">
        <h2 class="section-title">Our Craft</h2>
        <p style="max-width: 700px; margin: 0 auto; font-size: 1.1rem;">
            At Lumina Gems, we believe jewelry is more than an accessory—it's a memory frozen in time. 
            Every piece is ethically sourced and meticulously handcrafted by artisans with decades of experience. 
            We combine traditional techniques with modern design to create heirlooms you'll cherish forever.
        </p>
    </section>

    <!-- Contact -->
    <section class="section contact" id="contact">
        <h2 class="section-title">Get in Touch</h2>
        <p style="margin-bottom: 2rem;">Have a custom request? We'd love to hear from you.</p>
        <form class="contact-form">
            <input type="text" placeholder="Your Name" required>
            <input type="email" placeholder="Your Email" required>
            <textarea rows="5" placeholder="Tell us about your idea..." required></textarea>
            <button type="submit" class="btn">Send Message</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2026 Lumina Gems. All rights reserved.</p>
    </footer>

</body>
</html>
