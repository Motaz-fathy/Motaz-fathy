<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Motaz Fathy - Portfolio</title>
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/typed.js@2.0.12"></script>
    <style>
        /* Custom Styles */
        .animated-text {
            font-size: 2rem;
            font-weight: 700;
        }
        html {
                scroll-behavior: smooth;
             }
    </style>
</head>
<body class="bg-gray-100 text-gray-800">
    
    <!-- Navbar -->
    <nav class="bg-gray-800 text-white p-4">
        <ul class="flex space-x-6">
            <li><a href="#about">About</a></li>
            <li><a href="#services">Services</a></li>
            <li><a href="#skills">Skills</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>
    
    <!-- About Section -->
    <section id="about" class="py-16 bg-gray-100 text-center">
        <div class="container mx-auto">
            <div class="animated-text" id="name"></div>
            <p class="mt-4 text-lg">
                I am a Front-End Developer with 4 years of experience in building responsive, user-friendly interfaces for websites and applications.
                Skilled in HTML, CSS, JavaScript, React.js/TypeScript, Angular, Vue.js, Tailwind, and Bootstrap, I specialize in optimizing performance
                and delivering seamless user experiences. I hold a degree in Computer and Information Science from Assiut University. My passion lies in
                creating visually engaging and interactive designs that exceed client expectations. I am eager to contribute my skills to dynamic and
                innovative development teams.
            </p>
            <img src="your-image.jpg" alt="Motaz Fathy" class="rounded-full mx-auto w-48 h-48 mt-8">
        </div>
    </section>
    
    <!-- Services Section -->
    <section id="services" class="py-16 bg-white">
        <div class="container mx-auto">
            <h2 class="text-3xl text-center font-semibold mb-8">Services</h2>
            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8">
                <!-- Service 1 -->
                <div class="border p-6 rounded-lg shadow-lg text-center">
                    <img src="react-logo.png" alt="React Logo" class="h-16 mx-auto mb-4">
                    <h3 class="text-xl font-bold">Create Projects React.js/TS</h3>
                    <p class="mt-2 text-gray-600">Build dynamic, responsive web apps using React.js and TypeScript.</p>
                    <p class="mt-4 text-green-600 font-semibold">$10/hour</p>
                </div>
                <!-- Service 2 -->
                <div class="border p-6 rounded-lg shadow-lg text-center">
                    <img src="next-logo.png" alt="Next.js Logo" class="h-16 mx-auto mb-4">
                    <h3 class="text-xl font-bold">Create Projects with Next.js</h3>
                    <p class="mt-2 text-gray-600">Develop server-side rendered web apps with Next.js.</p>
                    <p class="mt-4 text-green-600 font-semibold">$10/hour</p>
                </div>
                <!-- Service 3 -->
                <div class="border p-6 rounded-lg shadow-lg text-center">
                    <img src="angular-logo.png" alt="Angular Logo" class="h-16 mx-auto mb-4">
                    <h3 class="text-xl font-bold">Create Projects with Angular</h3>
                    <p class="mt-2 text-gray-600">Craft enterprise-grade apps using Angular 17.</p>
                    <p class="mt-4 text-green-600 font-semibold">$10/hour</p>
                </div>
                <!-- Service 4 -->
                <div class="border p-6 rounded-lg shadow-lg text-center">
                    <img src="vue-logo.png" alt="Vue.js Logo" class="h-16 mx-auto mb-4">
                    <h3 class="text-xl font-bold">Create Projects with Vue.js</h3>
                    <p class="mt-2 text-gray-600">Build fast, scalable apps with Vue.js.</p>
                    <p class="mt-4 text-green-600 font-semibold">$10/hour</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="py-16 bg-gray-100 text-center">
        <div class="container mx-auto">
            <h2 class="text-3xl font-semibold mb-8">Skills</h2>
            <p class="text-lg">
                React.js/TypeScript, Angular, Vue.js, Next.js, Redux, Redux Toolkit, Vuex, Context API, Formik, Yup, i18n
            </p>
        </div>
    </section>
    
    <!-- Contact Section -->
    <section id="contact" class="py-16 bg-white">
        <div class="container mx-auto">
            <h2 class="text-3xl text-center font-semibold mb-8">Contact Me</h2>
            <p class="text-center">
                Phone: +201021882535 <br>
                WhatsApp: +201021882535 <br>
                Email: <a href="mailto:motazfathy7@gmail.com" class="text-blue-600">motazfathy7@gmail.com</a> <br>
                LinkedIn: <a href="https://www.linkedin.com/in/motaz-fathi-09a17a118/" class="text-blue-600">Motaz Fathy</a> <br>
                GitHub: <a href="https://github.com/Motaz-fathy" class="text-blue-600">Motaz Fathy</a> <br>
                <a href="https://drive.google.com/file/d/1iLKxBtIvd9BOdl5GUSxS-HJ-FGxao3P3/view" class="text-blue-600">Qualification Certificate</a>
            </p>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-800 text-white text-center py-4">
        &copy; 2024 Motaz Fathy. All rights reserved.
    </footer>

    <script>
        // Animated Text
        var typed = new Typed('#name', {
            strings: ["Motaz Fathy"],
            typeSpeed: 100,
            backSpeed: 50,
            loop: true
        });

            // Highlight active navbar link when scrolling
    const sections = document.querySelectorAll('section');
    const navLinks = document.querySelectorAll('nav ul li a');

    window.addEventListener('scroll', () => {
        let currentSection = '';
        
        sections.forEach(section => {
            const sectionTop = section.offsetTop - 100;
            if (window.scrollY >= sectionTop) {
                currentSection = section.getAttribute('id');
            }
        });

        navLinks.forEach(link => {
            link.classList.remove('text-yellow-400'); // Reset color for all links
            if (link.getAttribute('href').includes(currentSection)) {
                link.classList.add('text-yellow-400'); // Highlight the active link
            }
        });
    });
    </script>
</body>
</html>
