# f4-black-birds22025
Sample Project
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Indian F4 Black Birds - Official Team</title>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;700&display=swap">
    <style>
        :root {
            --ferrari-red: #e10600;
            --carbon-black: #1a1a1a;
            --carbon-fiber: #2a2a2a;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Roboto', sans-serif;
        }

        body {
            background: var(--carbon-black);
            color: white;
            overflow-x: hidden;
        }

        .hero {
            height: 100vh;
            position: relative;
            overflow: hidden;
        }

        .hero video {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            object-fit: cover;
            z-index: -1;
        }

        .nav {
            position: fixed;
            top: 0;
            width: 100%;
            padding: 20px;
            background: rgba(0,0,0,0.8);
            z-index: 100;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .nav img {
            height: 40px;
        }

        .nav-links {
            display: flex;
            gap: 30px;
        }

        .nav-links a {
            color: white;
            text-decoration: none;
            font-weight: 600;
            letter-spacing: 1px;
            transition: color 0.3s;
        }

        .nav-links a:hover {
            color: var(--ferrari-red);
        }

        .content {
            padding: 100px 10%;
        }

        .section {
            margin: 100px 0;
        }

        .team-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 50px;
        }

        .team-member {
            background: rgba(255,255,255,0.05);
            padding: 20px;
            border-radius: 10px;
            text-align: center;
        }

        .team-member img {
            width: 200px;
            height: 200px;
            border-radius: 50%;
            object-fit: cover;
            margin: 0 auto 20px;
            border: 3px solid var(--ferrari-red);
        }

        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.05); }
            100% { transform: scale(1); }
        }

        .car-showcase {
            text-align: center;
            padding: 50px 0;
            animation: pulse 3s infinite;
        }

        .car-showcase img {
            max-width: 80%;
            margin: 20px auto;
            border: 2px solid var(--ferrari-red);
            border-radius: 10px;
        }

        .schedule {
            background: rgba(255,255,255,0.05);
            padding: 30px;
            border-radius: 10px;
            margin: 50px 0;
        }

        .schedule h3 {
            color: var(--ferrari-red);
            margin-bottom: 20px;
        }

        .schedule-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }

        .schedule-item {
            padding: 15px;
            border: 1px solid rgba(255,255,255,0.1);
            border-radius: 5px;
        }

        .sponsors {
            display: flex;
            flex-wrap: wrap;
            gap: 30px;
            justify-content: center;
            margin: 50px 0;
        }

        .sponsor img {
            height: 80px;
            filter: brightness(0) invert(1);
            opacity: 0.7;
            transition: opacity 0.3s;
        }

        .sponsor img:hover {
            opacity: 1;
        }

        .contact-form {
            max-width: 600px;
            margin: 50px auto;
            background: rgba(255,255,255,0.05);
            padding: 30px;
            border-radius: 10px;
        }

        .contact-form input, .contact-form textarea {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            background: rgba(255,255,255,0.1);
            border: 1px solid rgba(255,255,255,0.2);
            color: white;
        }

        .contact-form button {
            background: var(--ferrari-red);
            color: white;
            padding: 12px 30px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background 0.3s;
        }

        .contact-form button:hover {
            background: #ff1a00;
        }

        footer {
            background: rgba(0,0,0,0.9);
            padding: 50px 10%;
            text-align: center;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin: 20px 0;
        }

        .social-links a {
            color: white;
            font-size: 24px;
            transition: color 0.3s;
        }

        .social-links a:hover {
            color: var(--ferrari-red);
        }

        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }
            .content {
                padding: 80px 5%;
            }
        }
    </style>
</head>
<body>
    <nav class="nav">
        <img src="https://via.placeholder.com/200x40/333/fff?text=IMA+LOGO" alt="IMA Logo">
        <div class="nav-links">
            <a href="#about">About</a>
            <a href="#team">Team</a>
            <a href="#car">The Car</a>
            <a href="#schedule">Schedule</a>
            <a href="#contact">Contact</a>
        </div>
    </nav>

    <section class="hero">
        <video autoplay muted loop id="heroVideo">
            <source src="https://www.youtube.com/embed/VIDEO_ID?autoplay=1&mute=1&loop=1&controls=0" type="video/mp4">
        </video>
        <div style="position: absolute; bottom: 10%; left: 10%; color: white;">
            <h1 style="font-size: 4em; text-shadow: 2px 2px 4px #000;">INDIAN F4 BLACK BIRDS</h1>
            <p style="font-size: 1.5em;">Powering the Future of Indian Motorsports</p>
        </div>
    </section>

    <div class="content">
        <section id="about" class="section">
            <h2 style="color: var(--ferrari-red); margin-bottom: 30px;">About Us</h2>
            <p>Indian Motorsports Academy's premier F4 team, competing in the Indian F4 Championship with cutting-edge engineering and driver development.</p>
        </section>

        <section id="car" class="section">
            <h2 style="color: var(--ferrari-red); margin-bottom: 30px;">The Machine</h2>
            <div class="car-showcase">
                <img src="https://images.unsplash.com/photo-1588943211347-0905a1b7634c?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="F4 Car">
                <p>Our custom-built F4 machine features:</p>
                <ul style="text-align: left; max-width: 600px; margin: 20px auto;">
                    <li>Carbon fiber monocoque chassis</li>
                    <li>Renault 2.0L turbocharged engine</li>
                    <li>Advanced aerodynamics package</li>
                    <li>State-of-the-art data acquisition systems</li>
                </ul>
            </div>
        </section>

        <section id="team" class="section">
            <h2 style="color: var(--ferrari-red); margin-bottom: 30px;">Our Team</h2>
            <div class="team-grid">
                <div class="team-member">
                    <img src="https://randomuser.me/api/portraits/men/32.jpg" alt="Driver">
                    <h3>Arjun Singh</h3>
                    <p>Lead Driver</p>
                </div>
                <div class="team-member">
                    <img src="https://randomuser.me/api/portraits/women/44.jpg" alt="Driver">
                    <h3>Priya Sharma</h3>
                    <p>Development Driver</p>
                </div>
                <div class="team-member">
                    <img src="https://randomuser.me/api/portraits/men/65.jpg" alt="Engineer">
                    <h3>Rajiv Mehta</h3>
                    <p>Technical Director</p>
                </div>
            </div>
        </section>

        <section id="schedule" class="section">
            <h2 style="color: var(--ferrari-red); margin-bottom: 30px;">2025 Race Schedule</h2>
            <div class="schedule">
                <div class="schedule-grid">
                    <div class="schedule-item">
                        <h3>Round 1</h3>
                        <p>Buddh International Circuit</p>
                        <p>March 15-16</p>
                    </div>
                    <div class="schedule-item">
                        <h3>Round 2</h3>
                        <p>Chennai Street Circuit</p>
                        <p>April 12-13</p>
                    </div>
                    <div class="schedule-item">
                        <h3>Round 3</h3>
                        <p>Hyderabad International Circuit</p>
                        <p>May 24-25</p>
                    </div>
                </div>
            </div>
        </section>

        <section class="section">
            <h2 style="color: var(--ferrari-red); margin-bottom: 30px;">Our Sponsors</h2>
            <div class="sponsors">
                <div class="sponsor"><img src="https://via.placeholder.com/150x80/333/fff?text=SPONSOR+1" alt="Sponsor"></div>
                <div class="sponsor"><img src="https://via.placeholder.com/150x80/333/fff?text=SPONSOR+2" alt="Sponsor"></div>
                <div class="sponsor"><img src="https://via.placeholder.com/150x80/333/fff?text=SPONSOR+3" alt="Sponsor"></div>
            </div>
        </section>

        <section id="contact" class="section">
            <h2 style="color: var(--ferrari-red); margin-bottom: 30px;">Contact Us</h2>
            <div class="contact-form">
                <form>
                    <input type="text" placeholder="Name" required>
                    <input type="email" placeholder="Email" required>
                    <input type="text" placeholder="Subject">
                    <textarea rows="5" placeholder="Message"></textarea>
                    <button type="submit">Send Message</button>
                </form>
            </div>
        </section>
    </div>

    <footer>
        <div class="social-links">
            <a href="#"><i>FB</i></a>
            <a href="#"><i>TW</i></a>
            <a href="#"><i>IG</i></a>
            <a href="#"><i>YT</i></a>
        </div>
        <p>&copy; 2025 Indian Motorsports Academy. All rights reserved.</p>
    </footer>

    <script>
        // Add smooth scrolling
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });

        // Video hover effect
        const video = document.getElementById('heroVideo');
        video.addEventListener('mouseover', () => {
            video.playbackRate = 1.5;
        });
        video.addEventListener('mouseout', () => {
            video.playbackRate = 1;
        });
    </script>
</body>
</html>
