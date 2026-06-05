<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Box Mapping Assignment</title>

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial, sans-serif;
}

body{
    background:#f4f4f4;
}

/* ================= NAVBAR ================= */

.navbar{
    background:#111827;
    padding:20px 60px;

    display:flex;
    justify-content:space-between;
    align-items:center;

    border:4px solid #00d4ff;
}

.logo{
    color:#00d4ff;
    font-size:30px;
    font-weight:bold;
}

.nav-links{
    display:flex;
    gap:25px;
}

.nav-links a{
    color:white;
    text-decoration:none;
    font-size:18px;
}

.search-box{
    display:flex;
    gap:10px;
}

.search-box input{
    padding:10px;
    border:none;
    border-radius:5px;
}

.search-box button{
    padding:10px 18px;
    background:#00d4ff;
    border:none;
    border-radius:5px;
    font-weight:bold;
    cursor:pointer;
}

/* ================= HERO SECTION ================= */

.hero{
    background:#dbeafe;
    margin:30px;
    padding:60px;

    display:flex;
    justify-content:space-between;
    align-items:center;
    gap:40px;

    border:4px solid #2563eb;
}

.hero-left{
    width:50%;
    background:white;
    padding:40px;
    border-radius:15px;
    border:4px solid #00d4ff;
}

.tagline{
    background:#00d4ff;
    display:inline-block;
    padding:10px 20px;
    border-radius:20px;
    margin-bottom:25px;
    font-weight:bold;
}

.hero-left h1{
    font-size:55px;
    color:#111827;
    margin-bottom:25px;
}

.hero-left p{
    font-size:18px;
    color:#555;
    line-height:1.7;
    margin-bottom:30px;
}

.hero-buttons{
    display:flex;
    gap:15px;
}

.primary-btn{
    padding:14px 28px;
    background:#111827;
    color:white;
    border:none;
    border-radius:8px;
    font-size:16px;
    cursor:pointer;
}

.secondary-btn{
    padding:14px 28px;
    background:#00d4ff;
    color:black;
    border:none;
    border-radius:8px;
    font-size:16px;
    cursor:pointer;
}

.hero-right{
    width:50%;
}

.hero-right img{
    width:100%;
    border-radius:20px;
    border:4px solid #111827;
}

/* ================= FEATURES SECTION ================= */

.features{
    background:#111827;
    margin:30px;
    padding:60px;
    color:white;

    border:4px solid #00d4ff;
}

.feature-top{
    background:#1f2937;
    padding:40px;
    border-radius:15px;
    margin-bottom:40px;
}

.feature-top span{
    color:#00d4ff;
    font-size:18px;
    font-weight:bold;
}

.feature-top h2{
    font-size:45px;
    margin:15px 0;
}

.feature-top p{
    color:#d1d5db;
    font-size:18px;
}

.feature-cards{
    background:#374151;
    padding:30px;
    border-radius:15px;

    display:flex;
    gap:25px;
}

.card{
    background:white;
    color:black;
    padding:30px;
    border-radius:15px;
    width:33%;
}

.icon{
    width:70px;
    height:70px;
    background:#00d4ff;
    border-radius:10px;
    margin-bottom:20px;
}

.card h3{
    margin-bottom:15px;
    font-size:25px;
}

.card p{
    color:#555;
    line-height:1.7;
}

/* ================= TESTIMONIALS ================= */

.testimonials{
    background:#fef3c7;
    margin:30px;
    padding:60px;

    border:4px solid #f59e0b;
}

.testimonial-top{
    background:white;
    padding:40px;
    border-radius:15px;
    margin-bottom:40px;

    display:flex;
    gap:30px;
}

.title-box{
    width:50%;
    background:#dbeafe;
    padding:30px;
    border-radius:10px;
}

.subtext-box{
    width:50%;
    background:#dcfce7;
    padding:30px;
    border-radius:10px;
}

.title-box h2{
    font-size:40px;
}

.subtext-box p{
    font-size:18px;
    line-height:1.7;
}

.testimonial-cards{
    background:#fde68a;
    padding:30px;
    border-radius:15px;

    display:flex;
    gap:25px;
}

.testimonial-card{
    background:white;
    padding:30px;
    border-radius:15px;
    width:33%;
}

.quote{
    font-size:17px;
    line-height:1.7;
    margin-bottom:20px;
}

.stars{
    color:gold;
    font-size:25px;
    margin-bottom:25px;
}

.user{
    display:flex;
    align-items:center;
    gap:15px;
}

.user-image{
    width:60px;
    height:60px;
    background:#00d4ff;
    border-radius:50%;
}

.user-info span{
    display:block;
}

/* ================= FOOTER ================= */

.footer{
    background:#111827;
    color:white;
    margin:30px;
    padding:60px;

    border:4px solid #00d4ff;
}

.footer-top{
    display:flex;
    gap:25px;
    margin-bottom:40px;
}

.footer-box{
    background:#1f2937;
    padding:30px;
    border-radius:15px;
    width:33%;
}

.footer-box a{
    color:#00d4ff;
    text-decoration:none;
    font-size:28px;
    font-weight:bold;
}

.footer-box p{
    margin:20px 0;
    line-height:1.7;
}

.brand{
    background:#00d4ff;
    color:black;
    padding:12px;
    border-radius:8px;
    text-align:center;
    font-weight:bold;
}

.copyright{
    background:#374151;
    padding:20px;
    border-radius:10px;
    text-align:center;
}

</style>
</head>

<body>

<!-- ================= NAVBAR ================= -->

<div class="navbar">

    <div class="logo">AI TECH</div>

    <div class="nav-links">
        <a href="#">Home</a>
        <a href="#">About</a>
        <a href="#">Services</a>
        <a href="#">Contact</a>
    </div>

    <div class="search-box">
        <input type="text" placeholder="Search Here">
        <button>Search</button>
    </div>

</div>

<!-- ================= HERO SECTION ================= -->

<div class="hero">

    <div class="hero-left">

        <div class="tagline">
            <p>Modern AI Website</p>
        </div>

        <h1>Build Creative Websites With AI</h1>

        <p>
            Design beautiful and modern websites with responsive layouts,
            smooth user experience and colorful UI sections.
        </p>

        <div class="hero-buttons">
            <button class="primary-btn">Get Started</button>
            <button class="secondary-btn">Learn More</button>
        </div>

    </div>

    <div class="hero-right">

        <img src="https://images.unsplash.com/photo-1518770660439-4636190af475?q=80&w=1200&auto=format&fit=crop" alt="AI Image">

    </div>

</div>

<!-- ================= FEATURES SECTION ================= -->

<div class="features">

    <div class="feature-top">

        <span>FEATURES</span>

        <h2>Our Best Features</h2>

        <p>
            Explore modern and professional website features with clean layouts.
        </p>

    </div>

    <div class="feature-cards">

        <div class="card">

            <div class="icon"></div>

            <h3>Fast Performance</h3>

            <p>
                Optimized website speed with smooth and responsive layouts.
            </p>

        </div>

        <div class="card">

            <div class="icon"></div>

            <h3>Creative Design</h3>

            <p>
                Attractive UI design with colorful sections and modern style.
            </p>

        </div>

        <div class="card">

            <div class="icon"></div>

            <h3>Responsive Layout</h3>

            <p>
                Fully responsive website design for mobile and desktop screens.
            </p>

        </div>

    </div>

</div>

<!-- ================= TESTIMONIALS ================= -->

<div class="testimonials">

    <div class="testimonial-top">

        <div class="title-box">
            <h2>What Clients Say</h2>
        </div>

        <div class="subtext-box">
            <p>
                Read our customer feedback and explore how our AI designs
                helped businesses create modern websites.
            </p>
        </div>

    </div>

    <div class="testimonial-cards">

        <div class="testimonial-card">

            <p class="quote">
                “Amazing website design with creative sections and modern UI.”
            </p>

            <div class="stars">
                ★★★★★
            </div>

            <div class="user">

                <div class="user-image"></div>

                <div class="user-info">
                    <span><b>Ali Khan</b></span>
                    <span>Web Developer</span>
                </div>

            </div>

        </div>

        <div class="testimonial-card">

            <p class="quote">
                “The colorful box mapping style looks professional and clean.”
            </p>

            <div class="stars">
                ★★★★★
            </div>

            <div class="user">

                <div class="user-image"></div>

                <div class="user-info">
                    <span><b>Sara Ahmed</b></span>
                    <span>UI Designer</span>
                </div>

            </div>

        </div>

        <div class="testimonial-card">

            <p class="quote">
                “Responsive layout and smooth structure made the project amazing.”
            </p>

            <div class="stars">
                ★★★★★
            </div>

            <div class="user">

                <div class="user-image"></div>

                <div class="user-info">
                    <span><b>Umair Malik</b></span>
                    <span>Frontend Expert</span>
                </div>

            </div>

        </div>

    </div>

</div>

<!-- ================= FOOTER ================= -->

<div class="footer">

    <div class="footer-top">

        <div class="footer-box">

            <a href="#">AI TECH</a>

            <p>
                Modern AI solutions for creative and responsive website design.
            </p>

            <div class="brand">
                Creative Brand
            </div>

        </div>

        <div class="footer-box">

            <a href="#">SERVICES</a>

            <p>
                Web Design, UI/UX, Frontend Development and AI Solutions.
            </p>

            <div class="brand">
                Premium Services
            </div>

        </div>

        <div class="footer-box">

            <a href="#">CONTACT</a>

            <p>
                Email, social media and customer support available 24/7.
            </p>

            <div class="brand">
                Support Team
            </div>

        </div>

    </div>

    <div class="copyright">

        <p>© 2026 AI TECH | All Rights Reserved</p>

    </div>

</div>

</body>
</html>
