<style>
    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }

    :root {
        --primary-blue: #5B8DEF;
        --secondary-blue: #7FA8F8;
        --light-blue: #EAF2FF;
        --soft-gray: #F7F9FC;
        --white: #FFFFFF;
        --text-dark: #425466;
        --text-light: #6B7A90;
        --border-light: #DCE6F5;
    }

    html {
        scroll-behavior: smooth;
    }

    body {
        font-family: 'DM Sans', sans-serif;
        line-height: 1.6;
        color: var(--text-dark);
        background: var(--white);
        overflow-x: hidden;
    }

    /* Navigation */
    nav {
        position: sticky;
        top: 0;
        background: rgba(255,255,255,0.95);
        backdrop-filter: blur(10px);
        color: var(--text-dark);
        padding: 1.2rem 3rem;
        display: flex;
        justify-content: space-between;
        align-items: center;
        z-index: 1000;
        border-bottom: 1px solid var(--border-light);
        box-shadow: 0 2px 12px rgba(91,141,239,0.08);
    }

    nav .logo {
        font-family: 'Playfair Display', serif;
        font-size: 1.4rem;
        font-weight: 800;
        color: var(--primary-blue);
    }

    nav ul {
        display: flex;
        list-style: none;
        gap: 2rem;
    }

    nav a {
        color: var(--text-dark);
        text-decoration: none;
        font-size: 0.95rem;
        font-weight: 600;
        transition: 0.3s ease;
        position: relative;
    }

    nav a:hover {
        color: var(--primary-blue);
    }

    /* Hero */
    .hero {
        background: linear-gradient(135deg, #F7FAFF 0%, #EAF2FF 100%);
        color: var(--text-dark);
        padding: 8rem 3rem 6rem;
        position: relative;
        overflow: hidden;
    }

    .hero::before {
        content: '';
        position: absolute;
        top: -200px;
        right: -100px;
        width: 500px;
        height: 500px;
        background: rgba(91,141,239,0.08);
        border-radius: 50%;
    }

    .hero-content {
        position: relative;
        z-index: 2;
        max-width: 900px;
    }

    .hero h1 {
        font-family: 'Playfair Display', serif;
        font-size: 4rem;
        font-weight: 800;
        margin-bottom: 1.5rem;
        line-height: 1.1;
        color: var(--primary-blue);
    }

    .hero .subtitle {
        font-size: 1.3rem;
        color: var(--text-light);
        margin-bottom: 2rem;
        max-width: 700px;
    }

    .credentials {
        background: rgba(255,255,255,0.8);
        border: 1px solid var(--border-light);
        padding: 1.5rem 2rem;
        border-radius: 16px;
        margin: 2rem 0;
        color: var(--text-dark);
        box-shadow: 0 4px 20px rgba(91,141,239,0.08);
    }

    .cta-buttons {
        display: flex;
        gap: 1rem;
        flex-wrap: wrap;
    }

    .btn {
        padding: 1rem 2.5rem;
        border-radius: 12px;
        text-decoration: none;
        font-weight: 700;
        transition: 0.3s ease;
        display: inline-block;
    }

    .btn-primary {
        background: var(--primary-blue);
        color: white;
        box-shadow: 0 8px 24px rgba(91,141,239,0.25);
    }

    .btn-primary:hover {
        transform: translateY(-3px);
        background: var(--secondary-blue);
    }

    .btn-secondary {
        background: white;
        border: 1px solid var(--border-light);
        color: var(--primary-blue);
    }

    .btn-secondary:hover {
        transform: translateY(-3px);
        background: var(--light-blue);
    }

    /* Sections */
    section {
        padding: 5rem 3rem;
    }

    .light-bg {
        background: var(--soft-gray);
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

    p {
        color: var(--text-dark);
        line-height: 1.8;
    }

    /* Cards */
    .foundation-grid,
    .building-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
        gap: 2rem;
        margin-top: 3rem;
    }

    .foundation-card,
    .solution-card,
    .advantage-item {
        background: white;
        padding: 2rem;
        border-radius: 20px;
        border: 1px solid var(--border-light);
        box-shadow: 0 8px 30px rgba(91,141,239,0.08);
        transition: 0.3s ease;
    }

    .foundation-card:hover,
    .solution-card:hover,
    .advantage-item:hover {
        transform: translateY(-5px);
    }

    .foundation-card h4,
    .solution-card h3 {
        color: var(--primary-blue);
    }

    /* Vision */
    .vision-section {
        background: linear-gradient(135deg, #DCEBFF 0%, #F7FAFF 100%);
        position: relative;
        overflow: hidden;
        text-align: center;
    }

    .vision-content {
        max-width: 800px;
        margin: auto;
        position: relative;
        z-index: 2;
    }

    .vision-content h2 {
        color: var(--primary-blue);
    }

    .vision-content p {
        color: var(--text-light);
        font-size: 1.2rem;
    }

    /* Status */
    .status {
        display: inline-block;
        background: var(--light-blue);
        color: var(--primary-blue);
        padding: 0.5rem 1rem;
        border-radius: 999px;
        font-size: 0.85rem;
        font-weight: 700;
        margin-top: 1rem;
    }

    /* Contact */
    .contact-box {
        background: linear-gradient(135deg, #F7FAFF 0%, #EAF2FF 100%);
        border: 1px solid var(--border-light);
        padding: 3rem;
        border-radius: 24px;
        box-shadow: 0 8px 30px rgba(91,141,239,0.08);
    }

    .contact-info a {
        color: var(--primary-blue);
        text-decoration: none;
        font-weight: 600;
    }

    /* Footer */
    footer {
        background: #F7FAFF;
        color: var(--text-light);
        text-align: center;
        padding: 2rem;
        border-top: 1px solid var(--border-light);
    }

    /* Responsive */
    @media (max-width: 768px) {

        nav {
            padding: 1rem 1.5rem;
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
