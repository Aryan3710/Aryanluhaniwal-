<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aak Portfolio</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
        }

        body {
            background-color: #f5f5f5;
        }

        /* Navigation */
        nav {
            background-color: #333;
            padding: 1rem 5%;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }

        nav ul {
            display: flex;
            justify-content: flex-end;
            list-style: none;
        }

        nav ul li {
            margin-left: 2rem;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
            font-size: 1.1rem;
        }

        /* Header Section */
        .header {
            height: 100vh;
            display: flex;
            align-items: center;
            padding: 0 5%;
            background-color: #2c3e50;
            color: white;
        }

        .header-content {
            max-width: 600px;
        }

        .header-content h1 {
            font-size: 3.5rem;
            margin-bottom: 1rem;
        }

        .header-content p {
            font-size: 1.2rem;
            margin-bottom: 2rem;
        }

        .profile-img {
            width: 300px;
            height: 300px;
            border-radius: 50%;
            margin-left: auto;
        }

        /* Skills Section */
        .skills {
            padding: 5rem 5%;
        }

        .skills h2 {
            text-align: center;
            margin-bottom: 3rem;
        }

        .skills-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }

        .skill-card {
            background-color: white;
            padding: 2rem;
            border-radius: 10px;
            text-align: center;
        }

        /* Projects Section */
        .projects {
            padding: 5rem 5%;
            background-color: #ecf0f1;
        }

        .projects h2 {
            text-align: center;
            margin-bottom: 3rem;
        }

        .project-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .project-card {
            background-color: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }

        .project-card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }

        .project-info {
            padding: 1.5rem;
        }

        /* Contact Section */
        .contact {
            padding: 5rem 5%;
            text-align: center;
        }

        .contact-form {
            max-width: 600px;
            margin: 0 auto;
        }

        .contact-form input,
        .contact-form textarea {
            width: 100%;
            padding: 1rem;
            margin-bottom: 1rem;
            border: 1px solid #ddd;
            border-radius: 5px;
        }

        .btn {
            display: inline-block;
            padding: 1rem 2rem;
            background-color: #3498db;
            color: white;
            text-decoration: none;
            border-radius: 5px;
            transition: background-color 0.3s;
        }

        .btn:hover {
            background-color: #2980b9;
        }

        /* Footer */
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 2rem 5%;
        }

        .social-links {
            margin-bottom: 1rem;
        }

        .social-links a {
            color: white;
            margin: 0 1rem;
            font-size: 1.5rem;
        }
    </style>
</head>
<body>
    <!-- Navigation -->
    <nav>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#skills">Skills</a></li>
            <li><a href="#projects">Projects</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <!-- Header Section -->
    <header class="header" id="home">
        <div class="header-content">
            <h1>Hi, I'm Aak</h1>
            <p>Web Developer & Designer</p>
            <p>Creating beautiful and functional websites</p>
            <a href="#contact" class="btn">Get in Touch</a>
        </div>
        <img src="img/1.webp" alt="Profile Image" class="profile-img">
    </header>

    <!-- Skills Section -->
    <section class="skills" id="skills">
        <h2>My Skills</h2>
        <div class="skills-container">
            <div class="skill-card">
                <h3>Web Development</h3>
                <p>HTML, CSS, JavaScript</p>
            </div>
            <div class="skill-card">
                <h3>UI/UX Design</h3>
                <p>Figma, Adobe XD</p>
            </div>
            <div class="skill-card">
                <h3>Backend</h3>
                <p>Node.js, MongoDB</p>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section class="projects" id="projects">
        <h2>My Projects</h2>
        <div class="project-grid">
            <div class="project-card">
                <img src="project1.jpg" alt="Project 1">
                <div class="project-info">
                    <h3>E-commerce Website</h3>
                    <p>Full-stack e-commerce platform with payment gateway</p>
                </div>
            </div>
            <div class="project-card">
                <img src="project2.jpg" alt="Project 2">
                <div class="project-info">
                    <h3>Portfolio Website</h3>
                    <p>Responsive portfolio website with modern design</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="contact" id="contact">
        <h2>Contact Me</h2>
        <form class="contact-form">
            <input type="text" placeholder="Name" required>
            <input type="email" placeholder="Email" required>
            <textarea rows="5" placeholder="Message" required></textarea>
            <button type="submit" class="btn">Send Message</button>
        </form>
    </section>

    <!-- Footer -->
    <footer>
        <div class="social-links">
            <a href="#"><i class="fab fa-github"></i></a>
            <a href="#"><i class="fab fa-linkedin"></i></a>
            <a href="#"><i class="fab fa-twitter"></i></a>
        </div>
        <p>&copy; 2023 Aak. All rights reserved</p>
    </footer>
</body>
</html>
