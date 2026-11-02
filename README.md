<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">



<title>Nassaie Udris | Floral Portfolio</title>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Segoe UI', Arial, sans-serif;
    scroll-behavior: smooth;
}

body {
    background: #f8f3ff;
    color: #49375f;
    line-height: 1.7;
    overflow-x: hidden;
}

/* FLOWER DECORATIONS */
.flower {
    position: fixed;
    z-index: -1;
    opacity: 0.45;
    pointer-events: none;
    animation: floatFlower 6s ease-in-out infinite;
}

.flower-one {
    top: 100px;
    left: 12px;
    font-size: 35px;
}

.flower-two {
    top: 280px;
    right: 12px;
    font-size: 30px;
    animation-delay: 2s;
}

.flower-three {
    bottom: 120px;
    left: 20px;
    font-size: 32px;
    animation-delay: 1s;
}

.flower-four {
    bottom: 220px;
    right: 15px;
    font-size: 36px;
    animation-delay: 3s;
}

@keyframes floatFlower {
    0%, 100% {
        transform: translateY(0) rotate(0deg);
    }
    50% {
        transform: translateY(-15px) rotate(10deg);
    }
}

/* HEADER */
header {
    position: relative;
    overflow: hidden;
    text-align: center;
    padding: 55px 20px;
    color: white;
    background: #7652a8;
    border-bottom: 6px solid #e8c9f0;
}

.header-flower {
    position: absolute;
    font-size: 48px;
    opacity: 0.85;
}

.left-flower {
    top: 15px;
    left: 20px;
}

.right-flower {
    bottom: 12px;
    right: 20px;
}

header h1 {
    font-size: 38px;
    margin-bottom: 8px;
    letter-spacing: 1px;
}

header p {
    font-size: 16px;
}

.header-subtitle {
    color: #f7e8ff;
    margin-top: 5px;
}

/* NAVIGATION */
nav {
    background: #eadfff;
    padding: 14px 8px;
    text-align: center;
    position: sticky;
    top: 0;
    z-index: 100;
    box-shadow: 0 3px 10px #7652a822;
}

nav a {
    display: inline-block;
    color: #63438d;
    text-decoration: none;
    margin: 5px 9px;
    font-size: 14px;
    font-weight: bold;
    transition: 0.3s;
}

nav a:hover {
    color: #d45f9b;
    transform: translateY(-2px);
}

/* MAIN CONTENT */
.container {
    width: 90%;
    max-width: 1000px;
    margin: 35px auto;
}

/* SECTIONS */
section {
    position: relative;
    background: #ffffff;
    padding: 30px;
    margin-bottom: 28px;
    border-radius: 20px;
    border: 1px solid #eadfff;
    border-left: 6px solid #a98bd6;
    box-shadow: 0 6px 20px #7652a812;
    overflow: hidden;
}

section::after {
    content: "✿";
    position: absolute;
    top: 5px;
    right: 15px;
    font-size: 28px;
    color: #e7c3e9;
    opacity: 0.8;
    pointer-events: none;
}

section h2 {
    color: #7652a8;
    font-size: 25px;
    margin-bottom: 18px;
    padding-bottom: 10px;
    border-bottom: 2px solid #e6d9fa;
}

section h3 {
    color: #7652a8;
    margin-bottom: 8px;
}

/* HOME */
.profile {
    text-align: center;
    background: #fffaff;
    border-left-color: #c7a6eb;
}

.profile .welcome {
    color: #d16b9f;
    font-size: 16px;
    font-weight: bold;
    letter-spacing: 2px;
}

.profile img {
    display: block;
    width: 175px;
    height: 175px;
    object-fit: cover;
    border-radius: 50%;
    border: 6px solid #d8c3fa;
    outline: 4px solid #e7f6ff;
    margin: 22px auto;
    background: #f1e7ff;
    box-shadow: 0 5px 20px #7652a833;
}

.profile h2 {
    border-bottom: none;
    margin-bottom: 5px;
}

.profile h3 {
    font-size: 23px;
}

.profile p {
    margin: 10px 0;
}

.profile input {
    display: block;
    max-width: 100%;
    margin: 15px auto;
    padding: 10px;
    background: #f0e8fc;
    border-radius: 10px;
}

.upload-label {
    color: #7652a8;
    font-weight: bold;
}

/* ABOUT ME */
#about {
    border-left-color: #b5a0e5;
}

#about p {
    margin-bottom: 12px;
}

/* PERSONAL INFORMATION */
#information {
    border-left-color: #e8a9cb;
}

.info p {
    padding: 10px 14px;
    margin: 10px 0;
    background: #fff3f9;
    border-radius: 10px;
    border-left: 3px solid #e8a9cb;
    overflow-wrap: anywhere;
}

/* SKILLS, HOBBIES, PROJECTS */
.skills-list,
.hobbies-list,
.projects-list {
    display: flex;
    flex-wrap: wrap;
    gap: 16px;
    margin-top: 18px;
}

.skill,
.hobby,
.project {
    flex: 1 1 200px;
    padding: 22px 17px;
    border-radius: 16px;
    text-align: center;
    transition: transform 0.3s, box-shadow 0.3s;
    border: 1px solid #e3d4f5;
    background: #f3edff;
}

.skill:nth-child(even),
.project:nth-child(even) {
    background: #eaf7ff;
    border-color: #c8e7f7;
}

.hobby:nth-child(2) {
    background: #fff0f7;
    border-color: #f4d1e3;
}

.hobby:nth-child(3) {
    background: #eaf7ff;
    border-color: #c8e7f7;
}

.skill:hover,
.hobby:hover,
.project:hover {
    transform: translateY(-5px);
    box-shadow: 0 8px 18px #7652a822;
}

.card-flower {
    display: block;
    font-size: 30px;
    margin-bottom: 8px;
}

/* CONTACT */
#contact {
    border-left-color: #e8a9cb;
    background: #fffaff;
}

#contact p {
    margin: 13px 0;
}

#contact a:not(.button) {
    color: #7652a8;
    font-weight: bold;
    text-decoration: none;
    overflow-wrap: anywhere;
}

#contact a:not(.button):hover {
    color: #d45f9b;
}

/* BUTTON */
.button {
    display: inline-block;
    background: #7652a8;
    color: white !important;
    text-decoration: none;
    padding: 12px 23px;
    border-radius: 30px;
    margin-top: 12px;
    font-weight: bold;
    transition: 0.3s;
    box-shadow: 0 4px 10px #7652a833;
}

.button:hover {
    background: #d16b9f;
    transform: translateY(-2px);
}

/* FOOTER */
footer {
    position: relative;
    background: #7652a8;
    color: white;
    text-align: center;
    padding: 30px 15px;
    margin-top: 40px;
}

footer .footer-flower {
    font-size: 25px;
    margin-bottom: 5px;
}

footer p {
    margin: 4px 0;
}

/* BACK TO TOP */
.back-top {
    display: inline-block;
    margin-top: 12px;
    padding: 7px 16px;
    color: #7652a8;
    background: white;
    text-decoration: none;
    border-radius: 20px;
    font-weight: bold;
}

/* MOBILE DESIGN */
@media (max-width: 600px) {
    header {
        padding: 45px 15px;
    }

    header h1 {
        font-size: 29px;
    }

    .header-flower {
        font-size: 30px;
    }

    .container {
        width: 93%;
        margin: 22px auto;
    }

    section {
        padding: 22px 17px;
    }

    section h2 {
        font-size: 22px;
    }

    nav a {
        font-size: 12px;
        margin: 4px 6px;
    }

    .profile img {
        width: 150px;
        height: 150px;
    }

    .skill,
    .hobby,
    .project {
        flex: 1 1 100%;
    }

    .flower-one,
    .flower-two,
    .flower-three,
    .flower-four {
        font-size: 24px;
    }
}
</style>
</head>

<body>

<!-- DECORATIVE FLOWERS -->
<div class="flower flower-one">🌸</div>
<div class="flower flower-two">🌷</div>
<div class="flower flower-three">🦋</div>
<div class="flower flower-four">🌺</div>

<!-- HEADER -->
<header id="top">
    <span class="header-flower left-flower">🌸</span>
    <span class="header-flower right-flower">🌷</span>

    <h1>✿ Nassaie Udris ✿</h1>
    <p>Welcome to My Personal Portfolio</p>
    <p class="header-subtitle">BSIT Student | Future IT Professional</p>
</header>

<!-- NAVIGATION -->
<nav>
    <a href="#home">Home</a>
    <a href="#about">About Me</a>
    <a href="#information">Information</a>
    <a href="#skills">Skills</a>
    <a href="#hobbies">What I Love</a>
    <a href="#projects">Projects</a>
    <a href="#contact">Contact</a>
</nav>

<main class="container">

    <!-- HOME -->
    <section id="home" class="profile">
        <p class="welcome">🌷 WELCOME TO MY LITTLE WORLD 🌷</p>

        <img
            id="profilePhoto"
            src="https://placehold.co/175x175/e8d9ff/7652a8?text=My+Photo"
            alt="Nassaie Udris Profile Photo"
        >

        <h2>♡ Hello, I'm Nassaie Udris! ♡</h2>

        <p>
            Welcome to my personal website! Here you can learn about
            my background, skills, hobbies, and projects.
        </p>

        <label class="upload-label" for="photoInput">
            🌸 Choose Your Profile Picture
        </label>

        <input
            type="file"
            id="photoInput"
            accept="image/*"
            onchange="changePhoto(event)"
        >

        <p><small>Choose a photo from your device.</small></p>
    </section>

    <!-- ABOUT ME -->
    <section id="about">
        <h2>🌸 About Me</h2>

        <p>
            My name is Nassaie Udris. I am a first-year college student
            at Mindanao State University, taking Bachelor of Science
            in Information Technology (BSIT).
        </p>

        <p>
            I am interested in computers, programming, and web design.
            I enjoy learning new things and improving my knowledge
            about technology.
        </p>

        <p>
            My dream is to become a skilled IT professional in the
            future and create useful projects using my knowledge.
        </p>
    </section>

    <!-- PERSONAL INFORMATION -->
    <section id="information">
        <h2>💜 Personal Information</h2>

        <div class="info">
            <p><strong>Name:</strong> Nassaie Udris</p>

            <p>
                <strong>University:</strong>
                Mindanao State University
            </p>

            <p><strong>Year Level:</strong> First-Year College</p>

            <p>
                <strong>Course:</strong>
                Bachelor of Science in Information Technology (BSIT)
            </p>

            <p><strong>Address:</strong> Tayungan, Panamao, Sulu</p>
        </div>
    </section>

    <!-- SKILLS -->
    <section id="skills">
        <h2>🦋 My Skills</h2>

        <div class="skills-list">

            <div class="skill">
                <span class="card-flower">💻</span>
                <h3>HTML</h3>
                <p>Creating the structure of web pages.</p>
            </div>

            <div class="skill">
                <span class="card-flower">🎨</span>
                <h3>CSS</h3>
                <p>Designing websites with beautiful colors and layouts.</p>
            </div>

            <div class="skill">
                <span class="card-flower">✨</span>
                <h3>JavaScript</h3>
                <p>Learning basic website interactions.</p>
            </div>

            <div class="skill">
                <span class="card-flower">⌨️</span>
                <h3>C++ Programming</h3>
                <p>Practicing basic programming concepts.</p>
            </div>

            <div class="skill">
                <span class="card-flower">🤝</span>
                <h3>Teamwork</h3>
                <p>Working and learning with other people.</p>
            </div>

        </div>
    </section>

    <!-- WHAT I LOVE -->
    <section id="hobbies">
        <h2>🌷 What I Love</h2>

        <div class="hobbies-list">

            <div class="hobby">
                <span class="card-flower">💃</span>
                <h3>Dancing</h3>
                <p>
                    I enjoy dancing and expressing myself through movement.
                </p>
            </div>

            <div class="hobby">
                <span class="card-flower">📚</span>
                <h3>Reading</h3>
                <p>
                    I love reading and learning new things.
                </p>
            </div>

            <div class="hobby">
                <span class="card-flower">🏐</span>
                <h3>Volleyball</h3>
                <p>
                    I enjoy playing volleyball and being part of a team.
                </p>
            </div>

        </div>
    </section>

    <!-- PROJECTS -->
    <section id="projects">
        <h2>🌸 My Projects</h2>

        <div class="projects-list">

            <div class="project">
                <span class="card-flower">🌷</span>
                <h3>Personal Portfolio</h3>
                <p>
                    A website that introduces my background, skills,
                    and interests.
                </p>
            </div>

            <div class="project">
                <span class="card-flower">🩵</span>
                <h3>Basic HTML Page</h3>
                <p>
                    A simple webpage created using HTML and CSS.
                </p>
            </div>

            <div class="project">
                <span class="card-flower">💜</span>
                <h3>C++ Practice</h3>
                <p>
                    Basic programs created while learning C++.
                </p>
            </div>

        </div>
    </section>

    <!-- CONTACT -->
    <section id="contact">
        <h2>💌 Contact Me</h2>

        <p>
            <strong>Facebook:</strong>
            <a
                href="https://www.facebook.com/profile.php?id=61592464006652"
                target="_blank"
                rel="noopener noreferrer"
            >
                Visit My Facebook Profile
            </a>
        </p>

        <p>
            <strong>Email:</strong>
            Add your email address here
        </p>

        <a
            class="button"
            href="https://www.facebook.com/profile.php?id=61592464006652"
            target="_blank"
            rel="noopener noreferrer"
        >
            💜 Visit My Facebook
        </a>
    </section>

</main>

<!-- FOOTER -->
<footer>
    <div class="footer-flower">🌸 🦋 🌷</div>

    <p><strong>Nassaie Udris</strong></p>
    <p>My Personal Portfolio</p>
    <p>Made with love for learning and creativity.</p>
    <p>&copy; 2026 Nassaie Udris. All rights reserved.</p>

    <a class="back-top" href="#top">↑ Back to Top</a>
</footer>

<!-- PROFILE PHOTO SCRIPT -->
<script>
function changePhoto(event) {
    const file = event.target.files[0];

    if (file && file.type.startsWith("image/")) {
        const imageURL = URL.createObjectURL(file);

        document.getElementById("profilePhoto").src = imageURL;
    }
}
</script>

</body>
</html>
