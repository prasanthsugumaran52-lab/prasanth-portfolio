# prasanth-portfolio
My personal portfolio website built using HTML, CSS and JavaScript.
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Prasanth Sugumaran | Portfolio</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
            font-family: Arial, sans-serif;
        }

        body {
            background: #0b1120;
            color: white;
        }

        /* Navigation */
        nav {
            position: fixed;
            top: 0;
            width: 100%;
            background: rgba(11, 17, 32, 0.95);
            padding: 18px 8%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            z-index: 1000;
        }

        .logo {
            font-size: 24px;
            font-weight: bold;
            color: #38bdf8;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 25px;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
            font-size: 16px;
            transition: 0.3s;
        }

        nav ul li a:hover {
            color: #38bdf8;
        }

        /* Home */
        #home {
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            padding: 100px 20px 40px;
            background: linear-gradient(135deg, #0b1120, #172554);
        }

        .home-content h1 {
            font-size: 55px;
            margin-bottom: 15px;
        }

        .home-content h1 span {
            color: #38bdf8;
        }

        .home-content h2 {
            font-size: 28px;
            color: #cbd5e1;
            margin-bottom: 20px;
        }

        .home-content p {
            max-width: 650px;
            margin: auto;
            line-height: 1.7;
            color: #94a3b8;
        }

        .btn {
            display: inline-block;
            margin-top: 30px;
            padding: 13px 28px;
            background: #38bdf8;
            color: #06111f;
            text-decoration: none;
            border-radius: 30px;
            font-weight: bold;
            transition: 0.3s;
        }

        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 25px rgba(56, 189, 248, 0.35);
        }

        /* Common Section */
        section {
            padding: 90px 8%;
        }

        .section-title {
            text-align: center;
            font-size: 35px;
            margin-bottom: 45px;
            color: #38bdf8;
        }

        /* About */
        .about {
            max-width: 850px;
            margin: auto;
            text-align: center;
            line-height: 1.8;
            color: #cbd5e1;
        }

        /* Skills */
        .skills-container {
            max-width: 900px;
            margin: auto;
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 20px;
        }

        .skill {
            background: #111827;
            padding: 25px 15px;
            text-align: center;
            border-radius: 15px;
            border: 1px solid #1e3a5f;
            transition: 0.3s;
        }

        .skill:hover {
            transform: translateY(-7px);
            border-color: #38bdf8;
        }

        .skill h3 {
            margin-top: 10px;
            color: #e2e8f0;
        }

        .skill-icon {
            font-size: 35px;
        }

        /* Education */
        .education {
            max-width: 800px;
            margin: auto;
        }

        .education-box {
            background: #111827;
            padding: 25px;
            margin-bottom: 20px;
            border-left: 4px solid #38bdf8;
            border-radius: 10px;
        }

        .education-box h3 {
            color: #38bdf8;
            margin-bottom: 8px;
        }

        .education-box p {
            color: #cbd5e1;
            line-height: 1.6;
        }

        /* Projects */
        .projects-container {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 25px;
        }

        .project {
            background: #111827;
            padding: 30px;
            border-radius: 15px;
            transition: 0.3s;
            border: 1px solid #1e293b;
        }

        .project:hover {
            transform: translateY(-8px);
            border-color: #38bdf8;
        }

        .project h3 {
            color: #38bdf8;
            margin-bottom: 12px;
        }

        .project p {
            color: #94a3b8;
            line-height: 1.6;
        }

        /* Contact */
        .contact {
            text-align: center;
        }

        .contact p {
            color: #cbd5e1;
            margin: 12px;
        }

        .contact strong {
            color: #38bdf8;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 25px;
            background: #060b14;
            color: #94a3b8;
        }

        /* Responsive */
        @media (max-width: 800px) {
            nav {
                padding: 15px 5%;
            }

            nav ul {
                gap: 12px;
            }

            nav ul li a {
                font-size: 13px;
            }

            .home-content h1 {
                font-size: 40px;
            }

            .home-content h2 {
                font-size: 22px;
            }

            .skills-container {
                grid-template-columns: repeat(2, 1fr);
            }

            .projects-container {
                grid-template-columns: 1fr;
            }
        }

        @media (max-width: 500px) {
            nav {
                flex-direction: column;
                gap: 10px;
            }

            .skills-container {
                grid-template-columns: 1fr;
            }

            section {
                padding: 70px 6%;
            }
        }
    </style>
</head>

<body>

    <!-- Navigation -->
    <nav>
        <div class="logo">PS</div>

        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#skills">Skills</a></li>
            <li><a href="#education">Education</a></li>
            <li><a href="#projects">Projects</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>


    <!-- Home -->
    <section id="home">
        <div class="home-content">

            <h1>Hello, I'm <span>Prasanth Sugumaran</span></h1>

            <h2>Student & Future Developer</h2>

            <p>
                Welcome to my personal portfolio website.
                I am interested in technology, programming,
                web development and creating innovative projects.
            </p>

            <a href="#about" class="btn">Explore My Portfolio</a>

        </div>
    </section>


    <!-- About -->
    <section id="about">

        <h2 class="section-title">About Me</h2>

        <div class="about">

            <p>
                Hi! I'm <strong>Prasanth Sugumaran</strong>.
                I am a passionate student interested in
                software development and modern technologies.
                I enjoy learning new programming concepts,
                developing projects and improving my technical skills.
            </p>

        </div>

    </section>


    <!-- Skills -->
    <section id="skills">

        <h2 class="section-title">My Skills</h2>

        <div class="skills-container">

            <div class="skill">
                <div class="skill-icon">🌐</div>
                <h3>HTML & CSS</h3>
            </div>

            <div class="skill">
                <div class="skill-icon">⚡</div>
                <h3>JavaScript</h3>
            </div>

            <div class="skill">
                <div class="skill-icon">🐍</div>
                <h3>Python</h3>
            </div>

            <div class="skill">
                <div class="skill-icon">☕</div>
                <h3>Java</h3>
            </div>

            <div class="skill">
                <div class="skill-icon">📱</div>
                <h3>Android Development</h3>
            </div>

            <div class="skill">
                <div class="skill-icon">🎨</div>
                <h3>UI/UX Design</h3>
            </div>

            <div class="skill">
                <div class="skill-icon">🗄️</div>
                <h3>Database</h3>
            </div>

            <div class="skill">
                <div class="skill-icon">🧠</div>
                <h3>Problem Solving</h3>
            </div>

        </div>

    </section>


    <!-- Education -->
    <section id="education">

        <h2 class="section-title">Education</h2>

        <div class="education">

            <div class="education-box">
                <h3>College</h3>
                <p>
                    Currently pursuing my college education
                    and developing my technical knowledge
                    through academic and practical projects.
                </p>
            </div>

            <div class="education-box">
                <h3>Technical Learning</h3>
                <p>
                    Learning programming, software engineering,
                    data management, Android development,
                    networking and modern technologies.
                </p>
            </div>

        </div>

    </section>


    <!-- Projects -->
    <section id="projects">

        <h2 class="section-title">My Projects</h2>

        <div class="projects-container">

            <div class="project">
                <h3>🏨 Smart Hostel System</h3>
                <p>
                    A concept for managing hostel-related
                    activities using a smart digital system.
                </p>
            </div>

            <div class="project">
                <h3>🏎️ Car Racing Game</h3>
                <p>
                    A browser-based racing game developed
                    using HTML, CSS and JavaScript.
                </p>
            </div>

            <div class="project">
                <h3>💻 Personal Portfolio</h3>
                <p>
                    A responsive personal portfolio website
                    designed to showcase my skills and projects.
                </p>
            </div>

        </div>

    </section>


    <!-- Contact -->
    <section id="contact">

        <h2 class="section-title">Contact Me</h2>

        <div class="contact">

            <p>
                <strong>Name:</strong> Prasanth Sugumaran
            </p>

            <p>
                <strong>Email:</strong> yourmail@example.com
            </p>

            <p>
                <strong>Location:</strong> Tamil Nadu, India
            </p>

            <a href="mailto:yourmail@example.com" class="btn">
                Send Email
            </a>

        </div>

    </section>


    <!-- Footer -->
    <footer>
        <p>
            © 2026 Prasanth Sugumaran. All Rights Reserved.
        </p>
    </footer>

</body>
</html>