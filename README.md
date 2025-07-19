<!DOCTYPE html>
<html lang="he" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>מערכת ניתוח נתונים למכירת רכבים 🚗📊</title>
  <link href="https://fonts.googleapis.com/css2?family=Noto+Sans+Hebrew:wght@400;700&display=swap" rel="stylesheet">
  <script src="https://cdn.tailwindcss.com"></script>
  <style>
    body {
      font-family: 'Noto Sans Hebrew', sans-serif;
    }
    .hero-bg {
      background: linear-gradient(135deg, #3b82f6, #ec4899, #10b981, #8b5cf6);
      background-size: 400% 400%;
      animation: gradientAnimation 12s ease infinite;
    }
    .card {
      transition: transform 0.4s ease, box-shadow 0.4s ease;
    }
    .card:hover {
      transform: translateY(-12px) scale(1.02);
      box-shadow: 0 20px 40px rgba(0, 0, 0, 0.25);
    }
    .btn {
      transition: background-color 0.3s ease, transform 0.3s ease;
    }
    .btn:hover {
      transform: scale(1.1);
    }
    .nav-btn.active {
      background-color: #1e40af;
      animation: pulse 2s infinite;
    }
    .section-hidden {
      opacity: 0;
      transform: translateY(30px);
      transition: opacity 0.6s ease, transform 0.6s ease;
    }
    .section-visible {
      opacity: 1;
      transform: translateY(0);
    }
    .tableau-embed {
      height: 800px;
      width: 100%;
      border-radius: 1rem;
      overflow: hidden;
    }
    @keyframes gradientAnimation {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }
    @keyframes pulse {
      0% { transform: scale(1); }
      50% { transform: scale(1.1); }
      100% { transform: scale(1); }
    }
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }
  </style>
</head>
<body class="bg-gradient-to-b from-gray-50 to-gray-200 text-gray-900">
  <!-- Hero Section -->
  <header class="hero-bg text-white py-24 relative overflow-hidden">
    <div class="container mx-auto px-4 text-center">
      <h1 class="text-4xl md:text-6xl font-bold mb-4 animate-[fadeIn_1s_ease-out]">מערכת ניתוח נתונים למכירת רכבים 🚗🎉</h1>
      <p class="text-xl md:text-3xl mb-8">גלה תובנות מדהימות עם דשבורדים אינטראקטיביים ב-Tableau! 📊</p>
      <a href="#dashboards" class="inline-block bg-white text-blue-600 font-semibold py-3 px-8 rounded-full btn hover:bg-blue-100 pulse">צפה בדשבורדים 🌟</a>
    </div>
  </header>

  <!-- Navigation Bar -->
  <nav class="sticky top-0 bg-white shadow-lg z-10 py-4">
    <div class="container mx-auto px-4 flex justify-center gap-4">
      <a href="#strategic" class="nav-btn bg-blue-600 text-white py-2 px-6 rounded-full btn hover:bg-blue-700">דשבורד אסטרטגי 🌍</a>
      <a href="#managerial" class="nav-btn bg-green-600 text-white py-2 px-6 rounded-full btn hover:bg-green-700">דשבורד ניהולי 👨‍💼</a>
      <a href="#operational" class="nav-btn bg-purple-600 text-white py-2 px-6 rounded-full btn hover:bg-purple-700">דשבורד תפעולי ⚙️</a>
    </div>
  </nav>

  <!-- Main Content -->
  <main class="container mx-auto px-4 py-12">
    <!-- System Overview -->
    <section id="overview" class="mb-20 section-hidden">
      <h2 class="text-4xl font-bold text-center text-blue-900 mb-8">על המערכת שלנו 🚘</h2>
      <div class="bg-white p-10 rounded-3xl shadow-2xl card max-w-4xl mx-auto">
        <h3 class="text-2xl font-semibold text-blue-700 mb-4">סקירה כללית</h3>
        <p class="text-lg leading-relaxed text-gray-700">
          מערכת המידע שלנו למכירת רכבים היא פלטפורמה מתקדמת לניתוח נתונים ממכירות, מלאי ולקוחות. היא מספקת דשבורדים אינטראקטיביים ב-Tableau המותאמים להנהלה, מנהלים וצוותים תפעוליים, לקבלת החלטות מהירות ומדויקות! 📈😊
        </p>
      </div>
    </section>

    <!-- Dashboards Section -->
    <section id="dashboards" class="mb-20">
      <!-- Strategic Dashboard -->
      <div id="strategic" class="mb-12 section-hidden">
        <div class="bg-gradient-to-br from-blue-200 to-blue-400 p-8 rounded-3xl shadow-xl card">
          <h3 class="text-2xl font-semibold text-blue-800 mb-3">דשבורד אסטרטגי 🌍</h3>
          <p class="text-gray-700 mb-4">
            מיועד להנהלה הבכירה, מציג הכנסות, נתח שוק ותחזיות עם גרפים מרהיבים! 📈
          </p>
          <ul class="list-disc mr-4 text-gray-700 mb-4">
            <li>מכירות לפי חודשים</li>
            <li>השוואת מחיר מחירון למחיר בפועל לפי מותג</li>
            <li>מכירות לאורך זמן</li>
          </ul>
          <iframe src="https://public.tableau.com/views/_17529314688580/sheet3?:language=en-US&:display_count=n&:origin=viz_share_link&:showVizHome=no" class="tableau-embed" title="דשבורד אסטרטגי"></iframe>
        </div>
      </div>

      <!-- Managerial Dashboard -->
      <div id="managerial" class="mb-12 section-hidden">
        <div class="bg-gradient-to-br from-green-200 to-green-400 p-8 rounded-3xl shadow-xl card">
          <h3 class="text-2xl font-semibold text-green-800 mb-3">דשבורד ניהולי 👨‍💼</h3>
          <p class="text-gray-700 mb-4">
            תומך במנהלי מחלקות עם נתונים על אנשי מכירות, סניפים ודגמים! 😊
          </p>
          <ul class="list-disc mr-4 text-gray-700 mb-4">
            <li>ביצועי אנשי מכירות בסניפים</li>
            <li>פירוט עסקאות לפי סניפים</li>
            <li>דגמים נמכרים ביותר</li>
          </ul>
          <iframe src="https://public.tableau.com/views/_17529321384840/sheet10?:language=en-US&:display_count=n&:origin=viz_share_link&:showVizHome=no" class="tableau-embed" title="דשבורד ניהולי"></iframe>
        </div>
      </div>

      <!-- Operational Dashboard -->
      <div id="operational" class="mb-12 section-hidden">
        <div class="bg-gradient-to-br from-purple-200 to-purple-400 p-8 rounded-3xl shadow-xl card">
          <h3 class="text-2xl font-semibold text-purple-800 mb-3">דשבורד תפעולי ⚙️</h3>
          <p class="text-gray-700 mb-4">
            מסייע לצוותים תפעוליים בניהול עסקאות ותהליכים! 🚀
          </p>
          <ul class="list-disc mr-4 text-gray-700 mb-4">
            <li>סוגי תשלום לפי סניף</li>
            <li>פערים בין מחירונים לתשלומים</li>
            <li>גיל לקוח מול סכום קנייה</li>
          </ul>
          <iframe src="https://public.tableau.com/views/_17529322897620/sheet11?:language=en-US&:display_count=n&:origin=viz_share_link&:showVizHome=no" class="tableau-embed" title="דשבורד תפעולי"></iframe>
        </div>
      </div>
    </section>
  </main>

  <!-- Footer -->
  <footer class="hero-bg text-white py-10">
    <div class="container mx-auto px-4 text-center">
      <p class="text-lg mb-4">© 2025 מערכת ניתוח נתונים למכירת רכבים. כל הזכויות שמורות. 🎉</p>
      <a href="#overview" class="inline-block bg-white text-blue-600 font-semibold py-2 px-6 rounded-full btn hover:bg-blue-100">חזור למעלה ⬆️</a>
    </div>
  </footer>

  <script>
    // Scroll animation for sections
    document.addEventListener('DOMContentLoaded', () => {
      const sections = document.querySelectorAll('.section-hidden');
      const navButtons = document.querySelectorAll('.nav-btn');
      
      const observer = new IntersectionObserver((entries) => {
        entries.forEach(entry => {
          if (entry.isIntersecting) {
            entry.target.classList.add('section-visible');
            // Highlight active nav button
            navButtons.forEach(btn => btn.classList.remove('active'));
            const activeBtn = document.querySelector(`a[href="#${entry.target.id}"]`);
            if (activeBtn) activeBtn.classList.add('active');
            observer.unobserve(entry.target);
          }
        });
      }, { threshold: 0.2 });

      sections.forEach(section => observer.observe(section));
    });
  </script>
</body>
</html>
