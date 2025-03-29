# sang
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SANG SURYA LANDSCAPE - Jasa Desain dan Pembuatan Taman Profesional</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        :root {
            --primary: #2e7d32;
            --secondary: #81c784;
            --light: #f1f8e9;
            --dark: #1b5e20;
            --white: #ffffff;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            line-height: 1.6;
            color: #333;
        }
        
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 15px;
        }
        
        /* Header */
        header {
            background-color: var(--white);
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            position: fixed;
            width: 100%;
            z-index: 100;
        }
        
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
        }
        
        .logo {
            font-size: 24px;
            font-weight: 700;
            color: var(--primary);
            text-decoration: none;
        }
        
        .logo span {
            color: var(--secondary);
        }
        
        .nav-links {
            display: flex;
            list-style: none;
        }
        
        .nav-links li {
            margin-left: 30px;
        }
        
        .nav-links a {
            text-decoration: none;
            color: var(--dark);
            font-weight: 500;
            transition: color 0.3s;
        }
        
        .nav-links a:hover {
            color: var(--primary);
        }
        
        .cta-button {
            background-color: var(--primary);
            color: white;
            padding: 10px 20px;
            border-radius: 5px;
            transition: background-color 0.3s;
        }
        
        .cta-button:hover {
            background-color: var(--dark);
            color: white;
        }
        
        .whatsapp-button {
            background-color: #25D366;
            color: white;
            padding: 15px 25px;
            border-radius: 5px;
            display: inline-flex;
            align-items: center;
            font-weight: 600;
            text-decoration: none;
            transition: all 0.3s;
        }
        
        .whatsapp-button i {
            margin-right: 10px;
            font-size: 20px;
        }
        
        .whatsapp-button:hover {
            background-color: #128C7E;
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        
        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)), url('https://images.unsplash.com/photo-1585320806297-9794b3e4eeae');
            background-size: cover;
            background-position: center;
            height: 100vh;
            display: flex;
            align-items: center;
            text-align: center;
            color: white;
            padding-top: 80px;
        }
        
        .hero-content {
            max-width: 800px;
            margin: 0 auto;
        }
        
        .hero h1 {
            font-size: 48px;
            margin-bottom: 20px;
        }
        
        .hero p {
            font-size: 20px;
            margin-bottom: 30px;
        }
        
        /* Services */
        .services {
            padding: 80px 0;
            background-color: var(--light);
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 50px;
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
        
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .service-card {
            background-color: var(--white);
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }
        
        .service-card:hover {
            transform: translateY(-10px);
        }
        
        .service-img {
            height: 200px;
            overflow: hidden;
        }
        
        .service-img img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s;
        }
        
        .service-card:hover .service-img img {
            transform: scale(1.1);
        }
        
        .service-content {
            padding: 20px;
        }
        
        .service-content h3 {
            font-size: 22px;
            margin-bottom: 10px;
            color: var(--dark);
        }
        
        .service-content p {
            color: #666;
            margin-bottom: 15px;
        }
        
        /* About */
        .about {
            padding: 80px 0;
            display: flex;
            align-items: center;
        }
        
        .about-img {
            flex: 1;
            padding-right: 50px;
        }
        
        .about-img img {
            width: 100%;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        
        .about-content {
            flex: 1;
        }
        
        .about-content h2 {
            font-size: 36px;
            color: var(--dark);
            margin-bottom: 20px;
        }
        
        .about-content p {
            margin-bottom: 15px;
            color: #666;
        }
        
        /* Portfolio */
        .portfolio {
            padding: 80px 0;
            background-color: var(--light);
        }
        
        .portfolio-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
        }
        
        .portfolio-item {
            position: relative;
            overflow: hidden;
            border-radius: 10px;
            height: 250px;
        }
        
        .portfolio-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s;
        }
        
        .portfolio-item:hover img {
            transform: scale(1.1);
        }
        
        .portfolio-overlay {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            background: linear-gradient(transparent, rgba(0,0,0,0.8));
            color: white;
            padding: 20px;
            transform: translateY(100%);
            transition: transform 0.3s;
        }
        
        .portfolio-item:hover .portfolio-overlay {
            transform: translateY(0);
        }
        
        /* Testimonials */
        .testimonials {
            padding: 80px 0;
        }
        
        .testimonial-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .testimonial-card {
            background-color: var(--white);
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
        }
        
        .testimonial-card p {
            font-style: italic;
            margin-bottom: 20px;
            color: #666;
        }
        
        .testimonial-author {
            display: flex;
            align-items: center;
        }
        
        .testimonial-author img {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            object-fit: cover;
            margin-right: 15px;
        }
        
        .author-info h4 {
            color: var(--dark);
            margin-bottom: 5px;
        }
        
        .author-info p {
            font-style: normal;
            font-size: 14px;
            color: #999;
        }
        
        /* Contact */
        .contact {
            padding: 80px 0;
            background-color: var(--light);
        }
        
        .contact-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 50px;
        }
        
        .contact-info h3 {
            font-size: 24px;
            color: var(--dark);
            margin-bottom: 20px;
        }
        
        .contact-info p {
            margin-bottom: 15px;
            color: #666;
        }
        
        .contact-info i {
            color: var(--primary);
            margin-right: 10px;
        }
        
        .whatsapp-cta {
            text-align: center;
            margin-top: 40px;
        }
        
        .whatsapp-cta h3 {
            font-size: 24px;
            margin-bottom: 20px;
            color: var(--dark);
        }
        
        .whatsapp-cta p {
            margin-bottom: 30px;
            color: #666;
        }
        
        /* Footer */
        footer {
            background-color: var(--dark);
            color: white;
            padding: 50px 0 20px;
        }
        
        .footer-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 30px;
            margin-bottom: 30px;
        }
        
        .footer-col h3 {
            font-size: 20px;
            margin-bottom: 20px;
            position: relative;
            padding-bottom: 10px;
        }
        
        .footer-col h3::after {
            content: '';
            position: absolute;
            left: 0;
            bottom: 0;
            width: 50px;
            height: 2px;
            background-color: var(--secondary);
        }
        
        .footer-col p {
            margin-bottom: 15px;
            color: #ddd;
        }
        
        .footer-links {
            list-style: none;
        }
        
        .footer-links li {
            margin-bottom: 10px;
        }
        
        .footer-links a {
            color: #ddd;
            text-decoration: none;
            transition: color 0.3s;
        }
        
        .footer-links a:hover {
            color: var(--secondary);
        }
        
        .social-links {
            display: flex;
            gap: 15px;
        }
        
        .social-links a {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            background-color: rgba(255,255,255,0.1);
            border-radius: 50%;
            color: white;
            transition: all 0.3s;
        }
        
        .social-links a:hover {
            background-color: var(--secondary);
            transform: translateY(-5px);
        }
        
        .copyright {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid rgba(255,255,255,0.1);
            color: #ddd;
            font-size: 14px;
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }
            
            .hero h1 {
                font-size: 36px;
            }
            
            .hero p {
                font-size: 18px;
            }
            
            .about {
                flex-direction: column;
            }
            
            .about-img {
                padding-right: 0;
                margin-bottom: 30px;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container">
            <nav>
                <a href="#" class="logo">SANG SURYA <span>LANDSCAPE</span></a>
                <ul class="nav-links">
                    <li><a href="#home">Beranda</a></li>
                    <li><a href="#services">Layanan</a></li>
                    <li><a href="#about">Tentang Kami</a></li>
                    <li><a href="#portfolio">Portfolio</a></li>
                    <li><a href="#contact">Kontak</a></li>
                    <li><a href="https://wa.me/6285334398018" class="cta-button">Konsultasi Gratis</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="container">
            <div class="hero-content">
                <h1>Transformasi Ruang Terbuka Anda Menjadi Taman Impian</h1>
                <p>Kami menyediakan jasa desain dan pembuatan taman profesional untuk hunian dan komersial dengan kualitas terbaik.</p>
                <a href="https://wa.me/6285334398018" class="whatsapp-button">
                    <i class="fab fa-whatsapp"></i> Hubungi via WhatsApp
                </a>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section class="services" id="services">
        <div class="container">
            <div class="section-title">
                <h2>Layanan Kami</h2>
                <p>Kami menawarkan berbagai layanan profesional untuk mewujudkan taman impian Anda</p>
            </div>
            <div class="services-grid">
                <div class="service-card">
                    <div class="service-img">
                        <img src="https://images.unsplash.com/photo-1585320806297-9794b3e4eeae" alt="Desain Taman">
                    </div>
                    <div class="service-content">
                        <h3>Desain Taman</h3>
                        <p>Konsultasi dan desain taman profesional sesuai dengan kebutuhan dan karakteristik lahan Anda.</p>
                        <a href="https://wa.me/6285334398018?text=Saya%20tertarik%20dengan%20layanan%20Desain%20Taman" class="cta-button">Konsultasi Sekarang</a>
                    </div>
                </div>
                <div class="service-card">
                    <div class="service-img">
                        <img src="https://images.unsplash.com/photo-1600566752227-8f3b1a105971" alt="Pembuatan Taman">
                    </div>
                    <div class="service-content">
                        <h3>Pembuatan Taman</h3>
                        <p>Eksekusi pembuatan taman dengan material berkualitas dan tanaman pilihan terbaik.</p>
                        <a href="https://wa.me/6285334398018?text=Saya%20tertarik%20dengan%20layanan%20Pembuatan%20Taman" class="cta-button">Konsultasi Sekarang</a>
                    </div>
                </div>
                <div class="service-card">
                    <div class="service-img">
                        <img src="https://images.unsplash.com/photo-1600566753190-17f0baa2a6c3" alt="Perawatan Taman">
                    </div>
                    <div class="service-content">
                        <h3>Perawatan Taman</h3>
                        <p>Layanan perawatan rutin untuk menjaga keindahan dan kesehatan tanaman di taman Anda.</p>
                        <a href="https://wa.me/6285334398018?text=Saya%20tertarik%20dengan%20layanan%20Perawatan%20Taman" class="cta-button">Konsultasi Sekarang</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section class="about" id="about">
        <div class="container">
            <div class="about-img">
                <img src="https://images.unsplash.com/photo-1600566752355-35792bedcfea" alt="Tentang Kami">
            </div>
            <div class="about-content">
                <h2>Tentang SANG SURYA LANDSCAPE</h2>
                <p>SANG SURYA LANDSCAPE adalah perusahaan jasa pertamanan profesional yang berkomitmen untuk menciptakan ruang hijau yang indah dan fungsional.</p>
                <p>Dengan tim ahli yang berpengalaman dan kami berkomitmen pada pelayan dan kualitas, selain dalam hal pertamanan sang surya landscape aktif dalam program pengembangan masyarkat dan berkontribusi langsung di organisasi muhammadiyah.</p>
                <p>Kami menggunakan tanaman berkualitas tinggi dan material terbaik untuk memastikan taman Anda tetap indah dalam jangka panjang.</p>
                <p>SANG SURYA LANDSCAPE merupakan bagian dari PT SANG SURYA MULTI CORPORATION.</p>
                <a href="https://wa.me/6285334398018" class="cta-button">Hubungi Kami</a>
            </div>
        </div>
    </section>

    <!-- Portfolio Section -->
    <section class="portfolio" id="portfolio">
        <div class="container">
            <div class="section-title">
                <h2>Portfolio Kami</h2>
                <p>Beberapa contoh hasil kerja kami yang telah memuaskan banyak klien</p>
            </div>
            <div class="portfolio-grid">
                <div class="portfolio-item">
                    <img src="https://images.unsplash.com/photo-1585320806297-9794b3e4eeae" alt="Taman Modern">
                    <div class="portfolio-overlay">
                        <h3>Taman Modern</h3>
                        <p>DI ISI SESUAI KEBUTUHAN</p>
                    </div>
                </div>
                <div class="portfolio-item">
                    <img src="https://images.unsplash.com/photo-1600566752227-8f3b1a105971" alt="Taman Minimalis">
                    <div class="portfolio-overlay">
                        <h3>Taman Minimalis</h3>
                        <p>DI ISI SESUAI KEBUTUHAN</p>
                    </div>
                </div>
                <div class="portfolio-item">
                    <img src="https://images.unsplash.com/photo-1600566752355-35792bedcfea" alt="Taman Tropis">
                    <div class="portfolio-overlay">
                        <h3>Taman Tropis</h3>
                        <p>DI ISI SESUAI KEBUTUHAN</p>
                    </div>
                </div>
                <div class="portfolio-item">
                    <img src="https://images.unsplash.com/photo-1600566753190-17f0baa2a6c3" alt="Taman Vertikal">
                    <div class="portfolio-overlay">
                        <h3>Taman Vertikal</h3>
                        <p>Kantor Pusat, Sudirman</p>
                    </div>
                </div>
                <div class="portfolio-item">
                    <img src="https://images.unsplash.com/photo-1600585154340-be6161a56e0c" alt="Kolam Hias">
                    <div class="portfolio-overlay">
                        <h3>Kolam Hias</h3>
                        <p>DI ISI SESUAI KEBUTUHAN</p>
                    </div>
                </div>
                <div class="portfolio-item">
                    <img src="https://images.unsplash.com/photo-1600607687920-4e2a09cf159d" alt="Rooftop Garden">
                    <div class="portfolio-overlay">
                        <h3>Rooftop Garden</h3>
                        <p>DI ISI SESUAI KEBUTUHAN</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials Section -->
    <section class="testimonials">
        <div class="container">
            <div class="section-title">
                <h2>Apa Kata Klien Kami</h2>
                <p>Testimonial dari klien yang telah menggunakan jasa kami</p>
            </div>
            <div class="testimonial-grid">
                <div class="testimonial-card">
                    <p>"Sangat puas dengan hasil kerja SANG SURYA LANDSCAPE. Taman rumah saya sekarang menjadi tempat favorit keluarga untuk bersantai."</p>
                    <div class="testimonial-author">
                        <img src="data:image/jpeg;base64,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" alt="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAKgAAAEsCAMAAABgwwj8AAABlVBMVEX/1gAAAAD/1gP/2AD/VWL/2gD+LQYAAAT/1QT91wMAAAj4307/3AQAAAn/2ggAAAyqkAf///+3mguvlQz/4Aq1nQq9nwnvzxgAABD/4hHNtRP6LwT/3xOymQsAABT31RfHrxvjyB3evxSGeRX52RNiVxL/6BP/V2FuYRX/VGZMRw/wzhqZhhJcURriwQ3LsAbWwRo5MBeyohF1ZxOumRseHg9gWCAUEw8zKApgURlKQBV/dB7x1x0/OREnJhCjkBQ6NxeGexMgGA5FQgsoJwgRFwxXUg2ilxk2NAlhXQ1xYx6aixQrKxUoHgqVgRWSfSHItiAcEBchJQkAACFSSR+KiYrp7extbnVERk5yZwEnJydbXVvHzNN6d3i+vr55cSWcbB+lHxe3DRyMTh4wBwZEAAjhLBfKGg9mSRq2IxNeCwVxAA44PRafXhSlGBSEDQ9JHB6YPETAR1G5Rk5eJCvgU19aMhOMMhuIZxVPFA+DggmcM0zdJhtsFzd4RzZDAx51LhR8UR0sFg+EMT1cGzBTEDY3ACVhwGCDAAAZF0lEQVR4nO1dj3vayJnWzGSiGXUQTVdUlqKsJBAOAdshgOMsYINjx46XDXHvtu1t27t0r+1uc213b7eb9rp7ba/Xu/u77xuBQRCwMYxt9nl4n/zEQrx8M/P9npH2HYa59m3AiqhqfIexbw1RfNMcZsKKqGqsiKrGiqhqrIiqxoqoaqyIqsaKqGqsiKrGiqhqrIiqxoqoaqyIqsaKqGqsiKrGiqhqrIiqxoqoaqyIqsZ3mPZtIfrt4LkiqhzspgmssMIKK6ywwgorrLDCCiussMIKK6ywwgo3Aswx5pQvfyYTM5NG72foTfO4ENwU5Ud6Rtw0j/NBsMZFxkCosuQSxVwzuymk60tOFGPmVHXdQMtOVOPOpo5AoEtNlDNOok0gKakGS02URHkdAc1lJ8p5FXhKorr+cImJMpFL93iCVMvkpulMhiz7ipoc9pgoQvZNM5oCxplwU2csAdGSlgO5yfxtQz8jquvOkhLF2vpjZAwFurO+pHOUwwSVel7Xn7xXB8J1a0klqtnSwCO9ETqW02ygqrWk/qiXl/LczVqEMUxd1BHLuSWWBnJ+FnyTMVD75KGeIctIFLNoFzymnNdbQJwEhruMa4lgcYwM1PG0uOUDy4VlkyVcTJw09xDqWBpEdZokauV0gZdwMXHRkuMOXl68qZxxK180+RJKFPt7KO8Nx5qYz3NiGecoraE9mwzOEuCklLpH2RIyFW1wk8nwLAHiopDgJSOKTUbdVEEkFjmnGzv+8jX7gTIqpMMR8Yn8yRJmHxiP0L6X7JnDtt5aQqIYllIT84RIYYouYRzCmVMvWMzsSxQky2jjA39BotwkHDNugt8gU4MqvjbBdrrMuZl4xX9a9Ra9LQZ6fTsHfJUsTFGBqAMP1jxmIkABXfDWRCOCCiG4GUWRor5mK98VfGjYgWh1Z44IFMe/CKhfQi3P3irf6+aqJ0fFg4Mi2BIVRKNUcuUAY1ufw7uHoWaMSZK+m6ketLffHQS0B1yJI0bdHS/hIhNOO8bp5Z1msL+cCq/cKuoHuUrY9EthXeaw4FdHKHFvaKtqJv/PnNRhNMcRQkR4QUNPb9ZsTiFMINiqxTEYktZ4YZZMY1b+u8l4k5sVfcOakSgBvQPeICfA0m0g/SgTUUo0oAkrngYoFijMo8XrFuAhRYflkW/svdDtWdNjnMvfjPKwa6QPKk1r+COs0Xsy/EZj1nleEBLuNJN+EgQhVYtc4t6YRkHeOOyE6xSsxeArMyY24ixBbmGV3AN1D2AZDP5L/Ee6FMGsY0VEqdZOFQJTgF7nmA/uZDJRkDxf+Eqyl1iuJTGYQhx7LfS+NXIJm7ZkGcdE2J1n+n5o0bjBHg8vhmkZPZWJrEAo0aEYWx/tDzMNJrGfpsKh7o8xbSXAcvE33n3Wak50tExahrgW5Sw1oRcQPaoNzSUXDT0nRm89TSCMRsfpdM0XZGK4appyihY9RWeQYY0/d4dEqWuA9ZRGEOy0ZTmOs75ugcWWOmcMxKps652mXEB8AhWieW2EPmhSMumnlweEcWuwdiQN8MpkuiRjAUk7aO2ftOUc03f2Dk72Ww+bnmlqEFVhLj0MmJzZD9H7kwcdpIlBwZ4ifTtUVgYAokbYlyhh1oZRjdzOUVo3dordjJv1LcuLth5mGoepZ9WaHXnAEda2oP4+enJqTRtVAt/Z+wDthVRZaoCTMF3qTTIQQjmlP34BgihUsp4jxxt8IcYpiNgJM8U1vd4NIwFesBlsp19GdLrzhqnXQG2QgLI8G5BbK/XdWubtwTrdqZ7aFo01PmaycE/kaHNCva3uMx0Va03Lb6A9F+win6gPpNCJ99IolihXl2zBJNj2eZwaw1ZVN+q1pjfNLIHS3IdJe5jb1fNNMc1pl7EH8avpRnQZ83YxUVpp+zA7QVWLWmoziKi0/5M/AYIAEW7qoBz3hdT2U+4IUU25vVbxMFaZu4II9LkvOTB6+igQlIGLS6ZwwCBEYrVQqiK4nLuT78iI1zV2w9iiKiTKRet5BE4ZJnZGSJUnLdH0q2Wez30IJLQJYZDUp+CKZLdRx4PlrjYjxMVGPZLqUYvMWW4MMp12nVxzptXMpfOhpX6XKjdbz325MJj0+C6mOtVDkUSJ4N/7wW9PHfji51w3HzhtPfeCLISOMJzEvPgN2rQ8NMGiWWk/z3hEOjLqJUozT/brkfyged4ulSyXZ7RCKBJ+vVMPONUkUfX7fjl3keHOb+lg/YDaNL1S7SBdKJvmlR3XykxwlMXcsRcIz6SOXSumH7VsEyyRmtzNBBD2CLli3iQ4EdRxO0/0tW4oTCJd7CsrUOBT9F5ELj/1gZPAXrl2ktJ3O1nn6gsTogt2Zo6pz4jfyr9I6WizCSyvIYkuis9sPM24nwPOCAQAYSudd87TrergpU8sbZ40K0wXzqi1sSvYZG9PLUgT1RaJFoj7D9G15NDpQ32hIjIJU/b1EM2ktxYZN2Knt66FqGilExK5aFWABZfdEdJGnr1kG2pSYBdBbOiDJDh4PxfYP1k8oIKCNhoSRdnrIZrbsc/EyNjFEjWjcq2WjczBN7KvpyBFxEdnZQVCLUucrwAw89w6SqN//NA98weJja6lo4OIk2c2kclCUapVC7mywOe1PdBTGdn98Ec/+rFLeRyxANG4eVPWlLQIc/CelMaeQ6KPt32Ig7gInuoIvftPH0XnhI7E3oOLfnLnzp0foWiUqImxiI4qlgBHTFGyafSjrYO9SKa23bSuo5/eufOzwjl+GqiIAdEa7WVXbJQBV5m7keXn0U4l/1JgTWmYPCTqwyJ2DN0w0M+Awo8r06vKViFuKf7hnTv/LLPnWp8o0UxzLZXLo8ae8XgvWneuYuxFfS+CCRbEdat/AaI/PZmecffOmooB71mx3EgWVSjXvJ1XR/rheqZkpw0j7XP1Qag4OBSy0hR//k9+dueH6Pn0srL30VnPpoFyIiZKy6gCc1Kkg/VSvmHRUudhoK9TrDDp1Cf6+NDjQHTQi3keURr0JCrpumbshEqilHiNdIhNKwfBrKCufpqxudKeKbiZKD5xuKwmo17tStePzuaoLMBSkixismiz1/2s64+d3uDSEFa91zACAV6fKIHpIg+fpPWQKH14CES162t5kKgZ6X0ktjMwbpaDbJS4nohSPQXjnkYHZw4CDpHrvUS1XrEzfpGHay8VRyYc03K6JrNZtIJAlRvAdHPQ2GzSmq6ngmROgtGo8zyN2p2BD0pKevml3krWe6zqmq9Y6XNmNfQm8MRM1Ix49DebA8cEc7+Q7kbJlhiZ0MW+H0H4fvZaE30ICytZnA7huyulKXNNvlGwZALGNIW9UW9XA2tYwwPRWv6wfo01meljZpwJ6aUZZM3B1/WqpSWuErkT5U3cnNaMTJxmJyYmApyS5AogsJDI0E7BtxlbH1IHEVuH6G44PTi26sdvl3oWJWrldU9mZOLSjfw9QgUD12E9QSbzx97OvWbYNCoUD2cCwc7e8aIlm7dLWubeT8Jy6MsCu3TiyMiBYTBx/cawToSpPeYii/LPP/7XX+gdkejpAxdqZ97WLkx6boJf4mQ0myy2jF9+9vqzX2z4XKa6tb43QXlczKZWWEy9CDzKZGmOeOFmKUGUEa/28d3bt+/+KieGmUiYC1trC4S1DAZHHINVH43AWTb9yW3Ap79uasNkiZ/1HMtyfLeR1g09nQ8iS1hOqfNuN6mEuNh4Ld97+/VHCecAiGbT8+7Xkp0UEeHRM1TwRp82Jdx/A5GAWD750NEGk5HWnu2+d7S7bSC9t8FlL98o1MEcjcTF5vHr23dvy/dWk10PmATg9823mGDube0E6/toH204I2k74n5+u4fPjsVgqTARPu1vFknp/b1Nkm/KS4wGCX/Tf+vdnyckCkQzYFNnSVy/DRj1mp7+rV5bb+kVz4wLh3E3GqfuZ/0Pu/uDaKCIsEmcvJ7YM9JHaqCe4K1O/pM+0du/S/QKcSwa8/fkYKuRP0V5h1mtdKr9USfwI4+C7sGkTxRG//NgeHdw+ONdTejfv/jyzZsvf//FVz+QRLcHehzUPgj07iSimpVH0ZxEsVdGtS0jlAuq0jh6DuO52whsU3Az+3GPKKynr4fDJUUNRL/68sGDW/fv37oFf3z5FUJF6+wSxsX+QKC3f5cYenD2dw1zzqyzXTCO7K28AElhKhxRKtcKT1GqEPhW+PHZp909GvS4YXDVfAN98eBWjPiv+w/efNUYLBoY+T/cHkg0OUfBSdl+xOcJ7mCEbWPfI9HQCwJzI2w3t5ve65T/OCC6ObInyCx+cf/WKL48HsxRjKPPBwL95D9GJJrVq+YcREE6zHmxC15u0v5hDlx5uNFO/2nwee9ZI4rr6y8fjBH9JhgQZSR8PSTaSBgibAaoO2sXWhLSgVtvGCFhI6EBBgsAC9QrF//zTKLveUlbQN1vxon+uTlYI7CWhkQ/Tpp2JrroHp0nDGFm94XRhlhmLCksqRJOm3/sT7W7JyNDz5t/GaX54MFfHTycxc3X/Tl69/Yv3aQhsgqgneaosTBNdFBtfdpQmOT0097HffL1SK0Jey/fJGnef/AgP+xfArfpv2737NLt16mR/Ki/q/vzlJXBrfGKqWkZTM4jsdHTM59VzBGZk9NvkkRv3XrTGbqjMMe/7s+ZT/V2M/k2Wz/i81QXwXm39vVpoYG0TtHfYqa/2hohCl9hdOzvJ9aSNJTNP8m33X39SM8nAzkaQFzC5mi/hWlVRo/K2YhMqlHK6IKG//3xp5/+JueNmBOOvf03MOCJtZSwN/D1afi3Tz/9/A9fF41asvUO1tJ8O7MhhCnsPNVRbureJA4x/eNyCOFacn6AFS3//dZAlcI/fi3G1kgUhuWok9r1R/Rvfs7aA+PEh6ixgYJpOxIZ914aoeBjHXSYWUdvHgyJvtkQ4+/DxDo2dptJfQIWrThf4gHsu4kpi7a3S9MWFNaigzoM/EjoxsADPv1mMPQPbn0zngDn3LQq+pE3khIhWWN/oVCZPkR5YbJo8nIkpZS0JuPlN6f9YED0wV/Gy16Mm0F6f6TRFHOzk1owUe69TLVgeCffhNHSTo3yce1HTv88WEpvcuO+MDZPjYqVtOqEE7N46C+Wc2JREbliSskT1KJfzIjxPDG2imdK//7fy+NERfA8K3jyPeCNN+X+wkV4gocZojV7mhGWB1Tk3PGmfnA9voo9PBBofqT9F8vtJQUfYv6k58mkv+0uuIUBPJBAr0fEnOoveMG4/cJcVL6Jzef9/3FHSmXwk8yGp43LjjnFtrcoUZNZHb3gTW7y1eJjP8YTuBDqexuw8h88+PPxqIvJzUpgvtVwxkjJaIkFM82yAOQUUMObehtZ5Bx9BTQW8Y7/9/ff/B/4AaNa1g2l2zj2nbHonnWizg+5K0bzNtM5C25vTmDL3vbN5GYaQu1aBSajNipRTjjBYx4uId7a+9a59bTZAGu7WQSZ0ks+8lpcUHfs351ptGaUVXQ0w9iSZl0vgDRmn0ZE7k+Z2uSWBGfmo7ajJHHPZKNsXq/b4xmXc2yJSbTZKkbAs2LMm8t5Gxh7DbRXNsGUD/JvnE1zAy4DkMHuYaSuCQb0aQ2tVbxEopCHDxUQlVtLa3M3pL0F2Zhouc/kkhoQNV+p6F5hze12xJQ1asm2Y2Y28+hgsLOK1roqahgihyqCKTnTRh6VAYpJNt56LcOQ9Q/wKYmd8he9u8wBlVFdWakOXOOz0oEI66mcKTvEnXZt4dNIMGeimDpVVVwiZpAPROxJyG6FjfQuuGnWy7q3sC0BH+UYFSbZu3luptGygd7tbfQFEXAvW0/XvMCwF2+swMQ20qGaXmGYnKLd6aBDf3A74XdSeUPFsWPMyaOOmv1qGjNJsOZuffCoczaTYPVbLaRkt7+o6XVrnqzDBMBQ5yB6b5QfxWVtArYOw7hXzfnKAkkQEqYRON1q9qthLex2w60Np50VwvLs0PesABWjhRYSlhvGIBotopos26rZAkgrnZxfvmfljoPqjpEy9LVX6Hlzth0CU8HlvhLRRVVHmY1nVsEtREFAg3Tqg5dBNswG+0W5f2shMWBwHamLdpsKy95eu3kSZVyafRR4gkh4HjcXbFEhPif2th5ihU+HCrejvNfKgkMqdb50HmSbwIzO5jSI72e9TdBwCgVKym1x5LS2NGc3UrZJApNKZSNdU6RBe6CVvHB5lmsWrHRV+004qXyY7lhKm8Zot2oRmJOm2QjnKlpMAhYd1J2vN34qvGqc34RI9J6LtcW1fA/0FVpXdKszeEe9aj8ngYvVGBFNHhuCHEW3OoMoxolYsCUPgzl2sEyBUzdUE+UHcQoMNHQYnLOR95JwnuwoJkpYMY7gZGrGVuQ/APztR9bFV10GxO8RlXoe3DFFRMlWalNxcxvxjwbbAthbjVbzgrpGQ3UXnn/Sy35Kq2mqmqP0od5Rfdwvf9UjGrdoKSN6T02EkIRoxHMUNJOv7vA28ESVH0RvVXuLCdNgS1O1I9IqqN9+Iaq9s0ewpoyoLLAj5VuERLfcV/hBuGiavQ9M+HPkq7hTEjRo9bae0CBUZUJJaWcnuviySwGTbKzxMDYz5XlaPt4G3CWbqis/BJCUTqQYGaOZMlOi8ONjp5Tre4hCYxvKOW25ag7b41hsyBYnBbdKgomXMi3INZELph1FcTlwYlVBjSrfRS/cnBm3whQqak6UxcTMX8F2O878uinbK6yDe1RJGMqxfWio37uKmVV1ZVdF9KxGlbh5WAv1czbqzAvOzewrgeXB3HlHjR4lp+i8bW9zAjPT+tDmmlNN6TVrQmn48nc0W0b3ra4JFaDhdjNqpTY6qcDC09pLZoesAQb0KojKxHA6nfOck9SpUFC6ig6u6lxiE1RUxsPMq+qVxTdGYd9o+wqq85PAiSy9M+x1Uy1hLnh2EC+jgjX9BDgF4Cbzgp2GPIlokU+hLUMWLq5w3zIzuUbtwmFoLaRczMZVbwOPT2AkTpDa8BaZqebTqe1+akG97rNaRGVXEBvrbZkFxEabqvNOk4EFtaupapbHFvXSsqEZvXM9R2dzebxYtpA+qPgznZw1CiIai53GMTtkHoJTL5tHH9R8cTk9w7jppPeu53ySMxDL3USHFU+ehTYzV8xxiF6pOUl4ZnDiuXWjGFqXOOUOtMaxvvDR2ZdEvBvj2FirebNn9jlxDnRfWZp1Nsjdi7JzXK+ahM1oAsC718Gtvf7nuHBmnabRpk/ZbFKVTU4VoXRj+mzgcjOmrh80ZywWMmcTeWq3+s8G2WlkVZ91CtGMx2GH6YZQlma9HLDpt/ft2gwnEWryGBBdHqt7M0Q5La+5M3aCRbttRYddXx4MM9E1Zgh/5flEbmqhU7cWgjwl2HuRm6FsxDSvurbgtoAFQV09lO0s518F5jOlpO9wfnCrULQuMvkg0Ea6dLMP7WLgDZ9eVM0nRAr0BpR9AmCguh965wsLE7Oq2+Ka7fw4mOmngvEjKZLAXG5rvvGn4pigojrb5xQ6IC5kTnv3ej3mCSAEa35q/xxdHu84ca/ZEZ0AeYh4JeVOy/QScJvKxr51LWdOXgQmcs/8yY4RGHfqv9h1tKV4ZDjW+EHem5SUlOzMfNqeuMP0+sFkt93LSc/fxIx4DTlBl0KgUlFSebzQyNMN5NG38jnHVSMQCpLVqoDNMJ3xBmUzOV9NjInjPk+dXkkufF5gLKRMExJlQDOsptuhUPRECzWQJ8qWXnTOUn2MCifK5NOoG1G1B8ergGjUG3avS0bUGntIT1WlOG+a1lsgPgodt/e8UOdQ387XbKGuU04hiK+7xOw1BDvb6aYln2JiLqVEZVKx17rs6Tvr8cGC6o9BVAB+0NubAbrJ13cVN+CphDg562gioVG95gTjZSAa92Kiss8+pbyvTSFEt+fGy84RY96ju64DYqMXEcsmlGV8zuUAopWLiYI5raIbS9/MAHqvd7oT1qyDF84NJBhnBQ2qlizwgW+33Zj/iQ5XDxJUPXkuoWwXq5nLTNTNW1i2Q9MKCpcjSJoMUj6yeEkwYn20tvh+zCsEyR551ivKXW83d7XtAwuCZo+Ety9Kj0O5Xek6HnIxJ0i2KKKXVpDrPIuutM1hUQBRr7zhdI93wdAvXfyRAMkeiOBY5N/Xr+fREXODhHVR+X6kGzeeYrwAJDxwNu2Kvjtjiewq8VZzVfK/dOsoROtPUFlNa+Rc6D0CNGZFRoGH0MJ2+1XVqHhYPld3BP17KKc1/gJJ/AgnMXppM9XeWWt5cgfU6GXD/oO3sjuXIz/2/QkdYOwFIX9PhelGJdeJLxi9avB20b/j+P1HRD8drLS1lY3xcIDg+wl87wzvDHAP8M53x/DOd9/pv9a/pn/tO4MbJG4aBA/hVw+9T9/a2vLP9WW4bQPVrQTRIEgQzXwv08O9BN6ZBYnrz+6R6bOUfwzF4sYst2z7/O0Z8pH2UuzxQFCSGCgzRu8veKX/V//lGTC8lTh788jrveE340+HX/LcqvNGXz5JPN72Hv8pd63F5wvJh0LGMyN+FjbvP+hzsI56Uzu5ssa//sjK692B958o2hvJAeS5dixOVU481ej/AR7eWHoehL7TAAAAAElFTkSuQmCC">
                        <div class="author-info">
                            <h4>Ibu PIKACHU</h4>
                            <p>DI ISI SESUAI KEBUTUHAN</p>
                        </div>
                    </div>
                </div>
                <div class="testimonial-card">
                    <p>"Tim profesional dan detail oriented. Hasil taman kantor kami melebihi ekspektasi dan mendapat banyak pujian."</p>
                    <div class="testimonial-author">
                        <img src="data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/2wCEAAkGBw8PDw8PDw8PDQ0PDw0PDg4ODg8ODQ0NFREWFhUSFRUYHSggGBslHBUWITIhJik3Li4vFx8zODMsQygtLysBCgoKDg0OFxAQGDAfHx0tLS0tLSsrLS0tKy0tLS0tListLS0rLS0tLS0tLS0tLS0tKystLS0tLS0tLS0tLS0tLf/AABEIAKgBKwMBEQACEQEDEQH/xAAbAAEBAQADAQEAAAAAAAAAAAABAgADBAUGB//EAEQQAAICAQIDBAcEBwYEBwAAAAECAAMRBBIFITETQVFhBiIycYGRoRRCUmIjM3KCkrHRBxUkQ3PBoqPS8DREU4OkwuH/xAAaAQEBAAMBAQAAAAAAAAAAAAAAAQIDBAUG/8QAMxEBAAICAAUBBgUDBQEBAAAAAAECAxEEEiExQVEFExQyYXEigZGhsSNC0TNSYsHh8BX/2gAMAwEAAhEDEQA/APrwJ8U96VSIRARIGEYSKqEIkCJAwHEgYGkDCNiQOIVoE78tsUNZZy/R1qXcA9CQPZHmcDznRh4TLm+SrXfLWneXbTherYZFNaeV1+1vkiuPrPSp7Fv/AHWiHPPGV8QH4Zq1GTSr+VNwc/8AMCRf2Nkj5bRJHGV8w6vaDdsYMlnM9nYrVuQOpAPUeY5Tzc3C5cXz1dFMlb9pVic7YMSoIGhWlBKCASggEokyq0IDKogECTKogXCNIGEUJBpFhQgMIZAyBAkHW4prPs9Ft/Ztb2Vb2dmmN7hRkgfCbMOP3mSKb1tje3LWZfJaL+03ROcW16ij821bU/4Tu+k9LJ7Gyx8sxLmji6z3h9RwzjWl1Qzp767e7aGw4OM4KnBB+E4MvC5cU6vVvrkrbtL0cTnbDIJdwoLMQqjqScATKtZtOqxuUmYiNy7ug4VZf6z7qKe4YK6i0fH9Wv8Axfs45+/wfsqI1bN1+jhzcV4o+h0ukrqXZWi1rzOFGMk9SfEnvJ5me3FYrGocczMp12vqoXfc61qTgZ5s7fhVRzY+Q5xMxHWUiNq0erruQWVOtiHI3KcgEdQfAjwPMRExMbgOr0tdy7LEWxeuGGcHuI8CPEcxJMRaNSsTrs+c4hwqyj1k3XUc89XvpHn32L5+0O/dzI8TjfZUTu+H9P8ADsw8V4v+rpowYBlIZSAQwIIIPeDPAtWazqXdExMbgkSKJUEK0oMQAiUEoDAkiVRKMYRMqiAGUTCrhDIhEgYCBIqhCESBEgZAwNJtJfj3p96JnRWHUUL/AIKxug/8tYT7B/KT0Pw8M/U+z+OjNXkt80fu87Phms7js7X9k3EFXVW6SwBq9XXlVfBQ3VZYDB8VL/wiYe18dpxRkr3r/Bw1vxany/V20W39U5r/ACNm2r+EnI9ykCfNxn388b/l3csx2cT6kp+tQqSQFKZsSxicKqnAIYkgAEDJIAzNlMHvZ1ine/Hkm+o/E+i4TwbaVtvAa7qida9P7vF/ze/GATn6ng+Cpw9fW3mXm5c03n6PZna0vP49xH7Lp7LsAlTWo3EhAzuqBmI57QWycc8AzG1tRtYjc6fn9vExZYWNpsvYEGywGu0r1KVof1acug5nGSSczxc98l+s9nbStaw4aeI9hYXqt7O4Y37AbNwH3bEGdw9/MZOCOsuDJlp27F6Vt3fo/A9f9p09dxAUuGBCnK7lYqSPLK5ns1ncRLimNTp35kjwuL8H9q7Tr+k5tZSMBb+8le5bPPo3Q9zL5/G8DTPG46W9W/Dnmk68PGWxSu/PqEbtx9UBfE56fGfKzjtFuSY6vUi0TG3Guo3fq0e0fiUBa/fvbAYfs5mfuuX551/P6MZvHjq+K9OPTLU6G5dPVXp+0NS2MzGy0JuZgB93J9XPxnq8D7PxZ6c8zOv0c2bPas6fE3emPFL2CjU2ZchVroSuslicBV2ruJz5z1a8Dw2ON8vb1c/v8k+X6t6J8P1Gn0yrqrrL9S5NlhssNnZZAxWpJ6ADn5kz53jctMmT+nGoh34a2iv4p6vYnI2gwCUTKAwolQGVQYBAmVVSIRAqRGkVQgkiRCIkVIESDSBAhE3Uo6Mjqr1upV0YBlZSMEEHqJaXtSeas6kmNvy30k9D7+HXJrtAGtppsW3s+bW6cqc4Pe9fcT1APPxn0XDcfTiaTiy9Jnp93BkwzSear9U4XxCvVUVaio5ruRXXyBHMHzByD7p83nxTiyTSfDtpaLREw7BYLZQzewuoq3Du9YlF+Tsp+E7vZMxHE139WniY3jfWz695jyeOekui0I/xOoStiMioZe5h4itcsR54xA/P+P8A9pFGsA0lWnsFVt2nV7r3SvCi5GyEXOQcY5kdZrzb5J0yp80OjuZS1bs7MtlNilihHZNfgAY9YkKMHPz5zx+/WHb26SKiX2VqWAbtLbNrIF7NrC2D97J3csY7+fKJ6TMz+R36PQ4B/aTRpFOlu09prqu1CrdS6WZU3OQSh24HPuJnsYt8ld+jiv8ANL9A4H6R6PXDOmvS1gMtXzS5B4tW2GA88TYxerA+Io01bs9hG8NfqHqDHciqbnKsi9BkHdnr63WfIe0s0/EXinR6eCv4I27mfH4kzzYiZnTf2fgPHL7eKcSvbTo1zW2EUKvP9AgCK2eirgAknl60+1wVrw3D1i061HV5dt5L9H6R6GehdehAuuK3awj2hzroB6rXnqe4t8sd/h8d7RnNPJTpX+XbhwcnWe76yeW6QZRMoJQGAGVUyjGETiVRA0o0gqAyIRIqhCESBkCJAyBEIZFVARJtHVp0nY5+zhUVmZ2pPq1M7c2ZcD1CTzOAQefLJJm+ckZOmX9fP/rDk18rnW+uzNTgqzqwNVnJmXHPaRyYYPVTy8ph7u+OYvXrrzBuJ6S6fpd6SarS8OsCMy6gNVWmqC7t9TNgk9yWAYHPkc5XvC/V8Dx1OIrET0t6PNy4ZpP0fjqJZYWf17GZsvY7Z3P4tYx6+8zvm1Y7tURMud9DtA7WyuoNnAxbaT4/q1Kn+KYTkme1ZXl9Zejw/ia07VOoN9SkFarNIWCkdNjM4K93cQPCcuTBN+sV19pba3iPO213E1tBUan7PSf8qvSMgOfxMrkt3+APhGPBNJ3Ndz9ZLZIt508z7Kn3NRQfJu1pP/MQL9Z0+8nzWWvljxKRXbUVtG5Ch3LdU4IQ+ItrJCn4zKMlZ6MZrMP1f0O9J9XrtC1dpJtW1qX1QGwtpxWjZ5dbSWZcjoBuPPAPB7Q46vD11HzT2bsOHnnfh7Lsla5JWutQAMkKqjoBPkYrbJPTrL0txEPM4vXZq6bKK2fT12rssvK4s7I+0K0PMEjI3NjGcgGdWHlwXi9usx4/ywtE3jUDgnBNNoq+z09YrBxvc+tZYfFmPM/yHdGfisme27yypjrSNQ75nO2CVBKoMoIEygMokwrSoDKJMDQpEIRCmRCJFVCESSKkDIMJBrGCqWPRQWPuAzLEc0xEJvUIFr8s0WYPPKmpgPhuz9Jn7uvaLx+7Hn+g+21j2m7L/WVqc+7eBn4R7m/jr9upzw7KnIyOYPQjmDNUxMd2WzMVRbUrja6hlPcwBGe485lW81ndZ0kxE93z/pTorG02oqrd3Q6XUWtXYxswawCgRj6wJPiT7PLE9Lgsteet7RqdxG4aMsfhmPo/PeA6nYLCBnFQdQeZ2Keag93ImfW1iHlS9PjqCyhbF5hSrA+Knl/uPlM5R83MGTQNAwODuB2kfeBwwHvkmIV+jeg+juXS1rvNKOpvBXLO62WOARnkpwgPMHkRPmfaWTH72ba3ro9Hh98kQ+qq0qqQxy9gHKywl3GeuM+z7hgTy7ZrTGo6R9HRFIjq5cTUyEIDKqTKCEaVUyglAZRJhQJUBlVMI0KRCKEg0KoSIZBQkkIgMxDCJuTcjL4qw+YxMqTq0ST2c+kfdXW34kRvmoM15Y1e0fVK9ocswidK6zaCokkIEY9WqJqc+9kIJm2M+SPO/v1Y8kA6awexcfdai2KB5Fdp+ZMy97Sfmr+nRNT6g2WL7VW4fipcPgeJVtp+AzHJjt8tv1XmmO8J0li2W2kc1FdCEMrKQc2EgqwBHIjrMskTjpX7zLGJ5pl+Z8d4PTw7UAHWV0rYWFddlTPtqbIyxU52927+hM+m4Tjr5se4pvTiy4K1n5u7uaX0c1HY9murpalwSCKS4KsOqndjHfJPtWI6TRnHBb67cI9CH79X/wDHH/VMJ9q/8WXwX/Jj6Ev3asfHTj/qj/8AW/4/ufA/VxWehtqgsdVUFAJZmqKhQOpJzymUe1ImdcrGeCmP7k+jPo1RrrCF1iXVVNm1alK2MoPIjJ5KTyDY7uXdLxftC+Gm+TUz2YY+Hrafm2/TezCW1ooCqKGVVHIKqsgUDyAM+a5ptjtae/N/LuiNW19HYmhsaUBgBlRMKJUEqiUECTMgGBMoxlEmAQphFCBhMVUIRQkCJAiQVIMIRQjelTwv9RUPw1qh96jafqI4j/Uswp2dqaWTQNA0DrUH9Ld45rwO/Gwf1nReJ91T82EfNL8o9NLm0XHU1mpq7fTizT21I/Ku2pKwpQEjG5WDNjxwe+fUeyr0tw9Yr3ju8/iImLzt9jwvXvr3v1yaazS6S41jT1MFy+0HfeQvQsTjlyOzPPOZx+08uP3kVjvHd1cJExWdu9PN27GEbHS4lxL+7rKdbqdLbqtCi213VoqMarWKGq/a5AIG11yTy3j4+n7LyY+ea+fDi4zcxGuz4v0ItbVcdbU6Wn7Ppy+ptsqTGynTujBUOOWS+w48QcdJ1+1bUjhrRbvPb7ubh4nnh+orrKrNSESxLGSq4OFYMUIsrGDj/vlPm5xXpgmbRrcx/EvQj5ncM5mxoGlEmEEqpMqNKoMCZQGUSZRMKxlRJlBCmBUkowhVSIqQIkFCQaQIgVIJ4dyVl71uv+TWM4+jCZcR80T6xDCvl2poZNA0DQPiPSEZ1trey6diEdeTqBUrAq3Uc2ae3w06w1jx1/l6HBYaZMdotHn/AKfTcG1Y1NANgVnRilo2gr2i4O4DuyCrY7t08/iKThyfgnUT1cGTHyXmlvD0Zy/VEW17lYZKkggMApZTj2hkEZHmMTKttTHlJ7NUm1QMliAAWIUM3L2jgAZPkItO5nwR2UQDkHBBHMHvBmMTMdYOkvE9IrV09ArpVaTc+39Eor2pgl2G3HPGFz3bszv4SJy35rzvl9W3h8MXyRXx5eT6LDGqAHIfZrhgcgBvpnTxc7xTM+sO7j4iIrEPriJ5LzhAxlEwgMqgwJlGMomUBlEmUSYVjKiTKCFMCpJRhIqxCGQIkFCQMgwgVIOi2vTTvaH5b2WxSxCqR2aoRk9+U+s6PczlpWa+OjXHSZYcZDewaz7nDfyj4WY7s40G11viB7lH+8vuKwy1DiOrsP32+HL+UsYqx4NJNzn7zfxGZcsei6eTxfSsc3jJCJ+n59KweT/DJz5e7n1YLRP9P9P8N/D54w269pej6GscajHs5pPlvKtn6BPpOb2hHSn5nGzE5unpD376FfG7OQcqysyOp8mUgicNMk07OSaxLhOgrPt77R+Gyx3rPvTO0/ETZ8RaPl1H2hjyR5I0CD2N9XlU7In8Hsj5SfEWn5tT94OSPDlooVM7c5Y5ZmZndj5sTn4dBML5LX7+GURp4PpjUdtNv3KzYjnuUPtwx8BlAP3hO3gJ+avmXTwmStMsTbz0X6L6EohvcYa0AVg9Vp6gnwLHn7gvnHGZYn+nHjv9zic3vb7jtHZ7hnC0JgYyiYQGVQYEyjGUTKAyiTKJMKxlRJlBCmBUkowkVUIoSBkFCQaQIkFCBQjYh6Eb2kRv2lDfzmUZLx2mU5YcP92afupqU+KIqH5riZRxGWP7k5IQeE1dxsU+Iusb6MSPpMvir+dT+Ry/V5qjDWAO1iK21WcJuJXk59UAYzkdPu575127ROtTK029DTU5ZE7lC6iz35xSvzDN70E5rX5azaPPSP8AthbrbTnq0nYk9iqitmLPTgKA56sh7j+U8umCvfrtmjLGsneO0/5NTE9HcdgBk9B5EzniNs0DUIfvr/EJlyW9ANqax99f4gY5Leg5EYEAjoekxmPA6z0tYSLMCkHlWDk2477D4flHXvJ6TfXJXHH4fm9fT7f5Ycs2nr2GjG3fV3Vt6n+kw3LjyB3KP2Jcs82r+v8AMLT09HOZpZiBjKJhAZVBgTKjGVUygMokyiTCsZUSZQQpEIoSSMJFVCKEgRIKEg0khEChIKEgYGkkdbiOoNdZK8nbCV9+Hb72O/Ay2PBTN2CkXv17R1ljbs87R0rlE6IMDmfugdJ0ZbTqZZ9oerpedmoPeHrQfsClGH1dpzZelKfn/LVXvLtTnZuglb2Pcr2PsrcKi1k1FlNaPlmU7jzZl5ED1eYM65tXHSs1r1nzPVqiJmZ3Kjwmg/5fP8QexX/iBz9Zj8Vl9f2hnyQ6l3CSpDI9llYzup3KLD+zYRk9OhPPPtDGJvpxUWjVoiJ9fH5wxtFvEt2NjMnZJqKQHQtbfqnYGsMdwFZZskgDG4DG7uIwbz0iJ55i30iP+2Gpnt0exPPb3V/z386afo9uP5mbt/0o+8sY+ZzGa2YgYyiYQGVUmASjGUTKAyiTKJMLLGVEmUEKRCKEgwkVQhFCQIkFCQMgwhFSKRCKkUyDr6vSraAGLKVJZWQ4KsQRnnkHkT1Bm3FlnHvXlJjbo2cOtHsslo8G/Rvj3jIY/KdFc2O3eNfum7R9XDwvXhLnRwyqwRSTtK13KXG0kEjmFPTkOzxNnEYJtjiY8fwwi0TZ9ADnmOYnmTGmx1NV+jcXDJTbsuA5kVgkq4H5SWz5MT3ATfi1evu57+P8fm126TzO0jBgCCCDzBByCPfNNomJ1LPZmKtA0o87S377rmx6hSpamz+sRGsDEfvMefeMHvnXlpyYqx58/TbXSd2l3JzNrQAygMqCFTKglUGAGUSZQGUTBLGWBJlBCkQihINIsKEIYFCYyEQGQMiGRTAoSIYVpB0eOcSGl09l3IsoxWD0a1uSj3ZOT5Azfw2L3mSKpLp+i+n7bRBrl/8AEZYjJzsX1UYN1ySvaZ6gvmb+MyzTNEV/t/8Av/GuIjqLa9Rpz3219zowSw+TA4UnzyPdMq2xZevaf2Zxv7obiNh+7fnw9UfXdj6yxgrE94Xf0dbTNfW2agKqzz7J7Pvfl2ghR5ZI8AJuvGK8atO59WMRMdndXjTj20dT51NYPnXkTnnhKz8s/uy2TxxugVie7FFo+rDA+Jk+DjzP7m4cmnqv1JzaTVR3oCN9v5SV5KPHGc+IktbFh+Xrb+GMxMu/q1CNS4ACq3YnHICtwAAB+2tYmjHabRes+ev6JPSYc00tjSgMCTKAwJlRpVTKCWAGUBgTKAwAyghTCEQpkQiRVCEIkCJBQkGkQiRVQEGRFCFaB5PpRwtdTpmUsytXmyor/wCqFIUEd4OcfGdXB5Zx5O3Se7C06jcPX01C1VpWvJK0Stf2VAA/lOXJfnvNp8rWNQ5CJhE6V1bNBWegKn8p5fKbYzWhduE8M8H+a/8A7M/iPobYcLHe/wAlx/vHxH0NuxVoa17tx/Nz+nSa7ZrSjsTWOHW1F63VfaKnYfCwc1PwIBmzDblvEsbRuBVaHVXHsuqsPcRkS3ry2mPRlE7g5mKiEEqpMqCFYyiZQGUBlEmFEqAyqkwjQrCAwKkRhIqoRUgRIESBgMiEQpkDIioV19efUX/W0o+HbpNuD5p+0/wwv2d2czJoGgaBpRpBoCJSXQ4fyqrHcFCj3DkPoJ0Z/wDUljT5Yc5mpkJVEAlQSqDADLAmUEokwrSokyqIRoVoDCKBkGhVCQMiGAyChIGQbMIZFIgIMiODiFe+mwZVfVLBmOEVl9ZWJ8AQDNuCdZIS3Z52k17FVZGIUj2W57fFSD0I6TpyYYi0xMMo1MbdgcRs/L/DNXuaroHiFniB7lEe5qaT9tt/Gfkv9Jl7qnoaUuvtH3gfeoknDWTTkHEn8F+R/rMfcVNMeJv+FfrHuKmnT1vFHAxvCs3JR0UfnYjogzzPd8pvxcNWZ3rswtOoerRUEREHNUVVBPUgDAM48kza8zJEdFzFkCYBKghWMokygMoIEmVYEoDCAyghRAYGgUIDIjCFUJEIkFSSEQHMg0gRCHMikQPIOoGoKtgtRuPYovN9Qynm6LkAgHHrN6q8u85X0Yxxirrf4vM+n0/87ufn3P0cut0hrQuWCLj1ixX1D5k8jNOPJz21rbfzdOrpaerUuRtCFM87HrelcflBYlj8Mec33nDWOvf07sea3h3P7vt/HUP/AG2b/wCwmn3+L0ld2WOGv33L+7SR/NzMfiKf7f3PxeoPDX7rl/epJ/k4j4in+39zdvVP2C4feqb4On9Zl77F6Sc1nRsNyH9MqUqDzYbra2X/AFOQX94TfEY7R+Cdz+n7EXnfXo7dFRfmoLDAJ27ckeWSAfnNNrcvfoym3Q06haCoz/hndalbmOxtYgKjK3OskkDaeWSCMZxM74/eV3/dHX7x9PVorfU/SXqEzz28SoIGlVMoDAJQGUSYVpUEqpMDQJlUiEkyBEChIjQEGRVCEIkCJAwGQaQaEJ/nEdOo6mn0ArztttAIRcZrGK0GFQEKCFA6AHvJ6kmdF+Jm3eIa4xRHlzppUBDbdzjo7lrLB7mYkj5zXOa8xrf6M4pEOfM1MmgaBoBA2YNOudHXklV7Mk5JqZqix89hGfjNvvr61PX79WM1hxWaEM25rLTldjL+jw6ZztY7ckeHPIycYyZsjiZiNREMPdxvbtmc7YIVpQGUEAMomUBhRKAmEBlBCgykJhSIFSI0ChAZEaRVCCSIQyBkDAcyDQNIGEYQHMitmBswNmBswDMAlRoUyggTKNAJRMoCYBKrQiZVEAMCZVaBoFCAyIRCGRTCMJFUIQiQOYDINAcyBgaBpBoRoDA0AhWgaBjKDMDSiY0NKAygJgSYVpUBMqiEEKkyrAgEo//Z" alt="data:image/png;base64,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">
                        <div class="author-info">
                            <h4>Bapak PIKACHU</h4>
                            <p>DI ISI SESUAI KEBUTUHAN</p>
                        </div>
                    </div>
                </div>
                <div class="testimonial-card">
                    <p>"Layanan perawatan taman rutin sangat membantu. Tanaman selalu terlihat segar dan rapi tanpa saya perlu repot."</p>
                    <div class="testimonial-author">
                        <img src="data:image/jpeg;base64,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" alt="data:image/png;base64,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">
                        <div class="author-info">
                            <h4>Ibu PIKACHU</h4>
                            <p>DI ISI SESUAI KEBUTUHAN</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="contact" id="contact">
        <div class="container">
            <div class="section-title">
                <h2>Hubungi Kami</h2>
                <p>Konsultasikan kebutuhan taman Anda dengan tim ahli kami</p>
            </div>
            <div class="whatsapp-cta">
                <h3>Hubungi Kami via WhatsApp</h3>
                <p>Klik tombol di bawah ini untuk terhubung langsung dengan tim kami</p>
                <a href="https://wa.me/6285334398018" class="whatsapp-button">
                    <i class="fab fa-whatsapp"></i> Chat Sekarang
                </a>
            </div>
            <div class="contact-container">
                <div class="contact-info">
                    <h3>Informasi Kontak</h3>
                    <p><i class="fas fa-map-marker-alt"></i> UTARA PKU GEMPOL PADING RT 02 RW 01, PUCUK KABUPATEN LAMONGAN PROVINSI JAWA TIMUR</p>
                    <p><i class="fas fa-phone"></i> +62 853 3439 8018</p>
                    <p><i class="fas fa-envelope"></i> EMAIL NYA SANG SURYA APA? HEHE</p>
                    <p><i class="fas fa-clock"></i> Senin - Sabtu: 9:00 - 17:00</p>
                    <div class="social-links">
                        <a href="#"><i class="fab fa-facebook-f"></i></a>
                        <a href="#"><i class="fab fa-instagram"></i></a>
                        <a href="https://wa.me/6285334398018"><i class="fab fa-whatsapp"></i></a>
                    </div>
                </div>
                <div class="contact-info">
                    <h3>Area Layanan</h3>
                    <p><i class="fas fa-check"></i> Lamongan</p>
                    <p><i class="fas fa-check"></i> Tuban</p>
                    <p><i class="fas fa-check"></i> Surabaya</p>
                    <p><i class="fas fa-check"></i> Gresik</p>
                    <p><i class="fas fa-check"></i> Bojonegoro</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-container">
                <div class="footer-col">
                    <h3>SANG SURYA LANDSCAPE</h3>
                    <p>Spesialis jasa desain, pembuatan, dan perawatan taman profesional untuk hunian dan komersial.</p>
                    <div class="social-links">
                        <a href="#"><i class="fab fa-facebook-f"></i></a>
                        <a href="#"><i class="fab fa-instagram"></i></a>
                        <a href="https://wa.me/6285334398018"><i class="fab fa-whatsapp"></i></a>
                    </div>
                </div>
                <div class="footer-col">
                    <h3>Layanan</h3>
                    <ul class="footer-links">
                        <li><a href="#">Desain Taman</a></li>
                        <li><a href="#">Pembuatan Taman</a></li>
                        <li><a href="#">Perawatan Taman</a></li>
                        <li><a href="#">Taman Vertikal</a></li>
                        <li><a href="#">Kolam Hias</a></li>
                    </ul>
                </div>
                <div class="footer-col">
                    <h3>Link Cepat</h3>
                    <ul class="footer-links">
                        <li><a href="#home">Beranda</a></li>
                        <li><a href="#services">Layanan</a></li>
                        <li><a href="#about">Tentang Kami</a></li>
                        <li><a href="#portfolio">Portfolio</a></li>
                        <li><a href="#contact">Kontak</a></li>
                    </ul>
                </div>
                <div class="footer-col">
                    <h3>Kontak</h3>
                    <p><i class="fas fa-map-marker-alt"></i> UTARA PKU GEMPOL PADING RT 02 RW 01, PUCUK KABUPATEN LAMONGAN PROVINSI JAWA TIMUR</p>
                    <p><i class="fas fa-phone"></i> +62 853 3439 8018</p>
                    <p><i class="fas fa-envelope"></i> EMAIL NYA SANG SURYA APA? HEHE</p>
                </div>
            </div>
            <div class="copyright">
                <p>&copy; 2023 SANG SURYA LANDSCAPE. All Rights Reserved.</p>
            </div>
        </div>
    </footer>
</body>
</html>
