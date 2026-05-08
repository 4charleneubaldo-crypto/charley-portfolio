<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />

    <title>
        Charlene Ubaldo RN | Healthcare AI Strategy & Clinical Innovation
    </title>

    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700;800&family=DM+Sans:wght@400;500;600;700&display=swap" rel="stylesheet">

    <style>

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {

            --primary-blue: #4F7FEA;
            --secondary-blue: #709CF7;

            --light-blue: #EDF4FF;
            --background: #F8FBFF;

            --text-dark: #344054;
            --text-light: #667085;

            --border: #E2E8F0;

            --white: #FFFFFF;
        }

        html {
            scroll-behavior: smooth;
        }

        body {

            font-family: 'DM Sans', sans-serif;

            background: var(--background);

            color: var(--text-dark);

            line-height: 1.8;

            overflow-x: hidden;
        }

        /* NAVBAR */

        nav {

            position: sticky;
            top: 0;

            z-index: 1000;

            display: flex;
            justify-content: space-between;
            align-items: center;

            padding: 1.2rem 3rem;

            background: rgba(255,255,255,0.92);

            backdrop-filter: blur(12px);

            border-bottom: 1px solid var(--border);

            box-shadow: 0 2px 12px rgba(15,23,42,0.04);
        }

        .logo {

            font-family: 'Playfair Display', serif;

            font-size: 1.3rem;

            font-weight: 800;

            color: var(--primary-blue);

            letter-spacing: 0.5px;
        }

        nav ul {

            display: flex;

            gap: 2rem;

            list-style: none;
        }

        nav a {

            text-decoration: none;

            color: var(--text-dark);

            font-weight: 600;

            transition: 0.3s ease;
        }

        nav a:hover {

            color: var(--primary-blue);
        }

        /* HERO */

        .hero {

            background:
            linear-gradient(
                135deg,
                #FFFFFF 0%,
                #F4F8FF 45%,
                #EAF1FF 100%
            );

            padding: 9rem 3rem 7rem;

            position: relative;

            overflow: hidden;

            border-bottom: 1px solid var(--border);
        }

        .hero::before {

            content: '';

            position: absolute;

            top: -150px;
            right: -100px;

            width: 500px;
            height: 500px;

            border-radius: 50%;

            background: rgba(79,127,234,0.06);
        }

        .hero-content {

            max-width: 950px;

            position: relative;

            z-index: 2;
        }

        .hero h1 {

            font-family: 'Playfair Display', serif;

            font-size: 4.3rem;

            line-height: 1.08;

            color: var(--primary-blue);

            margin-bottom: 1.5rem;

            letter-spacing: -1px;
        }

        .subtitle {

            font-size: 1.3rem;

            color: var(--text-light);

            max-width: 760px;

            margin-bottom: 2rem;
        }

        .credentials {

            background: rgba(255,255,255,0.88);

            border: 1px solid var(--border);

            border-radius: 20px;

            padding: 1.7rem 2rem;

            max-width: 760px;

            box-shadow:
                0 4px 14px rgba(15,23,42,0.03),
                0 12px 34px rgba(79,127,234,0.06);

            margin-bottom: 1.5rem;
        }

        .executive-tagline {

            margin-top: 1rem;

            font-size: 0.95rem;

            text-transform: uppercase;

            letter-spacing: 1.2px;

            color: var(--primary-blue);

            font-weight: 700;
        }

        /* BUTTONS */

        .cta-buttons {

            display: flex;

            gap: 1rem;

            flex-wrap: wrap;

            margin-top: 2rem;
        }

        .btn {

            text-decoration: none;

            padding: 1rem 2.4rem;

            border-radius: 14px;

            font-weight: 700;

            transition: all 0.3s ease;
        }

        .btn-primary {

            background: var(--primary-blue);

            color: white;

            box-shadow: 0 10px 24px rgba(79,127,234,0.24);
        }

        .btn-primary:hover {

            transform: translateY(-3px);

            background: var(--secondary-blue);
        }

        .btn-secondary {

            background: white;

            color: var(--primary-blue);

            border: 1px solid var(--border);
        }

        .btn-secondary:hover {

            background: var(--light-blue);

            transform: translateY(-3px);
        }

        /* SECTIONS */

        section {

            padding: 5rem 3rem;
        }

        .container {

            max-width: 1200px;

            margin: auto;
        }

        .light-bg {

            background: #F7FAFF;
        }

        h2 {

            font-family: 'Playfair Display', serif;

            font-size: 2.8rem;

            color: var(--primary-blue);

            margin-bottom: 2rem;
        }

        h3 {

            color: var(--primary-blue);

            margin-bottom: 1rem;
        }

        /* CARDS */

        .foundation-grid,
        .building-grid {

            display: grid;

            grid-template-columns: repeat(auto-fit, minmax(300px,1fr));

            gap: 2rem;

            margin-top: 3rem;
        }

        .foundation-card,
        .solution-card,
        .advantage-item {

            background: rgba(255,255,255,0.96);

            border: 1px solid #E2EAF5;

            border-radius: 18px;

            padding: 2.2rem;

            box-shadow:
                0 4px 12px rgba(15,23,42,0.04),
                0 10px 30px rgba(91,141,239,0.06);

            transition: all 0.3s ease;
        }

        .foundation-card:hover,
        .solution-card:hover,
        .advantage-item:hover {

            transform: translateY(-5px);
        }

        .advantage-list {

            display: grid;

            gap: 1.5rem;

            margin-top: 2rem;
        }

        .solution-card ul {

            margin-top: 1rem;

            padding-left: 1.2rem;
        }

        .solution-card li {

            margin-bottom: 0.8rem;
        }

        .status {

            display: inline-block;

            margin-top: 1.2rem;

            background: var(--light-blue);

            color: var(--primary-blue);

            padding: 0.55rem 1rem;

            border-radius: 999px;

            font-size: 0.85rem;

            font-weight: 700;
        }

        /* VISION */

        .vision-section {

            text-align: center;

            background:
            linear-gradient(
                135deg,
                #F8FBFF 0%,
                #EAF1FF 100%
            );
        }

        .vision-content {

            max-width: 850px;

            margin: auto;
        }

        .vision-content p {

            color: var(--text-light);

            font-size: 1.2rem;
        }

        /* CONTACT */

        .contact-box {

            background:
            linear-gradient(
                135deg,
                #FFFFFF 0%,
                #F4F8FF 100%
            );

            border: 1px solid var(--border);

            border-radius: 24px;

            padding: 3rem;

            box-shadow:
                0 4px 12px rgba(15,23,42,0.04),
                0 10px 30px rgba(91,141,239,0.06);
        }

        .contact-info {

            margin-top: 2rem;
        }

        .contact-info p {

            margin-bottom: 1rem;
        }

        .contact-info a {

            color: var(--primary-blue);

            text-decoration: none;

            font-weight: 700;
        }

        /* FOOTER */

        footer {

            text-align: center;

            padding: 2.5rem;

            background: white;

            border-top: 1px solid var(--border);

            color: var(--text-light);
        }

        /* MOBILE */

        @media (max-width: 768px) {

            nav {

                padding: 1rem 1.2rem;
            }

            nav ul {

                gap: 1rem;
            }

            .hero {

                padding: 5rem 1.5rem;
            }

            .hero h1 {

                font-size: 2.5rem;
            }

            section {

                padding: 3rem 1.5rem;
            }

            .cta-buttons {

                flex-direction: column;
            }

            .btn {

                width: 100%;

                text-align: center;
            }
        }

    </style>
</head>

<body>

    <!-- NAV -->

    <nav>

        <div class="logo">
            CHARLENE UBALDO, RN
        </div>

        <ul>
            <li><a href="#overview">Overview</a></li>
            <li><a href="#foundation">Experience</a></li>
            <li><a href="#building">Solutions</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>

    </nav>

    <!-- HERO -->

    <section class="hero">

        <div class="hero-content">

            <h1>
                Healthcare AI Strategy &
                Clinical Workflow Innovation
            </h1>

            <p class="subtitle">

                Registered Nurse with 20+ years of cross-continuum clinical
                experience focused on AI-powered workflow optimization,
                healthcare operations, and clinician-centered systems innovation.

            </p>

            <div class="credentials">

                <strong>
                    Registered Nurse | Healthcare Systems Thinker
                </strong>

                <br><br>

                Hospital • Clinics • Research • Home Health • Skilled Nursing

                <br>

                CNA to RN | Full Patient Lifecycle Experience

            </div>

            <p class="executive-tagline">

                Clinical Operations • Healthcare AI • Workflow Systems • Care Continuity

            </p>

            <div class="cta-buttons">

                <a href="#contact" class="btn btn-primary">
                    Let's Collaborate
                </a>

                <a href="#building" class="btn btn-secondary">
                    View Solutions
                </a>

            </div>

        </div>

    </section>

    <!-- OVERVIEW -->

    <section id="overview">

        <div class="container">

            <h2>
                Professional Overview
            </h2>

            <p style="font-size:1.08rem; max-width:900px;">

                Healthcare professional with more than 20 years of experience
                spanning acute care, outpatient services, clinical research,
                home health, skilled nursing, and interdisciplinary care coordination.

                Currently focused on integrating AI-driven workflow automation,
                operational efficiency, and systems-level clinical thinking into
                scalable healthcare solutions that improve clinician experience
                and patient outcomes.

            </p>

        </div>

    </section>

    <!-- FOUNDATION -->

    <section id="foundation" class="light-bg">

        <div class="container">

            <h2>
                Clinical Foundation
            </h2>

            <div class="foundation-grid">

                <div class="foundation-card">

                    <h3>
                        Cross-Continuum Experience
                    </h3>

                    <p>

                        Experience across hospitals, clinics,
                        research environments, home health,
                        and skilled nursing facilities.

                    </p>

                </div>

                <div class="foundation-card">

                    <h3>
                        Systems-Level Perspective
                    </h3>

                    <p>

                        Deep understanding of where care coordination,
                        communication, and workflow breakdowns occur
                        across transitions of care.

                    </p>

                </div>

                <div class="foundation-card">

                    <h3>
                        Clinician-Centered Innovation
                    </h3>

                    <p>

                        Focused on practical solutions that improve
                        clinician efficiency while supporting safer,
                        more connected patient care.

                    </p>

                </div>

            </div>

        </div>

    </section>

    <!-- VISION -->

    <section class="vision-section">

        <div class="vision-content">

            <h2>
                Building Clinician-Led Healthcare AI
            </h2>

            <p>

                Real-world healthcare insight combined with emerging
                AI automation capabilities to improve workflow efficiency,
                patient transitions, and operational continuity.

            </p>

        </div>

    </section>

    <!-- SOLUTIONS -->

    <section id="building" class="light-bg">

        <div class="container">

            <h2>
                Solutions & Innovation Areas
            </h2>

            <div class="building-grid">

                <div class="solution-card">

                    <h3>
                        Medication Reconciliation Intelligence
                    </h3>

                    <p>

                        AI-assisted workflow support for reducing
                        medication discrepancies during transitions of care.

                    </p>

                    <ul>

                        <li>Context-aware medication review</li>

                        <li>Transition-of-care safety support</li>

                        <li>Cross-setting workflow continuity</li>

                    </ul>

                    <span class="status">
                        Prototype Development
                    </span>

                </div>

                <div class="solution-card">

                    <h3>
                        Readmission Risk Optimization
                    </h3>

                    <p>

                        Predictive workflow systems focused on
                        identifying high-risk discharge scenarios earlier.

                    </p>

                    <ul>

                        <li>Early risk visibility</li>

                        <li>Care coordination support</li>

                        <li>Preventive intervention planning</li>

                    </ul>

                    <span class="status">
                        Framework Complete
                    </span>

                </div>

                <div class="solution-card">

                    <h3>
                        Clinical Documentation Automation
                    </h3>

                    <p>

                        Workflow-centered documentation assistance
                        designed to reduce clinician cognitive burden.

                    </p>

                    <ul>

                        <li>Adaptive workflow support</li>

                        <li>Contextual documentation suggestions</li>

                        <li>Operational efficiency enhancement</li>

                    </ul>

                    <span class="status">
                        Active Design
                    </span>

                </div>

            </div>

        </div>

    </section>

    <!-- CONTACT -->

    <section id="contact">

        <div class="container">

            <h2>
                Collaboration & Contact
            </h2>

            <div class="contact-box">

                <h3>
                    Open to Strategic Collaboration
                </h3>

                <p>

                    Interested in connecting with healthcare innovators,
                    AI developers, workflow architects, and organizations
                    focused on improving operational healthcare systems.

                </p>

                <div class="contact-info">

                    <p>

                        <strong>Email:</strong>

                        <a href="mailto:4charleneubaldo@gmail.com">
                            4charleneubaldo@gmail.com
                        </a>

                    </p>

                    <p>

                        <strong>LinkedIn:</strong>

                        <a href="https://www.linkedin.com/in/charlene-ubaldo-90943a6b" target="_blank">
                            Charlene Ubaldo
                        </a>

                    </p>

                </div>

            </div>

        </div>

    </section>

    <!-- FOOTER -->

    <footer>

        <p>

            <strong>
                Healthcare AI • Clinical Innovation • Workflow Systems
            </strong>

        </p>

        <p>

            Clinician-centered healthcare technology strategy
            built from real-world operational experience.

        </p>

    </footer>

</body>
</html>
