

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Explore the power of tiny changes with Atomic Habits by James Clear. Learn how small behaviors can lead to remarkable personal transformation.">
    <meta name="keywords" content="Atomic Habits, James Clear, habit formation, personal development, behavior change, productivity, identity habits">
    <meta name="author" content="Anamitra">
    <title>Atomic Habits | Master Tiny Changes for Big Results</title>
    <style>
        :root {
            --primary-color: #1e3a8a;
            --secondary-color: #2563eb;
            --accent-color: #3b82f6;
            --light-bg: #f1f5f9;
            --dark-bg: #1e293b;
            --text-dark: #1f2937;
            --text-light: #f8fafc;
            --shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
            --transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
        }

        /* Animations */
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        @keyframes slideUp {
            from {
                transform: translateY(30px);
                opacity: 0;
            }
            to {
                transform: translateY(0);
                opacity: 1;
            }
        }

        @keyframes scaleIn {
            from {
                transform: scale(0.95);
                opacity: 0;
            }
            to {
                transform: scale(1);
                opacity: 1;
            }
        }

        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.02); }
            100% { transform: scale(1); }
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: var(--light-bg);
            color: var(--text-dark);
            line-height: 1.6;
            animation: fadeIn 0.8s ease-out;
        }

        header {
            background: linear-gradient(135deg, var(--dark-bg), #0f172a);
            color: var(--text-light);
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 20px 30px;
            box-shadow: var(--shadow);
            animation: slideUp 0.6s ease-out;
        }

        .logo {
            display: flex;
            align-items: center;
        }

        .logo img {
            width: 50px;
            height: auto;
            margin-right: 15px;
            border-radius: 4px;
            transition: var(--transition);
        }

        .logo:hover img {
            transform: rotate(-5deg) scale(1.1);
        }

        .logo h1 {
            font-size: 1.8rem;
            color: var(--text-light);
            background: linear-gradient(to right, #ffffff, #e0e7ff);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            animation: fadeIn 1s ease-out;
        }

        header p {
            font-size: 1rem;
            color: #cbd5e1;
            text-align: right;
            opacity: 0;
            animation: fadeIn 0.8s ease-out forwards;
            animation-delay: 0.3s;
        }

        .cta-nav {
            background-color: #0f172a;
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 20px;
            padding: 15px 0;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            opacity: 0;
            animation: slideUp 0.6s ease-out forwards;
            animation-delay: 0.4s;
        }

        .cta-nav a {
            color: var(--text-light);
            text-decoration: none;
            background-color: var(--secondary-color);
            padding: 12px 24px;
            border-radius: 30px;
            font-weight: bold;
            transition: var(--transition);
            transform: translateY(0);
            box-shadow: 0 4px 8px rgba(37, 99, 235, 0.3);
        }

        .cta-nav a:hover {
            background-color: var(--primary-color);
            transform: translateY(-2px);
            box-shadow: 0 6px 12px rgba(37, 99, 235, 0.4);
        }

        .cta-nav a:active {
            transform: translateY(0);
        }

        .container {
            max-width: 1100px;
            margin: 30px auto;
            padding: 0 20px;
            animation: fadeIn 0.8s ease-out;
            animation-delay: 0.6s;
        }

        section {
            background-color: white;
            padding: 30px;
            border-radius: 10px;
            box-shadow: var(--shadow);
            margin-bottom: 40px;
            opacity: 0;
            animation: slideUp 0.8s ease-out forwards;
            animation-delay: 0.8s;
            transition: var(--transition);
        }

        section:hover {
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.15);
            transform: translateY(-3px);
        }

        h2 {
            color: var(--primary-color);
            margin-bottom: 15px;
            font-size: 1.8rem;
            border-bottom: 2px solid #e2e8f0;
            padding-bottom: 8px;
            position: relative;
        }

        h2::after {
            content: '';
            position: absolute;
            bottom: -2px;
            left: 0;
            width: 70px;
            height: 3px;
            background: var(--accent-color);
            border-radius: 3px;
        }

        p {
            font-size: 1.1rem;
            margin-bottom: 15px;
        }

        strong {
            color: var(--primary-color);
        }

        img {
            width: 100%;
            height: auto;
            border-radius: 10px;
            margin-top: 20px;
            box-shadow: var(--shadow);
            transition: var(--transition);
        }

        img:hover {
            transform: scale(1.02);
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
        }

        footer {
            background: linear-gradient(135deg, var(--dark-bg), #0f172a);
            color: var(--text-light);
            text-align: center;
            padding: 25px 10px;
            font-size: 0.95rem;
            opacity: 0;
            animation: fadeIn 0.8s ease-out forwards;
            animation-delay: 1s;
        }

        footer p {
            margin-bottom: 5px;
        }

        footer strong {
            color: var(--accent-color);
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            header {
                flex-direction: column;
                text-align: center;
                padding: 20px 15px;
            }

            .logo {
                margin-bottom: 15px;
                justify-content: center;
            }

            header p {
                text-align: center;
            }

            .cta-nav {
                gap: 10px;
                padding: 10px;
            }

            .cta-nav a {
                padding: 8px 16px;
                font-size: 0.9rem;
            }

            section {
                padding: 20px;
            }

            h2 {
                font-size: 1.5rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="logo">
            <img src="https://m.media-amazon.com/images/I/91bYsX41DVL.jpg" alt="Atomic Habits Logo">
            <h1>Atomic Habits</h1>
        </div>
        <p>Transform your habits. Transform your life.</p>
    </header>

    <nav class="cta-nav">
        <a href="about.html">About the Book</a>
        <a href="author.html">About the Author</a>
        <a href="laws.html">The Four Laws</a>
        <a href="takeaways.html">Key Takeaways</a>
    </nav>

    <div class="container">
        <section>
            <h2>Welcome to the Atomic Habits Guide</h2>
            <p>This platform is your one-stop knowledge hub on James Clear's best-selling book <strong>Atomic Habits</strong>. Click on the sections above to explore insightful breakdowns of the book's core concepts.</p>
            <p>Discover how tiny changes can lead to remarkable results through our comprehensive guides, visual explanations, and practical applications of Clear's revolutionary framework.</p>
            <img src="https://m.media-amazon.com/images/I/91bYsX41DVL.jpg" alt="Atomic Habits Book Cover">
        </section>
    </div>

    <footer>
        <p>&copy; 2025 Atomic Habits Project. All rights reserved.</p>
        <p>Site developed and maintained by <strong>Anamitra</strong>. Unauthorized duplication is prohibited.</p>
    </footer>
</body>
</html>
