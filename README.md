<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aditya Singh - GitHub Profile</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: #fff;
            line-height: 1.6;
            padding: 20px;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 40px;
            box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.37);
        }

        header {
            text-align: center;
            padding: 40px 0;
            border-bottom: 2px solid rgba(255, 255, 255, 0.2);
            margin-bottom: 40px;
        }

        h1 {
            font-size: 3em;
            margin-bottom: 10px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
        }

        .tagline {
            font-size: 1.3em;
            margin-bottom: 20px;
            opacity: 0.9;
        }

        .contact-links {
            display: flex;
            gap: 15px;
            justify-content: center;
            flex-wrap: wrap;
            margin-top: 20px;
        }

        .contact-links a {
            background: rgba(255, 255, 255, 0.2);
            padding: 10px 25px;
            border-radius: 25px;
            text-decoration: none;
            color: #fff;
            transition: all 0.3s ease;
            border: 2px solid rgba(255, 255, 255, 0.3);
        }

        .contact-links a:hover {
            background: rgba(255, 255, 255, 0.3);
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
        }

        section {
            margin-bottom: 50px;
        }

        h2 {
            font-size: 2.5em;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            gap: 15px;
        }

        h2::before {
            content: '';
            width: 50px;
            height: 4px;
            background: #fff;
            border-radius: 2px;
        }

        h3 {
            font-size: 1.8em;
            margin: 25px 0 15px 0;
            color: #ffd700;
        }

        .about-text {
            font-size: 1.1em;
            line-height: 1.8;
            background: rgba(255, 255, 255, 0.1);
            padding: 25px;
            border-radius: 15px;
            border-left: 4px solid #ffd700;
        }

        .job {
            background: rgba(255, 255, 255, 0.1);
            padding: 25px;
            border-radius: 15px;
            margin-bottom: 25px;
            border-left: 4px solid #4ade80;
        }

        .job-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 15px;
            flex-wrap: wrap;
            gap: 10px;
        }

        .job-title {
            font-size: 1.4em;
            color: #4ade80;
        }

        .duration {
            background: rgba(255, 255, 255, 0.2);
            padding: 5px 15px;
            border-radius: 15px;
            font-size: 0.9em;
        }

        .project-name {
            font-weight: bold;
            margin-top: 15px;
            margin-bottom: 10px;
            color: #60a5fa;
        }

        ul {
            list-style: none;
            padding-left: 0;
        }

        ul li {
            padding: 8px 0 8px 30px;
            position: relative;
        }

        ul li::before {
            content: '▹';
            position: absolute;
            left: 0;
            color: #ffd700;
            font-size: 1.5em;
        }

        .tech-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin-top: 25px;
        }

        .tech-category {
            background: rgba(255, 255, 255, 0.1);
            padding: 20px;
            border-radius: 15px;
            border-top: 3px solid #60a5fa;
        }

        .tech-category h4 {
            color: #60a5fa;
            margin-bottom: 15px;
            font-size: 1.2em;
        }

        .tech-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }

        .tech-tag {
            background: rgba(255, 255, 255, 0.2);
            padding: 8px 15px;
            border-radius: 20px;
            font-size: 0.9em;
            border: 1px solid rgba(255, 255, 255, 0.3);
        }

        .project-card {
            background: rgba(255, 255, 255, 0.1);
            padding: 30px;
            border-radius: 15px;
            border-left: 4px solid #a78bfa;
            margin-bottom: 20px;
        }

        .project-card h3 {
            color: #a78bfa;
            margin-top: 0;
        }

        .project-subtitle {
            font-style: italic;
            opacity: 0.8;
            margin-bottom: 15px;
        }

        .achievements-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
            margin-top: 25px;
        }

        .achievement-card {
            background: rgba(255, 255, 255, 0.1);
            padding: 20px;
            border-radius: 15px;
            text-align: center;
            border: 2px solid #ffd700;
        }

        .achievement-icon {
            font-size: 2.5em;
            margin-bottom: 10px;
        }

        .education-card {
            background: rgba(255, 255, 255, 0.1);
            padding: 25px;
            border-radius: 15px;
            border-left: 4px solid #f472b6;
        }

        .education-card h3 {
            color: #f472b6;
            margin-top: 0;
        }

        footer {
            text-align: center;
            padding: 40px 0 20px 0;
            border-top: 2px solid rgba(255, 255, 255, 0.2);
            margin-top: 50px;
        }

        .quote {
            font-size: 1.3em;
            font-style: italic;
            margin-bottom: 20px;
            opacity: 0.9;
        }

        @media (max-width: 768px) {
            .container {
                padding: 20px;
            }

            h1 {
                font-size: 2em;
            }

            h2 {
                font-size: 1.8em;
            }

            .tech-grid {
                grid-template-columns: 1fr;
            }

            .job-header {
                flex-direction: column;
                align-items: flex-start;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>👋 Hi, I'm Aditya Singh</h1>
            <p class="tagline">Full-Stack AI Engineer | Community Builder | Open Source Enthusiast</p>
            <div class="contact-links">
                <a href="YOUR_LINKEDIN_URL">LinkedIn</a>
                <a href="YOUR_MEDIUM_URL">Medium</a>
                <a href="mailto:adityasinghwork11@gmail.com">Email</a>
                <a href="tel:+919315920610">Phone</a>
            </div>
        </header>

        <section id="about">
            <h2>🚀 About Me</h2>
            <div class="about-text">
                <p>I am a <strong>Full-Stack AI Engineer</strong> passionate about building intelligent, scalable, and user-focused applications by combining AI/ML, LLMs, and automation with modern full-stack technologies like Python, JavaScript/TypeScript. Skilled in deep learning, NLP, vector databases, and semantic search, I enjoy exploring how AI can transform workflows, make accurate predictions, and solve complex real-world problems. With strong experience in databases, cloud deployment, and CI/CD pipelines.</p>
                <p style="margin-top: 15px;">As a side quest, I founded <strong>Geek Room</strong>, a <strong>1,00,000+ developer community</strong> that connects students across India through hackathons, workshops, and bootcamps, fostering growth and collaboration. Driven by curiosity and creativity, I thrive on learning, experimenting, and bringing impactful ideas to life at the intersection of AI innovation, product development, and community building ✨</p>
            </div>
        </section>

        <section id="experience">
            <h2>💼 Professional Experience</h2>
            
            <div class="job">
                <div class="job-header">
                    <span class="job-title">🔹 Software Engineer @ Bynd AI</span>
                    <span class="duration">May 2024 – Present</span>
                </div>
                <div class="project-name">Project Discovery – AI Powered Financial Data Extraction System</div>
                <ul>
                    <li>Built production-ready system extracting structured/unstructured financial data from company filings and reports</li>
                    <li>Optimized document processing pipeline with BullMQ & Redis, reducing chunking time from 5 minutes to under 60 seconds</li>
                    <li>Integrated Azure Document Intelligence for intelligent OCR and layout-aware parsing</li>
                </ul>
                <div class="project-name">Project Intelligence – AI Driven News Aggregation</div>
                <ul>
                    <li>Developed real-time news aggregation platform monitoring financial publications using web scraping</li>
                    <li>Designed intelligent recommendation engine using NLP-based topic modeling and entity recognition</li>
                    <li>Automated newsletter generation with Next.js & FastAPI for enterprise users</li>
                </ul>
            </div>

            <div class="job">
                <div class="job-header">
                    <span class="job-title">🔹 Software Engineer Intern @ IcuPad India Pvt. Ltd.</span>
                    <span class="duration">Nov 2024 – Jan 2025</span>
                </div>
                <ul>
                    <li>Built AI-powered legal tech document management features with Transformers</li>
                    <li>Implemented auto-fill workflows using LLMs, reducing manual data entry by 90%</li>
                    <li>Developed backend automation with FastAPI & PostgreSQL</li>
                    <li>Integrated embedding-based semantic search and ML-driven validation via REST APIs</li>
                </ul>
            </div>

            <div class="job">
                <div class="job-header">
                    <span class="job-title">🔹 Software Engineer Intern @ Figr</span>
                    <span class="duration">Oct 2024 – Dec 2024</span>
                </div>
                <ul>
                    <li>Built AI-driven design automation system generating Figma screens from text prompts</li>
                    <li>Integrated AI models with prompt engineering for dynamic UI component generation</li>
                    <li>Developed asynchronous backend pipelines with FastAPI & PostgreSQL</li>
                </ul>
            </div>
        </section>

        <section id="tech-stack">
            <h2>🛠️ Technical Stack</h2>
            <div class="tech-grid">
                <div class="tech-category">
                    <h4>Languages & Frameworks</h4>
                    <div class="tech-tags">
                        <span class="tech-tag">Python</span>
                        <span class="tech-tag">TypeScript</span>
                        <span class="tech-tag">JavaScript</span>
                        <span class="tech-tag">C/C++</span>
                        <span class="tech-tag">React</span>
                        <span class="tech-tag">Next.js</span>
                        <span class="tech-tag">Node.js</span>
                        <span class="tech-tag">NestJS</span>
                        <span class="tech-tag">FastAPI</span>
                        <span class="tech-tag">Express.js</span>
                    </div>
                </div>
                <div class="tech-category">
                    <h4>AI & Machine Learning</h4>
                    <div class="tech-tags">
                        <span class="tech-tag">Generative AI</span>
                        <span class="tech-tag">LLMs</span>
                        <span class="tech-tag">NLP</span>
                        <span class="tech-tag">Transformers</span>
                        <span class="tech-tag">Deep Learning</span>
                        <span class="tech-tag">Semantic Search</span>
                    </div>
                </div>
                <div class="tech-category">
                    <h4>Databases & Cloud</h4>
                    <div class="tech-tags">
                        <span class="tech-tag">PostgreSQL</span>
                        <span class="tech-tag">Redis</span>
                        <span class="tech-tag">Pinecone</span>
                        <span class="tech-tag">Firebase</span>
                        <span class="tech-tag">Docker</span>
                        <span class="tech-tag">Kubernetes</span>
                        <span class="tech-tag">Azure</span>
                        <span class="tech-tag">Vercel</span>
                        <span class="tech-tag">GitHub Actions</span>
                    </div>
                </div>
            </div>
        </section>

        <section id="projects">
            <h2>🎯 Featured Projects</h2>
            <div class="project-card">
                <h3>🎥 AI Video Knowledge Extractor</h3>
                <p class="project-subtitle">AI-Powered Video Analysis System</p>
                <ul>
                    <li>Built monolithic NestJS system converting videos into searchable knowledge bases</li>
                    <li>Automated transcription with Whisper AI and semantic chunking with Pinecone</li>
                    <li>Engineered multi-stage background pipeline using BullMQ & Redis</li>
                    <li>Integrated Azure Blob Storage, PostgreSQL & OpenAI APIs for unified orchestration</li>
                </ul>
                <div class="tech-tags" style="margin-top: 15px;">
                    <span class="tech-tag">NestJS</span>
                    <span class="tech-tag">Whisper AI</span>
                    <span class="tech-tag">Pinecone</span>
                    <span class="tech-tag">BullMQ</span>
                    <span class="tech-tag">Redis</span>
                    <span class="tech-tag">Azure</span>
                    <span class="tech-tag">PostgreSQL</span>
                    <span class="tech-tag">OpenAI</span>
                </div>
            </div>
        </section>

        <section id="achievements">
            <h2>🏆 Achievements</h2>
            <div class="achievements-grid">
                <div class="achievement-card">
                    <div class="achievement-icon">🥇</div>
                    <p><strong>Winner</strong><br>HackNSUT'23, HackAvenue</p>
                </div>
                <div class="achievement-card">
                    <div class="achievement-icon">🏅</div>
                    <p><strong>Finalist</strong><br>Hustle X (IIM Lucknow)</p>
                </div>
                <div class="achievement-card">
                    <div class="achievement-icon">🏅</div>
                    <p><strong>Finalist</strong><br>Vihaan 6.0 (DTU)</p>
                </div>
                <div class="achievement-card">
                    <div class="achievement-icon">🎪</div>
                    <p><strong>15+ Hackathons</strong><br>Organized</p>
                </div>
                <div class="achievement-card">
                    <div class="achievement-icon">👨‍🏫</div>
                    <p><strong>25+ Teams</strong><br>Mentored</p>
                </div>
                <div class="achievement-card">
                    <div class="achievement-icon">🚀</div>
                    <p><strong>20+ Hackathons</strong><br>Participated</p>
                </div>
            </div>
        </section>

        <section id="education">
            <h2>🎓 Education</h2>
            <div class="education-card">
                <h3>BTech in Computer Science</h3>
                <p><strong>Guru Gobind Singh Indraprastha University (GGSIPU)</strong></p>
                <p>Delhi, India</p>
                <p style="margin-top: 10px;"><em>Nov 2022 – 2026</em></p>
            </div>
        </section>

        <footer>
            <h2>🤝 Let's Connect!</h2>
            <p style="margin-bottom: 25px;">I'm always excited to collaborate on innovative AI projects, discuss tech trends, or connect with fellow developers!</p>
            <div class="contact-links">
                <a href="YOUR_LINKEDIN_URL">LinkedIn - Let's Connect</a>
                <a href="YOUR_MEDIUM_URL">Medium - Follow Me</a>
                <a href="mailto:adityasinghwork11@gmail.com">Email - Drop a Message</a>
            </div>
            <p class="quote" style="margin-top: 40px;">"Building the future, one line of code at a time"</p>
        </footer>
    </div>
</body>
</html>
