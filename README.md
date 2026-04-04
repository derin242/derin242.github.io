<html lang="en">
<head>
    <link href="https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@400;700&display=swap" rel="stylesheet">
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Derin Ozturk | Cybersecurity Portfolio</title>


    <style>

        :root {

            --term-main: #ffffff;      

            --term-glow: #f8fafc;      

            --term-dim: #64748b;       

            --term-bg: #020617;      
            
            --font-main: "JetBrains Mono", "Lucida Console", "Monaco", monospace;
            
            --neon-glow: 0 0 8px rgba(255, 255, 255, 0.4);
    }

    body {
        margin: 0;
        font-family: var(--font-main);
        background: var(--term-bg);
        color: var(--term-main);
        line-height: 1.6;
        letter-spacing: 0.5px; /* Adds that terminal feel */
        overflow-x: hidden;
    }


        body::before {

            content: " ";

            display: block;

            position: fixed;

            top: 0; left: 0; bottom: 0; right: 0;

            background: linear-gradient(

                rgba(18, 16, 16, 0) 50%, 

                rgba(255, 255, 255, 0.02) 50%

            );

            z-index: 9999;

            background-size: 100% 3px;

            pointer-events: none;

        }


        header {

            max-width: 1000px;

            margin: auto;

            padding: 60px 20px;

            border-bottom: 1px solid var(--term-dim);

            text-shadow: var(--neon-glow);

        }


        header h1 {

            font-size: 36px;

            margin: 0;

            letter-spacing: 2px;

            text-transform: uppercase;

        }


        header h1::before { content: "> "; opacity: 0.5; }


        header p {

            font-size: 18px;

            color: var(--term-dim);

            margin-top: 10px;

        }


        nav {

            max-width: 1000px;

            margin: auto;

            padding: 20px;

            display: flex;

            gap: 30px;

        }


        nav a {

            color: var(--term-main);

            text-decoration: none;

            font-size: 14px;

            text-transform: uppercase;

            border: 1px solid transparent;

            padding: 5px 10px;

            transition: 0.3s;

        }


        nav a:hover {

            border: 1px solid var(--term-main);

            box-shadow: var(--neon-glow);

        }


        section {

            max-width: 1000px;

            margin: auto;

            padding: 50px 20px;

        }


        h2 {

            font-size: 20px;

            color: var(--term-dim);

            text-transform: uppercase;

            margin-bottom: 30px;

            letter-spacing: 4px;

        }


        .projects {

            display: grid;

            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));

            gap: 30px;

        }


        .project {

            border: 1px solid #1e293b;

            padding: 30px;

            background: rgba(255, 255, 255, 0.01);

            transition: all 0.3s ease;

        }


        .project:hover {

            border-color: var(--term-main);

            box-shadow: var(--neon-glow);

            transform: translateY(-2px);

        }


        .project h3 {

            margin-top: 0;

            font-size: 18px;

        }


        .project p {

            color: #cbd5e1;

            font-size: 14px;

        }


        .project a {

            color: var(--term-main);

            text-decoration: none;

            font-size: 12px;

            border: 1px solid var(--term-dim);

            padding: 8px 12px;

            display: inline-block;

            margin-top: 20px;

        }


        .project a:hover {

            background: var(--term-main);

            color: var(--term-bg);

            border-color: var(--term-main);

        }


        footer {

            text-align: center;

            padding: 60px;

            color: var(--term-dim);

            font-size: 11px;

            letter-spacing: 2px;

        }


        /* Responsive */

        @media (max-width: 600px) {

            header h1 { font-size: 24px; }

            nav { flex-direction: column; gap: 10px; }

        }

    </style>



</head>

<body>

<header>
    <h1>Derin Ozturk</h1>
    <p>Identity: Cybersecurity Student / Developer</p>
    <p>Status: 2nd Year, expected to graudate in 2028</p>
</header>

<nav>
    <a href="#about">[01] About</a>
    <a href="#projects">[02] Projects</a>
    <a href="#contact">[03] Contact</a>
</nav>

<section id="about">
    <h2>About_Me</h2>
    <p>
        I am a cybersecurity student with an interest in penetration testing (especially web), vulnerability research, and secure software developement. 
        I enjoy participating in security labs, CTFs, hackathons, and building projects that improve system security and automation.
    </p>
</section>

<section id="projects">
    <h2>Filesystem / Projects</h2>

    <div class="projects">
        <div class="project">
            <h3>QZ_Management</h3>
            <p>Full-stack security infrastructure tool. Automates vulnerability detection using Gemini AI normalization and NIST NVD cross-referencing.</p>
            <a href="https://devpost.com/software/qz-management">Execute Link</a>
        </div>

        <div class="project">
            <h3>ISSessions_FantasyCTF</h3>
            <p>Developed 5 security CTF challenges (Web Exploitation & OSINT). Featured project: E-Bazaar.</p>
            <a href="https://github.com/derin242/E-Bazaar-Writeup">Read_Writeup</a>
        </div>

        <div class="project">
            <h3>Paddington_Ext</h3>
            <p>Firefox extension utilizing BeautifulSoup (web scraping) and Perplexity AI for bias analysis of news metadata.</p>
            <a href="https://devpost.com/software/paddington">Execute Link</a>
        </div>
    </div>
</section>

<section id="contact">
    <h2>Comm_Channel</h2>
    <p>> <a href="https://www.linkedin.com/in/derin-ozturk">LinkedIn_Connect</a></p>
</section>

<footer>
    <p>END OF LINE. © 2026 Derin Ozturk</p>
</footer>

<script>
    document.addEventListener('DOMContentLoaded', function() {
        const links = document.querySelectorAll('a');
        links.forEach(link => {
            if (!link.getAttribute('href').startsWith('#')) {
                link.setAttribute('target', '_blank');
                link.setAttribute('rel', 'noopener noreferrer');
            }
        });
    });
</script>

</body>
</html>
