<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Glenn John M. Padroncillo | BSIT 2B</title>

    <style>
        /* =====================================================
           POLISHED GREEN + YELLOW STUDENT PORTFOLIO
           ===================================================== */

        :root {
            --dark-green: #12372e;
            --deep-green: #174d3d;
            --green: #25805f;
            --green-hover: #176044;
            --green-soft: #e8f5ed;

            --yellow: #f2c94c;
            --yellow-dark: #c89a1f;
            --yellow-soft: #fff5cc;

            --cream: #fbfcf7;
            --white: #ffffff;
            --text: #26332e;
            --muted: #68756f;
            --border: #d9e5df;

            --shadow: 0 12px 30px rgba(18, 55, 46, 0.10);
            --shadow-hover: 0 20px 42px rgba(18, 55, 46, 0.17);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }
    body {
        font-family: Arial, Helvetica, sans-serif;
        color: var(--text);
        background:
            radial-gradient(
                circle at 10% 20%,
                rgba(242, 201, 76, 0.10),
                transparent 22%
            ),
            radial-gradient(
                circle at 90% 70%,
                rgba(37, 128, 95, 0.10),
                transparent 24%
            ),
            linear-gradient(
                135deg,
                #ffffff 0%,
                #f8fbf9 45%,
                #eef8f2 100%
            );
        background-attachment: fixed;
        line-height: 1.7;
    }

        a {
            color: var(--green);
            text-decoration: none;
            transition: 0.25s ease;
        }

        a:hover {
            color: var(--yellow-dark);
        }

        img,
        iframe {
            max-width: 100%;
        }

        .container {
            width: min(1100px, 92%);
            margin: 0 auto;
        }

        section {
            padding: 85px 0;
            scroll-margin-top: 90px;
        }

        h1,
        h2,
        h3 {
            font-family: Georgia, "Times New Roman", serif;
        }

        h2 {
            color: var(--dark-green);
            font-size: clamp(1.8rem, 4vw, 2.5rem);
            margin-bottom: 12px;
        }

        h2::after {
            content: "";
            display: block;
            width: 55px;
            height: 4px;
            margin-top: 10px;
            border-radius: 20px;
            background: var(--yellow);
        }

        .section-intro {
            max-width: 700px;
            color: var(--muted);
            margin-bottom: 32px;
        }

        /* =========================
           NAVIGATION
           ========================= */

        nav {
            position: sticky;
            top: 0;
            z-index: 1000;
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(12px);
            border-bottom: 2px solid var(--yellow);
            box-shadow: 0 5px 20px rgba(18, 55, 46, 0.07);
        }

        .nav-container {
            min-height: 74px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            gap: 20px;
        }

        .logo {
            color: var(--dark-green);
            font: bold 1.25rem Georgia, "Times New Roman", serif;
            white-space: nowrap;
        }

        .logo span {
            color: var(--yellow-dark);
        }

        .nav-links {
            display: flex;
            gap: 6px;
            flex-wrap: wrap;
            justify-content: flex-end;
        }

        .nav-links a {
            color: var(--dark-green);
            font-weight: bold;
            padding: 9px 14px;
            border-radius: 999px;
        }

        .nav-links a:hover {
            color: var(--dark-green);
            background: var(--yellow-soft);
            transform: translateY(-2px);
        }

        /* =========================
           HERO
           ========================= */
    .hero {
        min-height: 84vh;
        display: flex;
        align-items: center;
        position: relative;
        overflow: hidden;
        background:
            radial-gradient(
                circle at 85% 15%,
                rgba(242, 201, 76, 0.18),
                transparent 25%
            ),
            radial-gradient(
                circle at 8% 82%,
                rgba(37, 128, 95, 0.10),
                transparent 30%
            ),
            linear-gradient(
                135deg,
                #ffffff 0%,
                #f1f8f4 100%
            );
    }

        .hero::before {
            content: "";
            position: absolute;
            width: 230px;
            height: 230px;
            right: -90px;
            bottom: 60px;
            border: 1px solid rgba(37, 128, 95, 0.12);
            border-radius: 50%;
        }

        .hero-content {
            position: relative;
            z-index: 1;
            max-width: 820px;
        }

        .badge {
            display: inline-block;
            background: var(--yellow-soft);
            color: #695216;
            border: 1px solid #ead28c;
            padding: 8px 14px;
            border-radius: 999px;
            font-size: 0.82rem;
            font-weight: 800;
            margin-bottom: 20px;
        }

        .hero h1 {
            color: var(--dark-green);
            font-size: clamp(3rem, 8vw, 5.6rem);
            line-height: 0.98;
            letter-spacing: -0.04em;
            margin-bottom: 22px;
        }

        .hero h1 span {
            color: var(--green);
        }

        .hero-text {
            max-width: 730px;
            color: var(--muted);
            font-size: 1.08rem;
        }

        .hero-buttons {
            display: flex;
            flex-wrap: wrap;
            gap: 12px;
            margin-top: 30px;
        }

        .btn {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            padding: 12px 20px;
            border-radius: 11px;
            font-weight: 800;
            transition: 0.25s ease;
        }

        .btn-primary {
            background: var(--green);
            color: var(--white);
            box-shadow: 0 8px 18px rgba(37, 128, 95, 0.18);
        }

        .btn-primary:hover {
            background: var(--dark-green);
            color: var(--white);
            transform: translateY(-3px);
            box-shadow: var(--shadow-hover);
        }

        .btn-secondary {
            background: var(--yellow);
            color: var(--dark-green);
        }

        .btn-secondary:hover {
            background: var(--yellow-dark);
            color: var(--white);
            transform: translateY(-3px);
        }

        /* =========================
           ABOUT
           ========================= */

        .about-grid {
            display: grid;
            grid-template-columns: repeat(2, minmax(0, 1fr));
            gap: 24px;
        }

        .about-card {
            position: relative;
            overflow: hidden;
            background: var(--white);
            padding: 30px;
            border: 1px solid var(--border);
            border-radius: 20px;
            box-shadow: var(--shadow);
        }

        .about-card::before {
            content: "";
            position: absolute;
            left: 0;
            top: 0;
            width: 100%;
            height: 4px;
            background: linear-gradient(
                90deg,
                var(--green),
                var(--yellow)
            );
        }

        .about-card h3 {
            color: var(--dark-green);
            margin-bottom: 12px;
            font-size: 1.35rem;
        }

        .about-card strong {
            color: var(--green);
        }

        /* =========================
           SKILLS & HOBBIES
           ========================= */

        .cards {
            display: grid;
            grid-template-columns: repeat(2, minmax(0, 1fr));
            gap: 24px;
        }

        .card {
            position: relative;
            overflow: hidden;
            background: var(--white);
            padding: 30px;
            border: 1px solid var(--border);
            border-radius: 20px;
            border-top: 5px solid var(--yellow);
            box-shadow: var(--shadow);
            transition: 0.3s ease;
        }

        .card:hover {
            transform: translateY(-8px);
            box-shadow: var(--shadow-hover);
        }

        .card::after {
            content: "";
            position: absolute;
            width: 110px;
            height: 110px;
            right: -55px;
            bottom: -55px;
            border-radius: 50%;
            background: var(--green-soft);
        }

        .card-icon {
            width: 56px;
            height: 56px;
            display: grid;
            place-items: center;
            background: var(--green-soft);
            color: var(--green-hover);
            border-radius: 15px;
            font-size: 1.35rem;
            font-weight: 900;
            margin-bottom: 16px;
        }

        .card h3 {
            color: var(--dark-green);
            font-size: 1.4rem;
            margin-bottom: 15px;
        }

        .skill-list,
        .hobby-list {
            padding-left: 22px;
            position: relative;
            z-index: 1;
        }

        .skill-list li,
        .hobby-list li {
            padding: 7px 0;
        }

        /* =========================
           IMAGE
           ========================= */

        .media-card {
            background: var(--white);
            padding: 20px;
            border: 1px solid var(--border);
            border-radius: 20px;
            box-shadow: var(--shadow);
        }

        .photo {
            display: block;
            width: 100%;
            max-width: 850px;
            height: auto;
            margin: auto;
            border-radius: 16px;
            border: 3px solid var(--yellow);
        }

        figcaption {
            text-align: center;
            color: var(--muted);
            margin-top: 12px;
            font-size: 0.92rem;
        }

        /* =========================
           WEBSITE TABLE
           ========================= */

        .table-box {
            overflow-x: auto;
            background: var(--white);
            border-radius: 20px;
            border: 1px solid var(--border);
            box-shadow: var(--shadow);
        }

        table {
            width: 100%;
            min-width: 680px;
            border-collapse: collapse;
        }

        th {
            background: var(--green-hover);
            color: var(--white);
            text-align: left;
            padding: 16px;
        }

        td {
            padding: 16px;
            border-bottom: 1px solid var(--border);
        }

        tbody tr {
            transition: 0.2s ease;
        }

        tbody tr:hover td {
            background: var(--yellow-soft);
        }

        tbody tr:last-child td {
            border-bottom: none;
        }

        /* =========================
           FORM
           ========================= */

        .form-card {
            max-width: 600px;
            background: var(--white);
            padding: 32px;
            border-radius: 20px;
            border: 1px solid var(--border);
            box-shadow: var(--shadow);
        }

        label {
            display: block;
            margin-bottom: 7px;
            font-weight: bold;
        }

        input,
        select {
            width: 100%;
            padding: 13px;
            margin-bottom: 18px;
            border-radius: 10px;
            border: 1px solid #bdcbc4;
            outline: none;
            font-size: 1rem;
            background: var(--white);
            color: var(--text);
        }

        input:focus,
        select:focus {
            border-color: var(--green);
            box-shadow: 0 0 0 3px rgba(37, 128, 95, 0.12);
        }

        button {
            background: var(--green);
            color: white;
            border: none;
            padding: 13px 22px;
            border-radius: 10px;
            font-weight: bold;
            cursor: pointer;
            transition: 0.25s ease;
        }

        button:hover {
            background: var(--yellow-dark);
            color: var(--dark-green);
            transform: translateY(-3px);
            box-shadow: var(--shadow);
        }

        /* =========================
           YOUTUBE VIDEO
           ========================= */

        .video-card {
            background: var(--white);
            padding: 20px;
            border-radius: 20px;
            border: 1px solid var(--border);
            box-shadow: var(--shadow);
        }

        .video-wrapper {
            position: relative;
            width: 100%;
            aspect-ratio: 16 / 9;
            overflow: hidden;
            border-radius: 16px;
            background: #111111;
            border: 3px solid var(--yellow);
        }

        .video-wrapper iframe {
            width: 100%;
            height: 100%;
            display: block;
            border: 0;
        }

        /* =========================
           FOOTER
           ========================= */

        footer {
            background:
                radial-gradient(
                    circle at 92% 10%,
                    rgba(242, 201, 76, 0.13),
                    transparent 25%
                ),
                var(--dark-green);
            color: #dce8e3;
            padding: 60px 0;
            border-top: 5px solid var(--yellow);
        }

        footer h2 {
            color: white;
        }

        footer a {
            color: var(--yellow);
        }

        footer a:hover {
            color: white;
        }

        address {
            font-style: normal;
            color: #b9cbc4;
        }

        /* =========================
           RESPONSIVE
           ========================= */

        @media (max-width: 800px) {
            section {
                padding: 60px 0;
            }

            .nav-container {
                flex-direction: column;
                align-items: flex-start;
                padding: 14px 0;
            }

            .nav-links {
                width: 100%;
                flex-wrap: wrap;
            }

            .about-grid,
            .cards {
                grid-template-columns: 1fr;
            }

            .hero {
                min-height: auto;
                padding: 90px 0;
            }
        }

        @media (max-width: 500px) {
            .container {
                width: min(100% - 20px, 1100px);
            }

            .nav-links {
                display: grid;
                grid-template-columns: repeat(2, 1fr);
                width: 100%;
            }

            .nav-links a {
                text-align: center;
            }

            .hero h1 {
                font-size: 2.5rem;
            }

            .hero-buttons {
                flex-direction: column;
            }

            .btn {
                width: 100%;
                text-align: center;
            }

            .about-card,
            .card,
            .media-card,
            .form-card,
            .video-card {
                padding: 20px;
            }

            .video-wrapper {
                aspect-ratio: 9 / 16;
            }
        }
    </style>
</head>

<body>

    <!-- TASK 3: Navigation -->
    <nav>
        <div class="container nav-container">

            <a class="logo" href="#home">
                Glenn John M. Padroncillo<span>.</span>
            </a>

            <div class="nav-links">
                <a href="#about">About</a>
                <a href="#skills">Skills</a>
                <a href="#work">Work</a>
                <a href="#contact">Contact</a>
            </div>

        </div>
    </nav>


    <!-- TASK 1: Basic Webpage Structure -->
    <section class="hero" id="home">

        <div class="container">

            <div class="hero-content">

                <span class="badge">
                    BSIT · 2B · Student Portfolio
                </span>

                <h1>
                    Hello, I'm
                    <span>Glenn John</span>.
                </h1>

                <p class="hero-text">
                    My name is Glenn John M. Padroncillo, a second-year
                    Bachelor of Science in Information Technology student
                    from section 2B. I enjoy learning about technology,
                    developing my skills, and creating useful projects.
                </p>

                <div class="hero-buttons">

                    <a href="#skills" class="btn btn-primary">
                        Explore My Skills
                    </a>

                    <a href="#contact" class="btn btn-secondary">
                        Contact Me
                    </a>

                </div>

            </div>

        </div>

    </section>


    <!-- TASK 2: About -->
    <section id="about">

        <div class="container">

            <h2>About Me</h2>

            <p class="section-intro">
                A little information about me as an IT student and
                what I want to achieve.
            </p>

            <div class="about-grid">

                <div class="about-card">

                    <h3>Who I Am</h3>

                    <p>
                        I am <strong>Glenn John M. Padroncillo</strong>,
                        currently studying Bachelor of Science in
                        Information Technology, second year, section 2B.
                    </p>

                    <p>
                        I am interested in computers, technology,
                        programming, and web development.
                    </p>

                </div>

                <div class="about-card">

                    <h3>My Goal</h3>

                    <p>
                        My goal is to continuously improve my skills
                        and gain more knowledge in information technology.
                    </p>

                    <p>
                        I want to become more confident in creating
                        websites and solving programming problems.
                    </p>

                </div>

            </div>

        </div>

    </section>


    <!-- TASK 4: Skills and Hobbies -->
    <section id="skills">

        <div class="container">

            <h2>Skills & Hobbies</h2>

            <p class="section-intro">
                These are some of the skills I use in school and
                some activities I enjoy during my free time.
            </p>

            <div class="cards">

                <div class="card">

                    <div class="card-icon">
                        S
                    </div>

                    <h3>My Skills</h3>

                    <ul class="skill-list">
                        <li>Communication</li>
                        <li>Teamwork</li>
                        <li>Time Management</li>
                    </ul>

                </div>


                <div class="card">

                    <div class="card-icon">
                        H
                    </div>

                    <h3>My Hobbies</h3>

                    <ol class="hobby-list">
                        <li>Dancing</li>
                        <li>Singing</li>
                        <li>Playing Games</li>
                    </ol>

                </div>

            </div>

        </div>

    </section>


    <!-- TASK 5: Image -->
    <section>

        <div class="container">

            <h2>My Favorite Picture</h2>

            <p class="section-intro">
                A memorable gathering with friends.
            </p>

            <div class="media-card">

                <figure>

                    <img
                        class="photo"
                        src="./favorite-picture.jpeg"
                        alt="A group of friends spending time together at a gathering"
                    >

                    <figcaption>
                        A memorable gathering with friends.
                    </figcaption>

                </figure>

            </div>

        </div>

    </section>


    <!-- TASK 6: Favorite Websites -->
    <section id="work">

        <div class="container">

            <h2>Websites I Use</h2>

            <p class="section-intro">
                These are two websites that I frequently use
                for communication and social interaction.
            </p>

            <div class="table-box">

                <table>

                    <thead>
                        <tr>
                            <th>Name</th>
                            <th>URL</th>
                            <th>Description</th>
                        </tr>
                    </thead>

                    <tbody>

                        <tr>
                            <td>Facebook</td>

                            <td>
                                <a
                                    href="https://www.facebook.com"
                                    target="_blank"
                                    rel="noopener"
                                >
                                    facebook.com
                                </a>
                            </td>

                            <td>
                                A social media platform for connecting
                                with friends and sharing content.
                            </td>
                        </tr>

                        <tr>
                            <td>Messenger</td>

                            <td>
                                <a
                                    href="https://www.messenger.com"
                                    target="_blank"
                                    rel="noopener"
                                >
                                    messenger.com
                                </a>
                            </td>

                            <td>
                                A messaging platform for communicating
                                with friends and family.
                            </td>
                        </tr>

                    </tbody>

                </table>

            </div>

        </div>

    </section>


    <!-- TASK 7: Simple Form -->
    <section>

        <div class="container">

            <h2>Send Me a Message</h2>

            <p class="section-intro">
                Fill out the form below to send a simple message.
            </p>

            <form
                class="form-card"
                onsubmit="showFormMessage(event)"
            >

                <label for="name">
                    Name
                </label>

                <input
                    type="text"
                    id="name"
                    name="name"
                    placeholder="Enter your name"
                    required
                >

                <label for="email">
                    Email
                </label>

                <input
                    type="email"
                    id="email"
                    name="email"
                    placeholder="Enter your email"
                    required
                >

                <label for="color">
                    Favorite Color
                </label>

                <select
                    id="color"
                    name="color"
                    required
                >
                    <option value="">
                        Choose a color
                    </option>

                    <option value="red">
                        Red
                    </option>

                    <option value="blue">
                        Blue
                    </option>

                    <option value="green">
                        Green
                    </option>

                    <option value="yellow">
                        Yellow
                    </option>
                </select>

                <button type="submit">
                    Send Message
                </button>

            </form>

        </div>

    </section>


    <!-- TASK 8: YouTube Video -->
    <section>

        <div class="container">

            <h2>Something Worth Watching</h2>

            <p class="section-intro">
                A featured video from my YouTube channel.
            </p>

            <div class="video-card">

                <div class="video-wrapper">

                    <iframe
                        src="https://www.youtube.com/embed/DsRBJAzsGUs"
                        title="My Featured YouTube Video"
                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                        allowfullscreen>
                    </iframe>

                </div>

            </div>

        </div>

    </section>


    <!-- TASK 10: Footer -->
    <footer id="contact">

        <div class="container">

            <h2>Get in Touch</h2>

            <p>
                I would be happy to connect with you.
            </p>

            <p>
                Email:
                <a href="mailto:crushsy48@gmail.com">
                    crushsy48@gmail.com
                </a>
            </p>

            <address>
                Centro Poblacion, Culasi, Antique<br>
                Phone: 09302025708
            </address>

            <p>
                <a
                    href="https://www.linkedin.com/"
                    target="_blank"
                    rel="noopener"
                >
                    My LinkedIn Profile
                </a>
            </p>

        </div>

    </footer>


    <!-- JAVASCRIPT -->
    <script>
        function showFormMessage(event) {
            event.preventDefault();

            const name = document.getElementById("name").value;

            alert(
                "Thank you, " + name +
                "! Your message has been received."
            );
        }
    </script>

</body>
</html>
