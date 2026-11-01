<!DOCTYPE html>
<html lang="bn">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>বাবুগঞ্জ বার্তা - সত্য ও সাহসের সাথে</title>
  <style>
    :root {
      --primary: #c8102e;
      --dark: #111827;
      --light: #f9fafb;
      --card-bg: #ffffff;
      --text: #1f2937;
      --border: #e5e7eb;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }

    body {
      background-color: #f3f4f6;
      color: var(--text);
      line-height: 1.6;
    }

    /* Ad Container Styles */
    .ad-container {
      background: #eef2ff;
      border: 1px dashed #6366f1;
      text-align: center;
      padding: 10px;
      margin: 15px auto;
      border-radius: 6px;
      overflow: hidden;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .ad-728x90 {
      min-height: 90px;
      max-width: 728px;
    }

    .ad-300x250 {
      min-height: 250px;
      width: 300px;
    }

    .ad-468x60 {
      min-height: 60px;
      max-width: 468px;
    }

    /* Top Greeting & Date Header */
    .top-header {
      color: white;
      padding: 12px 20px;
      transition: background 0.5s;
    }

    .greeting-banner {
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
      max-width: 1200px;
      margin: 0 auto;
    }

    .greeting-text {
      font-size: 1.3rem;
      font-weight: bold;
      display: flex;
      align-items: center;
      gap: 8px;
    }

    .dates-bar {
      font-size: 0.9rem;
      background: rgba(0, 0, 0, 0.2);
      padding: 6px 14px;
      border-radius: 20px;
      display: flex;
      gap: 15px;
      flex-wrap: wrap;
    }

    /* Site Title Branding */
    .brand-header {
      background: #ffffff;
      padding: 20px 0;
      text-align: center;
      border-bottom: 2px solid var(--primary);
    }

    .brand-header h1 {
      color: var(--primary);
      font-size: 2.8rem;
      letter-spacing: -1px;
    }

    .brand-header p {
      color: #6b7280;
      font-size: 1rem;
    }

    /* Navigation */
    nav {
      background: var(--dark);
      position: sticky;
      top: 0;
      z-index: 100;
    }

    .nav-container {
      max-width: 1200px;
      margin: 0 auto;
      display: flex;
      overflow-x: auto;
    }

    .nav-container a {
      color: white;
      padding: 12px 20px;
      text-decoration: none;
      white-space: nowrap;
      font-size: 1rem;
    }

    .nav-container a:hover, .nav-container a.active {
      background: var(--primary);
    }

    /* Main Container Grid */
    .container {
      max-width: 1200px;
      margin: 20px auto;
      padding: 0 15px;
      display: grid;
      grid-template-columns: 2fr 1fr;
      gap: 20px;
    }

    @media (max-width: 768px) {
      .container {
        grid-template-columns: 1fr;
      }
    }

    /* Live TV Section */
    .tv-section {
      background: #000;
      border-radius: 8px;
      padding: 15px;
      color: white;
      margin-bottom: 25px;
    }

    .tv-header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-bottom: 10px;
    }

    .tv-buttons {
      display: flex;
      gap: 8px;
    }

    .tv-btn {
      background: #374151;
      color: white;
      border: none;
      padding: 6px 12px;
      border-radius: 4px;
      cursor: pointer;
      font-size: 0.85rem;
    }

    .tv-btn.active {
      background: var(--primary);
    }

    .iframe-container {
      position: relative;
      width: 100%;
      padding-bottom: 56.25%;
      height: 0;
    }

    .iframe-container iframe {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      border: 0;
      border-radius: 4px;
    }

    /* News Post Form */
    .post-form-card {
      background: white;
      padding: 20px;
      border-radius: 8px;
      box-shadow: 0 2px 4px rgba(0,0,0,0.05);
      margin-bottom: 25px;
    }

    .post-form-card h3 {
      margin-bottom: 15px;
      color: var(--dark);
      border-left: 4px solid var(--primary);
      padding-left: 8px;
    }

    .form-group {
      margin-bottom: 12px;
    }

    .form-group label {
      display: block;
      font-size: 0.88rem;
      margin-bottom: 5px;
      font-weight: 600;
    }

    .form-group input, .form-group textarea, .form-group select {
      width: 100%;
      padding: 8px 12px;
      border: 1px solid var(--border);
      border-radius: 4px;
      font-size: 0.9rem;
    }

    .btn-submit {
      background: var(--primary);
      color: white;
      border: none;
      padding: 10px 18px;
      border-radius: 4px;
      cursor: pointer;
      font-weight: bold;
      width: 100%;
    }

    /* News Feed Grid */
    .news-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
      gap: 20px;
    }

    .news-card {
      background: white;
      border-radius: 8px;
      overflow: hidden;
      box-shadow: 0 2px 5px rgba(0,0,0,0.05);
      display: flex;
      flex-direction: column;
    }

    .news-img {
      width: 100%;
      height: 180px;
      object-fit: cover;
      background: #e5e7eb;
    }

    .news-content {
      padding: 15px;
      flex-grow: 1;
      display: flex;
      flex-direction: column;
    }

    .news-tag {
      font-size: 0.75rem;
      background: #fee2e2;
      color: var(--primary);
      padding: 2px 8px;
      border-radius: 4px;
      width: fit-content;
      margin-bottom: 8px;
      font-weight: bold;
    }

    .news-title {
      font-size: 1.1rem;
      font-weight: bold;
      margin-bottom: 8px;
      line-height: 1.4;
    }

    .news-desc {
      font-size: 0.9rem;
      color: #4b5563;
      margin-bottom: 12px;
      flex-grow: 1;
    }

    .news-link-box {
      background: #f3f4f6;
      border: 1px solid #d1d5db;
      padding: 8px 10px;
      border-radius: 6px;
      font-size: 0.85rem;
      margin-bottom: 12px;
      word-break: break-all;
    }

    .news-link-box a {
      color: #1d4ed8;
      text-decoration: underline;
      font-weight: bold;
    }

    .share-buttons {
      display: flex;
      gap: 6px;
      border-top: 1px solid var(--border);
      padding-top: 10px;
    }

    .share-btn {
      flex: 1;
      padding: 6px;
      border: none;
      border-radius: 4px;
      color: white;
      font-size: 0.78rem;
      cursor: pointer;
      text-align: center;
      text-decoration: none;
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .btn-fb { background: #1877f2; }
    .btn-wa { background: #25d366; }
    .btn-copy { background: #4b5563; }

    footer {
      background: var(--dark);
      color: white;
      text-align: center;
      padding: 20px;
      margin-top: 40px;
    }
  </style>
</head>
<body>

  <!-- Dynamic Time Banner -->
  <div class="top-header" id="greetingHeader">
    <div class="greeting-banner">
      <div class="greeting-text" id="greetingText">
        <span>👋</span> <span>শুভ বার্তা</span>
      </div>
      <div class="dates-bar">
        <span id="engDate">...</span> | 
        <span id="bngDate">...</span> | 
        <span id="hijriDate">...</span>
      </div>
    </div>
  </div>

  <!-- Adsterra Header Banner Spot (468x60 বসানো হলো) -->
  <div class="ad-container ad-468x60">
    <script>
      atOptions = {
        'key' : '866f6c699bd9fce63d3e0bfd5b973b1e',
        'format' : 'iframe',
        'height' : 60,
        'width' : 468,
        'params' : {}
      };
    </script>
    <script src="https://www.highrevenueformat.com/866f6c699bd9fce63d3e0bfd5b973b1e/invoke.js"></script>
  </div>

  <!-- Site Title -->
  <header class="brand-header">
    <h1>বাবুগঞ্জ বার্তা</h1>
    <p>সত্য ও সঠিক সংবাদের বিশ্বাসযোগ্য ঠিকানা</p>
  </header>

  <!-- Navigation -->
  <nav>
    <div class="nav-container">
      <a href="#" class="active">প্রচ্ছদ</a>
      <a href="#">জাতীয়</a>
      <a href="#">বাবুগঞ্জ</a>
      <a href="#">রাজনীতি</a>
      <a href="#">খেলাধুলা</a>
      <a href="#">বিনোদন</a>
      <a href="#">প্রযুক্তি</a>
    </div>
  </nav>

  <div class="container">
    <!-- Left Column (News Feed & Live TV) -->
    <main>
      <!-- Live TV Player -->
      <section class="tv-section">
        <div class="tv-header">
          <h3>🔴 লাইভ টিভি স্ট্রিমিং</h3>
          <div class="tv-buttons">
            <button class="tv-btn active" onclick="changeChannel('jamuna', this)">Jamuna TV</button>
            <button class="tv-btn" onclick="changeChannel('dbc', this)">DBC News</button>
            <button class="tv-btn" onclick="changeChannel('somoy', this)">Somoy TV</button>
          </div>
        </div>
        <div class="iframe-container">
          <iframe id="tvIframe" src="https://www.youtube.com/embed/live_stream?channel=UCjH5l0jR3F-Wq8CjT5B4Xsw" allowfullscreen></iframe>
        </div>
      </section>

      <!-- News Articles Grid -->
      <h3 style="margin-bottom: 15px; border-left: 4px solid var(--primary); padding-left: 8px;">সর্বশেষ সংবাদ</h3>
      <div class="news-grid" id="newsGrid">
        
        <!-- Default Post 1 With External Link -->
        <div class="news-card">
          <img src="https://picsum.photos/400/250?random=1" class="news-img" alt="নিউজ ছবি">
          <div class="news-content">
            <span class="news-tag">ফেসবুক খবর</span>
            <div class="news-title">বাবুগঞ্জে নতুন সেতু উদ্বোধনের তাজা আপডেট</div>
            <div class="news-desc">সেতু সংক্রান্ত ফেসবুক পোস্টের বিস্তারিত তথ্য দেখতে নিচের লিংকে ক্লিক করুন।</div>
            <div class="news-link-box">
              🔗 মূল লিংক: <a href="https://facebook.com" target="_blank">https://facebook.com/posts/example123</a>
            </div>
            <div class="share-buttons">
              <button class="share-btn btn-fb" onclick="shareSocial('fb', 'https://facebook.com/posts/example123')">FB</button>
              <button class="share-btn btn-wa" onclick="shareSocial('wa', 'https://facebook.com/posts/example123')">WA</button>
              <button class="share-btn btn-copy" onclick="copyLink('https://facebook.com/posts/example123')">📋 কপি</button>
            </div>
          </div>
        </div>

        <!-- Default Post 2 -->
        <div class="news-card">
          <img src="https://picsum.photos/400/250?random=2" class="news-img" alt="নিউজ ছবি">
          <div class="news-content">
            <span class="news-tag">জাতীয়</span>
            <div class="news-title">ডিজিটাল প্রযুক্তিতে আরও এক ধাপ এগিয়ে বাংলাদেশ</div>
            <div class="news-desc">সারাদেশে হাই-স্পিড ইন্টারনেট পৌঁছে দিতে নতুন প্রকল্প হাতে নিয়েছে আইসিটি বিভাগ...</div>
            <div class="share-buttons">
              <button class="share-btn btn-fb" onclick="shareSocial('fb', window.location.href)">FB</button>
              <button class="share-btn btn-wa" onclick="shareSocial('wa', window.location.href)">WA</button>
              <button class="share-btn btn-copy" onclick="copyLink(window.location.href)">📋 কপি</button>
            </div>
          </div>
        </div>

      </div>
    </main>

    <!-- Right Sidebar (Post Upload Form & Ad Spots) -->
    <aside>
      <!-- Post Upload Section -->
      <div class="post-form-card">
        <h3>➕ সংবাদ পোস্ট ও লিংক যোগ করুন</h3>
        <form id="postForm" onsubmit="handlePostSubmit(event)">
          <div class="form-group">
            <label>সংবাদের শিরোনাম</label>
            <input type="text" id="postTitle" placeholder="শিরোনাম লিখুন..." required>
          </div>
          <div class="form-group">
            <label>ক্যাটাগরি</label>
            <select id="postCategory">
              <option value="বাবুগঞ্জ">বাবুগঞ্জ</option>
              <option value="ফেসবুক খবর">ফেসবুক খবর</option>
              <option value="জাতীয়">জাতীয়</option>
              <option value="রাজনীতি">রাজনীতি</option>
              <option value="খেলাধুলা">খেলাধুলা</option>
            </select>
          </div>
          
          <!-- External / Facebook Link Input -->
          <div class="form-group">
            <label>ফেসবুক বা খবরের লিংক (অপশনাল)</label>
            <input type="url" id="postExternalUrl" placeholder="https://facebook.com/post/...">
          </div>

          <div class="form-group">
            <label>ছবি (URL অথবা লোকাল ফাইল আপলোড)</label>
            <input type="file" id="postImageFile" accept="image/*" onchange="previewFileImage(this)">
            <input type="url" id="postImageUrl" placeholder="অথবা ছবির URL দিন..." style="margin-top: 6px;">
          </div>

          <div class="form-group">
            <label>সংবাদের বিবরণ</label>
            <textarea id="postDesc" rows="4" placeholder="বিস্তারিত লিখুন..." required></textarea>
          </div>

          <button type="submit" class="btn-submit">পাবলিশ করুন</button>
        </form>
      </div>

      <!-- Sidebar Adsterra Square Ad (300x250 বসানো হলো) -->
      <div class="ad-container ad-300x250">
        <script>
          atOptions = {
            'key' : '6b87b36dbcafdff41c2109cc4b9863e0',
            'format' : 'iframe',
            'height' : 250,
            'width' : 300,
            'params' : {}
          };
        </script>
        <script src="https://www.highrevenueformat.com/6b87b36dbcafdff41c2109cc4b9863e0/invoke.js"></script>
      </div>

    </aside>
  </div>

  <!-- পপআন্ডার / সোশ্যাল বার স্ক্রিপ্ট এখানে বসানো হলো -->
  <script src="https://pl32138751.profitableratecpmnetwork.com/23/9c/9f/239c9f7331d72f15bdcaae548e54c5f5.js"></script>

  <footer>
    <p>&copy; ২০২৬ বাবুগঞ্জ বার্তা | সর্বস্বত্ব সংরক্ষিত</p>
  </footer>

  <script>
    // 1. Dynamic Time Banner & Date Logic
    function updateHeaderInfo() {
      const now = new Date();
      const hour = now.getHours();
      
      const greetingHeader = document.getElementById('greetingHeader');
      const greetingText = document.getElementById('greetingText');

      if (hour >= 5 && hour < 12) {
        greetingText.innerHTML = "☀️ শুভ সকাল! বাবুগঞ্জ বার্তায় আপনাকে স্বাগতম।";
        greetingHeader.style.background = "linear-gradient(135deg, #f59e0b, #d97706)";
      } else if (hour >= 12 && hour < 16) {
        greetingText.innerHTML = "🌤️ শুভ দুপুর! আজকের দিনটি আপনার ভালো কাটুক।";
        greetingHeader.style.background = "linear-gradient(135deg, #0284c7, #0369a1)";
      } else if (hour >= 16 && hour < 19) {
        greetingText.innerHTML = "🌅 শুভ সন্ধ্যা! দিনের সেরা সংবাদগুলো পড়ুন।";
        greetingHeader.style.background = "linear-gradient(135deg, #ea580c, #c2410c)";
      } else {
        greetingText.innerHTML = "🌙 শুভ রাত্রি! রাতের তাজা খবর নিয়ে সাথেই থাকুন।";
        greetingHeader.style.background = "linear-gradient(135deg, #1e1b4b, #312e81)";
      }

      // Dates
      const engOptions = { weekday: 'long', year: 'numeric', month: 'long', day: 'numeric' };
      document.getElementById('engDate').innerText = now.toLocaleDateString('en-US', engOptions);

      const bngMonths = ["বৈশাখ", "জ্যৈষ্ঠ", "আষাঢ়", "শ্রাবণ", "ভাদ্র", "আশ্বিন", "কার্তিক", "অগ্রহায়ণ", "পৌষ", "মাঘ", "ফাল্গুন", "চৈত্র"];
      const bngNums = ['০','১','২','৩','৪','৫','৬','৭','৮','৯'];
      const toBngNum = num => num.toString().split('').map(d => bngNums[d] || d).join('');
      
      let bDay = now.getDate();
      let bMonthIdx = now.getMonth();
      let bYear = now.getFullYear() - 593;
      document.getElementById('bngDate').innerText = `${toBngNum(bDay)} ${bngMonths[bMonthIdx]}, ${toBngNum(bYear)} বঙ্গাব্দ`;

      try {
        const hijriFormatter = new Intl.DateTimeFormat('bn-BD-u-ca-islamic-umalqura', {
          day: 'numeric', month: 'long', year: 'numeric'
        });
        document.getElementById('hijriDate').innerText = hijriFormatter.format(now) + " হিজরী";
      } catch (e) {
        document.getElementById('hijriDate').innerText = "হিজরী তারিখ...";
      }
    }

    // 2. Live TV Switching Logic
    const tvChannels = {
      jamuna: "https://www.youtube.com/embed/live_stream?channel=UCjH5l0jR3F-Wq8CjT5B4Xsw",
      dbc: "https://www.youtube.com/embed/live_stream?channel=UCp04-lI-mFj9Vn8Dk9D5uJg",
      somoy: "https://www.youtube.com/embed/live_stream?channel=UC4g3W4D2oK3uH7C77E5zTew"
    };

    function changeChannel(channelKey, btnElement) {
      document.getElementById('tvIframe').src = tvChannels[channelKey] || tvChannels.jamuna;
      document.querySelectorAll('.tv-btn').forEach(b => b.classList.remove('active'));
      btnElement.classList.add('active');
    }

    // 3. News Posting with Link Feature
    let uploadedImageBase64 = "";

    function previewFileImage(input) {
      if (input.files && input.files[0]) {
        const reader = new FileReader();
        reader.onload = function(e) {
          uploadedImageBase64 = e.target.result;
        }
        reader.readAsDataURL(input.files[0]);
      }
    }

    function handlePostSubmit(event) {
      event.preventDefault();

      const title = document.getElementById('postTitle').value;
      const category = document.getElementById('postCategory').value;
      const desc = document.getElementById('postDesc').value;
      const externalUrl = document.getElementById('postExternalUrl').value;
      const imageUrlInput = document.getElementById('postImageUrl').value;

      let finalImgSrc = uploadedImageBase64 || imageUrlInput || "https://picsum.photos/400/250?random=" + Math.floor(Math.random() * 100);

      let linkHtml = "";
      let targetLink = externalUrl || window.location.href;

      if (externalUrl) {
        linkHtml = `
          <div class="news-link-box">
            🔗 মূল লিংক: <a href="${externalUrl}" target="_blank" rel="noopener noreferrer">${externalUrl}</a>
          </div>
        `;
      }

      const newCard = document.createElement('div');
      newCard.className = 'news-card';
      newCard.innerHTML = `
        <img src="${finalImgSrc}" class="news-img" alt="নিউজ ছবি">
        <div class="news-content">
          <span class="news-tag">${category}</span>
          <div class="news-title">${title}</div>
          <div class="news-desc">${desc}</div>
          ${linkHtml}
          <div class="share-buttons">
            <button class="share-btn btn-fb" onclick="shareSocial('fb', '${targetLink}')">FB</button>
            <button class="share-btn btn-wa" onclick="shareSocial('wa', '${targetLink}')">WA</button>
            <button class="share-btn btn-copy" onclick="copyLink('${targetLink}')">📋 কপি</button>
          </div>
        </div>
      `;

      const grid = document.getElementById('newsGrid');
      grid.insertBefore(newCard, grid.firstChild);

      document.getElementById('postForm').reset();
      uploadedImageBase64 = "";
      alert("সংবাদটি সফলভাবে লিংক সহ প্রকাশিত হয়েছে!");
    }

    // 4. Link Copy & Sharing Options
    function copyLink(link) {
      navigator.clipboard.writeText(link).then(() => {
        alert("লিংকটি কপি করা হয়েছে:\n" + link);
      }).catch(() => {
        prompt("কপি করতে নিচের লিংকটি সিলেক্ট করুন:", link);
      });
    }

    function shareSocial(platform, link) {
      const url = encodeURIComponent(link);

      if (platform === 'fb') {
        window.open(`https://www.facebook.com/sharer/sharer.php?u=${url}`, '_blank');
      } else if (platform === 'wa') {
        window.open(`https://api.whatsapp.com/send?text=${url}`, '_blank');
      }
    }

    // Initialize Page
    updateHeaderInfo();
  </script>
</body>
</html>
