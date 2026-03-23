<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Derin Ozturk | Cybersecurity Portfolio</title>

<style>
body{
    margin:0;
    font-family:Arial, Helvetica, sans-serif;
    background:#0f172a;
    color:#e2e8f0;
}

header{
    text-align:center;
    padding:60px 20px;
    background:#020617;
}

header h1{
    font-size:40px;
    margin-bottom:10px;
}

header p{
    font-size:18px;
    color:#94a3b8;
}

nav{
    text-align:center;
    background:#020617;
    padding:15px;
}

nav a{
    color:#e2e8f0;
    margin:0 20px;
    text-decoration:none;
    font-weight:bold;
}

nav a:hover{
    color:#38bdf8;
}

section{
    max-width:1000px;
    margin:auto;
    padding:60px 20px;
}

.projects{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
    gap:25px;
}

.project{
    background:#020617;
    border:1px solid #1e293b;
    border-radius:10px;
    padding:25px;
}

.project h3{
    margin-top:0;
}

.project a{
    display:inline-block;
    margin-top:10px;
    color:#38bdf8;
    text-decoration:none;
}

.project a:hover{
    text-decoration:underline;
}

footer{
    text-align:center;
    padding:25px;
    background:#020617;
    color:#94a3b8;
}
</style>
</head>

<body>

<header>
<h1>Derin Ozturk</h1>
<p>Cybersecurity Student</p>
</header>

<nav>
<a href="#about">About</a>
<a href="#projects">Projects</a>
<a href="#contact">Contact</a>
</nav>

<section id="about">
<h2>About Me</h2>
<p>
I am a cybersecurity student interested in penetration testing,
web developement, secure software development, and vulnerability research.
I enjoy participating in security labs, hackathons, and building
projects that improve system security and automation.
</p>
</section>

<section id="projects">
<h2>Projects</h2>

<div class="projects">

<div class="project">
<h3>QZ Management</h3>
<p>
QZ Management is a full-stack security infrastructure tool designed to automate vulnerability detection across corporate networks. The system utilizes a distributed architecture consisting of a Python-based client agent and a centralized management server. The agent monitors local software registries and relays version data to the server, where it is processed using Gemini AI to normalize naming conventions. This data is then cross-referenced with the NIST National Vulnerability Database (NVD) API to provide real-time risk analysis, allowing system administrators to identify and mitigate exploits through a modern React-based dashboard.
</p>
<a href="https://devpost.com/software/qz-management" target="_blank">
View on Devpost
</a>
</div>

<div class="project">
<h3>2026 ISSessions FantasyCTF</h3>
<p>
Created 5 challanges for the ISSessions FantasyCTF (2 Web challanges and 3 Open-source Intelligence Challanges). All of my challanges will be added here once the repository goes public.
</p>

My best web challange: E-Bazaar
<a href="https://github.com/derin242/E-Bazaar-Writeup" target="_blank">
Click here to view my official write-up for E-Bazaar
</a>

</div>

<div class="project">
<h3>Paddington</h3>
<p>
Paddington is a Firefox browser extension that helps users quickly determine whether an online article may be biased before reading it. When the user clicks the analyze button, the extension sends the article URL to a local Python server built with Flask. The server retrieves the webpage content, extracts the text using BeautifulSoup, and sends it to the Perplexity AI API for bias analysis. The result is returned to the extension and displayed to the user, helping them quickly evaluate the reliability and potential bias of news content.

Technologies: Python, Flask, JavaScript, HTML, CSS, BeautifulSoup, APIs, JSON, Perplexity AI.
</p>
<a href="https://devpost.com/software/paddington" target="_blank">
View on Devpost
</a>
</div>

</div>
</section>

<footer>
<p>© 2026 Derin Ozturk | Portfolio</p>
</footer>

</body>
</html>
