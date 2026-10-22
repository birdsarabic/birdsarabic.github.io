<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>{{ page.title }} | طيور العرب</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@400;500;700;800&display=swap" rel="stylesheet">
    
    <style>
        /* إجبار الصفحة بالكامل وكل مكوناتها على الاتجاه من اليمين لليسار */
        html, body, div, span, applet, object, iframe,
        h1, h2, h3, h4, h5, h6, p, blockquote, pre,
        a, abbr, acronym, address, big, cite, code,
        del, dfn, em, img, ins, kbd, q, s, samp,
        small, strike, strong, sub, sup, tt, var,
        b, u, i, center, dl, dt, dd, ol, ul, li,
        fieldset, form, label, legend, table, caption,
        tbody, tfoot, thead, tr, th, td, article,
        aside, canvas, details, embed, figure,
        figcaption, footer, header, hgroup, menu,
        nav, output, ruby, section, summary, time, mark, audio, video {
            direction: rtl !important;
            text-align: right !important;
        }

        :root {
            --primary-color: #0e6251;
            --accent-color: #d4ac0d;
            --bg-color: #f8f9fa;
            --text-color: #2c3e50;
        }

        body {
            font-family: 'Tajawal', sans-serif !important;
            background-color: var(--bg-color);
            color: var(--text-color);
            line-height: 2;
            margin: 0;
            padding: 0;
        }

        header {
            background-color: var(--primary-color);
            color: white;
            padding: 1.2rem 2rem;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        }

        .navbar {
            max-width: 900px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo a {
            color: white;
            text-decoration: none;
            font-size: 1.8rem;
            font-weight: 800;
        }

        .post-container {
            max-width: 850px;
            margin: 3rem auto;
            background: #ffffff;
            padding: 2.5rem;
            border-radius: 12px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.05);
        }

        .post-title {
            font-size: 2.2rem;
            color: var(--primary-color);
            margin-bottom: 1rem;
            font-weight: 800;
        }

        .post-meta {
            font-size: 0.9rem;
            color: #7f8c8d;
            margin-bottom: 2rem;
            border-bottom: 2px solid #eee;
            padding-bottom: 1rem;
        }

        .post-content h1, .post-content h2, .post-content h3 {
            color: var(--primary-color);
            margin: 2rem 0 1rem;
            font-weight: 700;
        }

        .post-content p {
            margin-bottom: 1.5rem;
            font-size: 1.1rem;
            color: #333;
        }

        .post-content img {
            max-width: 100%;
            height: auto;
            border-radius: 8px;
            margin: 1.5rem auto;
            display: block;
        }

        .post-content ul, .post-content ol {
            padding-right: 2rem !important;
            padding-left: 0 !important;
            margin-bottom: 1.5rem;
        }

        .post-content blockquote {
            background-color: #e8f8f5;
            border-right: 5px solid var(--primary-color) !important;
            border-left: none !important;
            padding: 1rem 1.5rem;
            margin: 1.5rem 0;
            border-radius: 4px;
        }

        .post-content table {
            width: 100%;
            border-collapse: collapse;
            margin: 2rem 0;
        }

        .post-content th, .post-content td {
            border: 1px solid #ddd;
            padding: 12px;
        }

        .post-content th {
            background-color: var(--primary-color);
            color: white;
        }

        footer {
            background-color: #1a252f;
            color: white;
            text-align: center;
            padding: 2rem 1rem;
            margin-top: 4rem;
        }
    </style>
</head>
<body>

    <header>
        <nav class="navbar">
            <div class="logo">
                <a href="{{ site.baseurl }}/">🦜 طيور العرب</a>
            </div>
        </nav>
    </header>

    <main class="post-container">
        <h1 class="post-title">{{ page.title }}</h1>
        <div class="post-meta">
            📅 تاريخ النشر: {{ page.date | date: "%Y-%m-%d" }}
        </div>
        
        <article class="post-content">
            {{ content }}
        </article>
    </main>

    <footer>
        <p>&copy; 2026 طيور العرب - جميع الحقوق محفوظة.</p>
    </footer>

</body>
</html>
