<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Glow Fit Gyms</title>
<style>
    /* Reset */
    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }

    body {
        font-family: Arial, sans-serif;
        background: linear-gradient(135deg, #0f2027, #203a43, #2c5364);
        color: white;
        line-height: 1.6;
        scroll-behavior: smooth;
    }

    /* Pill Navigation Bar */
    .navbar {
        position: fixed;
        top: 20px;
        left: 50%;
        transform: translateX(-50%);
        background: rgba(255, 255, 255, 0.1);
        backdrop-filter: blur(10px);
        border-radius: 50px;
        padding: 10px 30px;
        display: flex;
        justify-content: space-between;
        align-items: center;
        width: 80%;
        z-index: 1000;
        box-shadow: 0 4px 20px rgba(0,0,0,0.3);
    }

    .logo {
        font-size: 1.5rem;
        font-weight: bold;
        color: #ffcc00;
    }

    .nav-links {
        display: flex;
        gap: 20px;
    }

    .nav-links a {
        color: white;
        text-decoration: none;
        font-weight: bold;
        padding: 8px 15px;
        border-radius: 25px;
        transition: all 0.3s ease;
    }

    .nav-links a:hover {
        background: #ffcc00;
        color: black;
        transform: scale(1.1);
    }

    /* Hero Section */
    .hero {
        height: 100vh;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        text-align: center;
        background: url('https://media0.giphy.com/media/v1.Y2lkPTc5MGI3NjExNDZyaTNnMnFzdHM4c2doODl0NG85bncyem1rc204eHB0YzcyM2hoYiZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/3o6ZsYzuLyRfSGX4f6/giphy.gif') center/cover no-repeat;
        position: relative;
    }

    .hero::after {
        content: "";
        position: absolute;
        top: 0; left: 0;
        width: 100%; height: 100%;
        background: rgba(0,0,0,0.5);
    }

    .hero-content {
        position: relative;
        z-index: 1;
        animation: fadeIn 2s ease-in-out;
    }

    .hero h2 {
        font-size: 2.5rem;
        margin-bottom: 20px;
    }

    .btn {
        background: #ffcc00;
        color: black;
        padding: 12px 25px;
        border: none;
        font-size: 1rem;
        cursor: pointer;
        transition: 0.3s;
        border-radius: 5px;
    }

    .btn:hover {
        background: #ffaa00;
    }

    /* Sections */
    section {
        padding: 80px 20px;
        text-align: center;
    }

    /* Animations */
    @keyframes fadeIn {
        from { opacity: 0; transform: translateY(20px); }
        to { opacity: 1; transform: translateY(0); }
    }

    /* Footer */
    footer {
        padding: 20px;
        text-align: center;
        background: rgba(0,0,0,0.6);
    }
    <style>
        </style>
    </head>
<body>

<!-- Navigation Bar -->
<div class="navbar">
    <div class="logo">Glow Fit Gyms</div>
    <div class="nav-links">
        <a href="#about" onclick="playClick()">About Us</a>
        <a href="#info" onclick="playClick()">Information</a>
        <a href="#more" onclick="playClick()">More</a>
    </div>
</div>

<!-- Hero Section -->
<section class="hero">
    <div class="hero-content">
        <h2>Transform Your Body, Transform Your Life</h2>
        <button class="btn" onclick="playClick()">Join Now</button>
    </div>
</section>

<!-- About Us -->
<section id="about">
    <h2>About Us</h2>
    <p>Welcome to Glow Fit Gym — your ultimate fitness destination. We offer world-class equipment, expert trainers, and a motivating environment to help you achieve your goals.</p>
</section>

<!-- Information -->
<section id="info">
    <h2>Information</h2>
    <p>We provide weight training, cardio, yoga, and personal training sessions. Open 24/7 with flexible membership plans.</p>
</section>

<!-- More -->
<section id="more">
    <h2>More</h2>
    <p>Check out our gallery, pricing plans, and special offers. Join the DJ Gym family today!</p>
</section>

<!-- Footer -->
<footer>
    <p>© 2026 Glow Fit Gyms. All Rights Reserved.</p>
</footer>

<!-- Sound Effect -->
<audio id="clickSound" src="https://www.soundjay.com/buttons/sounds/button-16.mp3" preload="auto"></audio>

<script>
    function playClick() {
        document.getElementById('clickSound').play();
    }
</script>
   /* Image gallery */
   .gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
            padding: 20px;
        }

        .gallery a {
            text-decoration: none;
            color: white;
        }
        .gallery a:hover img {
            transform: scale(1.05);
            box-shadow: 0 8px 20px rgba(0,0,0,0.3);
        }
        .gallery img {
            width: 550px;
            height: 360px;
            object-fit: cover;
            border-radius: 10px;
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .gallery img:hover {
            transform: scale(1.05);
            box-shadow: 0 8px 20px rgba(0,0,0,0.3);
        }
        <!-- IMAGE GALLERY WITH LINKS -->
    <section class="gallery">
        <a href="https://example.com" target="_blank">
            <img src="https://static.vecteezy.com/system/resources/previews/026/781/389/non_2x/gym-interior-background-of-dumbbells-on-rack-in-fitness-and-workout-room-photo.jpg" alt="Project 1" width="250" height="160">
        </a>
        <a href="https://example.com" target="_blank">
            <img src="https://media4.giphy.com/media/v1.Y2lkPTc5MGI3NjExOTBjbzE1NGYzZmlyaTkydnAzaWxnbGhtbTdhNmRzejRkbmQ1M3d2aSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/Oqj4dDZGas34lCBScR/giphy.gif" alt="Project 2" width="250" height="160">
        </a>
        <a href="https://example.com" target="_blank">
            <img src="https://img.freepik.com/premium-photo/blurry-photo-modern-gym-with-sports-equipment-exercise-machines-concept-gym-sports-equipment-exercise-machines-blurry-modern_918839-74570.jpg?w=2000" alt="Project 3" width="250" height="160">
        </a>
    </section>
</body>
</html>
