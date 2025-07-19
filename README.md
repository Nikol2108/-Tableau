<!DOCTYPE html>
<html lang="he" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>מערכת מידע למכירת רכבים 🚗📊</title>
  <link href="https://fonts.googleapis.com/css2?family=Noto+Sans+Hebrew:wght@400;700&display=swap" rel="stylesheet">
  <script src="https://cdn.tailwindcss.com"></script>
  <style>
    body {
      font-family: 'Noto Sans Hebrew', sans-serif;
    }
    .hero-bg {
      background: linear-gradient(135deg, #3b82f6, #ec4899, #10b981, #8b5cf6);
      background-size: 400% 400%;
      animation: gradientAnimation 10s ease infinite;
    }
    .card {
      transition: transform 0.4s ease, box-shadow 0.4s ease;
    }
    .card:hover {
      transform: translateY(-12px) scale(1.05);
      box-shadow: 0 20px 40px rgba(0, 0, 0, 0.25);
    }
    .btn {
      transition: background-color 0.3s ease, transform 0.3s ease;
    }
    .btn:hover {
      transform: scale(1.1);
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
    .pulse {
      animation: pulse 2s infinite;
    }
  </style>
</head>
<body class="bg-gradient-to-b from-gray-50 to-gray-200 text-gray-900">
  <!-- Hero Section -->
  <header class="hero-bg text-white py-24 relative overflow-hidden">
    <div class="container mx-auto px-4 text-center">
      <h1 class="text-4xl md:text-6xl font-bold mb-4 animate-[fadeIn_1s_ease-out]">ניתוח נתונים של חברת הרכבים הגדולה בקלות וביעילות 🚗🎉</h1>
      <p class="text-xl md:text-3xl mb-8">גלה את כוח הנתונים עם דשבורדים צבעוניים וחכמים! 📊</p>
      <a href="#tableau" class="inline-block bg-white text-blue-600 font-semibold py-3 px-8 rounded-full btn hover:bg-blue-100 pulse">צפה בדשבורד Tableau 🌟</a>
    </div>
  </header>

  <!-- Main Content -->
  <main class="container mx-auto px-4 py-12">
    <!-- System Overview -->
    <section id="overview" class="mb-20 section-hidden">
      <h2 class="text-4xl font-bold text-center text-blue-900 mb-8">על המערכת שלנו 🚘</h2>
      <div class="bg-white p-10 rounded-3xl shadow-2xl card max-w-4xl mx-auto">
        <h3 class="text-2xl font-semibold text-blue-700 mb-4">סקירה כללית</h3>
        <p class="text-lg leading-relaxed text-gray-700">
          מערכת המידע שלנו למכירת רכבים היא פלטפורמה חדשנית המשלבת ניתוח נתונים ממכירות, מלאי ולקוחות. היא מציעה דשבורדים אינטראקטיביים המותאמים לכל רמות הארגון, לקבלת החלטות מהירות ומדויקות! 📈😊
        </p>
      </div>
    </section>

    <!-- Dashboards Section -->
    <section id="dashboards" class="mb-20 section-hidden">
      <h2 class="text-4xl font-bold text-center text-blue-900 mb-10">דשבורדים צבעוניים 📊</h2>
      <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
        <!-- Strategic Dashboard -->
        <div class="bg-gradient-to-br from-blue-200 to-blue-400 p-8 rounded-3xl shadow-xl card">
          <img src="https://source.unsplash.com/400x200/?charts,strategy" alt="דשבורד אסטרטגי" class="w-full h-40 object-cover rounded-lg mb-4">
          <h3 class="text-2xl font-semibold text-blue-800 mb-3">דשבורד אסטרטגי 🌍</h3>
          <p class="text-gray-700 mb-4">
            מיועד להנהלה הבכירה, מציג הכנסות, נתח שוק ותחזיות עם גרפים מרהיבים! 📈
          </p>
          <ul class="list-disc mr-4 text-gray-700 mb-4">
            <li>מכירות לפי חודשים</li>
            <li>השוואת מכירות בין מחיר מחירון לבין מחיר בפועל לפי מותג</li>
            <li>מכירות לאורך זמן</li>
          </ul>
          <div class="flex gap-4">
            <button onclick="openModal('strategic')" class="bg-blue-600 text-white py-2 px-6 rounded-full btn hover:bg-blue-700">פרטים נוספים 🔍</button>
            <a href="https://public.tableau.com/app/profile/nikol.nutenko/viz/_17529314688580/sheet3?publish=yes" target="_blank" class="bg-blue-800 text-white py-2 px-6 rounded-full btn hover:bg-blue-900">צפה בדשבורד 🚀</a>
          </div>
        </div>

        <!-- Managerial Dashboard -->
        <div class="bg-gradient-to-br from-green-200 to-green-400 p-8 rounded-3xl shadow-xl card">
          <img src="https://source.unsplash.com/400x200/?business,management" alt="דשבורד ניהולי" class="w-full h-40 object-cover rounded-lg mb-4">
          <h3 class="text-2xl font-semibold text-green-800 mb-3">דשבורד ניהולי 👨‍💼</h3>
          <p class="text-gray-700 mb-4">
            תומך במנהלי מחלקות ומציג נתונים על אנשי מכירות, סניפים ודגמי רכבים! 😊
          </p>
          <ul class="list-disc mr-4 text-gray-700 mb-4">
            <li>ביצועי אנשי מכירות בסניפים</li>
            <li>פירוט עסקאות לפי סניפים</li>
            <li>ניתוח הדגמים הנמכרים ביותר בכל סניף</li>
          </ul>
          <div class="flex gap-4">
            <button onclick="openModal('managerial')" class="bg-green-600 text-white py-2 px-6 rounded-full btn hover:bg-green-700">פרטים נוספים 🔍</button>
            <a href="https://public.tableau.com/app/profile/nikol.nutenko/viz/_17529321384840/sheet10?publish=yes" target="_blank" class="bg-green-800 text-white py-2 px-6 rounded-full btn hover:bg-green-900">צפה בדשבורד 🚀</a>
          </div>
        </div>

        <!-- Operational Dashboard -->
        <div class="bg-gradient-to-br from-purple-200 to-purple-400 p-8 rounded-3xl shadow-xl card">
          <img src="https://source.unsplash.com/400x200/?operations,data" alt="דשבורד תפעולי" class="w-full h-40 object-cover rounded-lg mb-4">
          <h3 class="text-2xl font-semibold text-purple-800 mb-3">דשבורד תפעולי ⚙️</h3>
          <p class="text-gray-700 mb-4">
            מסייע לצוותים תפעוליים בניהול העסקאות! 🚀
          </p>
          <ul class="list-disc mr-4 text-gray-700 mb-4">
            <li>ניתוח סוגי התשלום לפי סניף</li>
            <li>ניתוח פערים בין מחירונים לפי סוגי התשלום</li>
            <li>הפערים בין גיל הלקוח לסכום קנייתו</li>
          </ul>
          <div class="flex gap-4">
            <button onclick="openModal('operational')" class="bg-purple-600 text-white py-2 px-6 rounded-full btn hover:bg-purple-700">פרטים נוספים 🔍</button>
            <a href="https://public.tableau.com/app/profile/nikol.nutenko/viz/_17529322897620/sheet11?publish=yes" target="_blank" class="bg-purple-800 text-white py-2 px-6 rounded-full btn hover:bg-purple-900">צפה בדשבורד 🚀</a>
          </div>
        </div>
      </div>
    </section>

  </main>

  <!-- Modal for Dashboard Details -->
  <div id="modal" class="fixed inset-0 bg-black bg-opacity-50 hidden items-center justify-center">
    <div class="bg-white p-8 rounded-2xl max-w-lg w-full transition-all duration-300">
      <h3 id="modal-title" class="text-2xl font-bold text-blue-900 mb-4"></h3>
      <p id="modal-content" class="text-gray-700 mb-6"></p>
      <div class="flex gap-4">
        <button onclick="closeModal()" class="bg-gray-600 text-white py-2 px-6 rounded-full btn hover:bg-gray-700">סגור ❌</button>
        <a id="modal-link" href="#" target="_blank" class="bg-blue-600 text-white py-2 px-6 rounded-full btn hover:bg-blue-700">צפה בדשבורד 🚀</a>
      </div>
    </div>
  </div>

  <!-- Footer -->
  <footer class="hero-bg text-white py-10">
    <div class="container mx-auto px-4 text-center">
      <p class="text-lg">© 2025 מערכת מידע למכירת רכבים. כל הזכויות שמורות. 🎉</p>
    </div>
  </footer>

  <script>
    // Modal functionality
    function openModal(type) {
      const modal = document.getElementById('modal');
      const title = document.getElementById('modal-title');
      const content = document.getElementById('modal-content');
      const link = document.getElementById('modal-link');
      
      if (type === 'strategic') {
        title.textContent = 'דשבורד אסטרטגי 🌍';
        content.textContent = 'הדשבורד האסטרטגי מספק תובנות להנהלה עם מדדי מפתח כמו הכנסות ונתח שוק, עם גרפים אינטראקטיביים לתכנון ארוך טווח! 📈';
        link.href = 'https://public.tableau.com/app/profile/nikol.nutenko/viz/_17529314688580/sheet3?publish=yes';
      } else if (type === 'managerial') {
        title.textContent = 'דשבורד ניהולי 👨‍💼';
        content.textContent = 'הדשבורד הניהולי תומך במנהלים עם נתונים על ביצועי סניפים ושביעות רצון לקוחות, לניהול יעיל ומהיר! 😊';
        link.href = 'https://public.tableau.com/app/profile/nikol.nutenko/viz/_17529321384840/sheet10?publish=yes';
      } else if (type === 'operational') {
        title.textContent = 'דשבורד תפעולי ⚙️';
        content.textContent = 'הדשבורד התפעולי מסייע לצוותים בניהול מלאי ותקלות, תוך שיפור היעילות היומיומית בזמן אמת! 🚀';
        link.href = 'https://public.tableau.com/app/profile/nikol.nutenko/viz/_17529322897620/sheet11?publish=yes';
      }
      
      modal.classList.remove('hidden');
      modal.classList.add('flex');
    }

    function closeModal() {
      const modal = document.getElementById('modal');
      modal.classList.add('hidden');
      modal.classList.remove('flex');
    }

    // Scroll animation for sections
    document.addEventListener('DOMContentLoaded', () => {
      const sections = document.querySelectorAll('.section-hidden');
      const observer = new IntersectionObserver((entries) => {
        entries.forEach(entry => {
          if (entry.isIntersecting) {
            entry.target.classList.add('section-visible');
            observer.unobserve(entry.target);
          }
        });
      }, { threshold: 0.1 });

      sections.forEach(section => observer.observe(section));
    });
  </script>
</body>
</html>
