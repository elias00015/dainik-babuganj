<!DOCTYPE html>
<html lang="bn">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>দৈনিক বাবুগঞ্জ - অনলাইন নিউজ পোর্টাল</title>
    <style>
        * { box-sizing: border-box; margin: 0; padding: 0; font-family: 'SolaimanLipi', Arial, sans-serif; }
        body { background-color: #f4f7f6; color: #333; line-height: 1.6; }
        header { background: #b30000; color: #fff; padding: 15px 0; box-shadow: 0 2px 5px rgba(0,0,0,0.1); }
        .container { width: 90%; max-width: 1200px; margin: auto; overflow: hidden; }
        .header-flex { display: flex; justify-content: space-between; align-items: center; flex-wrap: wrap; }
        .logo h1 { font-size: 28px; font-weight: bold; }
        .logo p { font-size: 13px; opacity: 0.9; }
        nav { background: #990000; padding: 10px 0; }
        nav ul { display: flex; list-style: none; justify-content: center; flex-wrap: wrap; }
        nav ul li { margin: 0 15px; }
        nav ul li a { color: #fff; text-decoration: none; font-size: 16px; font-weight: bold; transition: 0.3s; }
        nav ul li a:hover { color: #ffeb3b; }
        .ticker-bar { background: #fff3cd; color: #856404; padding: 10px; border-bottom: 1px solid #ffeeba; display: flex; align-items: center; }
        .ticker-title { background: #b30000; color: #fff; padding: 3px 10px; font-size: 14px; font-weight: bold; margin-right: 15px; border-radius: 3px; }
        .main-content { display: flex; flex-wrap: wrap; margin: 20px 0; gap: 20px; }
        .news-section { flex: 3; min-width: 300px; }
        .sidebar { flex: 1; min-width: 280px; }
        .card { background: #fff; padding: 20px; margin-bottom: 20px; border-radius: 5px; box-shadow: 0 2px 4px rgba(0,0,0,0.05); }
        .card h3 { border-bottom: 2px solid #b30000; padding-bottom: 8px; margin-bottom: 15px; color: #b30000; font-size: 18px; }
        .post-form input, .post-form select, .post-form textarea { width: 100%; padding: 10px; margin-bottom: 12px; border: 1px solid #ccc; border-radius: 4px; }
        .post-form button { background: #b30000; color: #fff; border: none; padding: 10px 20px; font-size: 16px; cursor: pointer; border-radius: 4px; font-weight: bold; }
        .post-form button:hover { background: #990000; }
        .ad-box { background: #e9ecef; border: 2px dashed #adb5bd; color: #6c757d; text-align: center; padding: 20px; margin: 20px 0; border-radius: 5px; font-size: 14px; }
        .social-bar-fixed { position: fixed; bottom: 0; left: 0; width: 100%; background: #222; color: #fff; text-align: center; padding: 8px; z-index: 999; font-size: 13px; }
        .calendar-box { background: #fff; padding: 15px; border-radius: 5px; text-align: center; margin-bottom: 20px; box-shadow: 0 2px 4px rgba(0,0,0,0.05); border-top: 4px solid #b30000; }
        .greeting-box { background: #e3f2fd; color: #0d47a1; padding: 12px; border-radius: 5px; text-align: center; font-weight: bold; margin-bottom: 20px; border: 1px solid #bbdefb; }
        .photocard-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 15px; }
        .photocard { background: #fff; border: 1px solid #ddd; border-radius: 6px; overflow: hidden; box-shadow: 0 2px 4px rgba(0,0,0,0.05); }
        .photocard img { width: 100%; height: 160px; object-fit: cover; }
        .photocard-body { padding: 12px; }
        .photocard-body h4 { font-size: 15px; margin-bottom: 8px; color: #222; }
        .share-btn { display: inline-block; background: #3b5998; color: #fff; padding: 5px 10px; text-decoration: none; font-size: 12px; border-radius: 3px; margin-top: 8px; }
        footer { background: #222; color: #fff; text-align: center; padding: 20px 0; margin-top: 40px; margin-bottom: 40px; }
    </style>
</head>
<body>

    <header>
        <div class="container header-flex">
            <div class="logo">
                <h1>দৈনিক বাবুগঞ্জ</h1>
                <p>সত্যের সাথে, জনগণের সাথে</p>
            </div>
            <div>
                <a href="#postSection" style="background:#fff; color:#b30000; padding:8px 15px; text-decoration:none; font-weight:bold; border-radius:4px;">✍️ পোষ্ট করুন (আফরিন)</a>
            </div>
        </div>
    </header>

    <nav>
        <ul>
            <li><a href="#">প্রচ্ছদ</a></li>
            <li><a href="#">জাতীয়</a></li>
            <li><a href="#">রাজনীতি</a></li>
            <li><a href="#">অর্থনীতি</a></li>
            <li><a href="#">খেলাধুলা</a></li>
            <li><a href="#">বিনোদন</a></li>
            <li><a href="#postSection">পোষ্ট করুন</a></li>
        </ul>
    </nav>

    <div class="container">
        <div class="ticker-bar">
            <div class="ticker-title">ব্রেকিং নিউজ</div>
            <marquee behavior="scroll" direction="left">দৈনিক বাবুগঞ্জ নিউজ পোর্টালে আপনাকে স্বাগতম! নিয়মিত আপডেট পেতে সাথেই থাকুন।</marquee>
        </div>

        <div class="main-content">
            <div class="news-section">
                <div id="greetingBanner" class="greeting-box">শুভ সকাল! আজকের দিনটি আপনার ভালো কাটুক।</div>

                <div class="calendar-box">
                    <h4 style="color: #b30000; margin-bottom: 5px;">📅 আজকের তারিখ ও পঞ্জিকা</h4>
                    <p id="fullDateDisplay" style="font-size: 16px; font-weight: bold; color: #333;">লোড হচ্ছে...</p>
                </div>

                <div class="ad-box">
                    [ Adsterra Native Banner Ad Space ]<br>
                    <small>এখানে আপনার অ্যাডস্টেরা নেটিভ ব্যানার কোড বসান</small>
                </div>

                <div class="card">
                    <h3>📺 টিভি চ্যানেল ফটোকার্ড ফিড (যমুনা, আরটিভি, নিউজ ২৪)</h3>
                    <div class="photocard-grid">
                        <div class="photocard">
                            <img src="https://picsum.photos/300/160?random=1" alt="Jamuna TV">
                            <div class="photocard-body">
                                <small style="color: #b30000; font-weight: bold;">যমুনা টেলিভিশন</small>
                                <h4>প্রধান উপদেষ্টার সাথে রাজনৈতিক দলগুলোর গুরুত্বপূর্ণ বৈঠক সমাপ্ত।</h4>
                                <a href="https://www.facebook.com/sharer/sharer.php?u=#" target="_blank" class="share-btn">ফটোকার্ড শেয়ার করুন</a>
                            </div>
                        </div>
                        <div class="photocard">
                            <img src="https://picsum.photos/300/160?random=2" alt="RTV">
                            <div class="photocard-body">
                                <small style="color: #b30000; font-weight: bold;">আরটিভি নিউজ</small>
                                <h4>দেশের বাজারে স্বর্ণের নতুন দাম নির্ধারণ, ভরি কত হলো জানুন।</h4>
                                <a href="https://www.facebook.com/sharer/sharer.php?u=#" target="_blank" class="share-btn">ফটোকার্ড শেয়ার করুন</a>
                            </div>
                        </div>
                        <div class="photocard">
                            <img src="https://picsum.photos/300/160?random=3" alt="News24">
                            <div class="photocard-body">
                                <small style="color: #b30000; font-weight: bold;">নিউজ টোয়েন্টি ফোর</small>
                                <h4>আসছে শীতের আমেজ, দেশের বিভিন্ন অঞ্চলে হালকা কুয়াশার পূর্বাভাস।</h4>
                                <a href="https://www.facebook.com/sharer/sharer.php?u=#" target="_blank" class="share-btn">ফটোকার্ড শেয়ার করুন</a>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="card" id="postSection">
                    <h3>✍️ নতুন সংবাদ পোস্ট করুন (আফরিন)</h3>
                    <form class="post-form" onsubmit="handlePost(event)">
                        <input type="text" id="newsTitle" placeholder="খবরের শিরোনাম লিখুন..." required>
                        <select id="newsCat">
                            <option value="জাতীয়">জাতীয়</option>
                            <option value="রাজনীতি">রাজনীতি</option>
                            <option value="অর্থনীতি">অর্থনীতি</option>
                            <option value="খেলাধুলা">খেলাধুলা</option>
                            <option value="বিনোদন">বিনোদন</option>
                        </select>
                        <input type="text" id="newsImage" placeholder="ছবির লিংক (URL) দিন..." required>
                        <textarea id="newsDesc" rows="4" placeholder="খবরের বিস্তারিত বিবরণ এখানে লিখুন..." required></textarea>
                        <button type="submit">প্রকাশ করুন</button>
                    </form>
                </div>

                <div class="card">
                    <h3>📢 সর্বশেষ সংবাদ ফিড</h3>
                    <div id="liveNewsFeed">
                        <p style="color: #666; font-size: 14px;">এখনও কোনো নতুন পোস্ট করা হয়নি। উপরের ফরম থেকে পোস্ট করুন।</p>
                    </div>
                </div>
            </div>

            <div class="sidebar">
                <div class="card">
                    <h3>বিজ্ঞাপন (Adsterra 300x250)</h3>
                    <div class="ad-box" style="margin: 0; padding: 40px 10px;">
                        [ Adsterra Banner Ad ]
                    </div>
                </div>

                <div class="card">
                    <h3>জনপ্রিয় সংবাদ</h3>
                    <ul style="padding-left: 20px; font-size: 14px;">
                        <li style="margin-bottom: 10px;"><a href="#" style="color:#333; text-decoration:none;">বাবুগঞ্জে নতুন রাস্তা নির্মাণ কাজের উদ্বোধন করলেন স্থানীয় প্রশাসন।</a></li>
                        <li style="margin-bottom: 10px;"><a href="#" style="color:#333; text-decoration:none;">কৃষি প্রণোদনা পাচ্ছেন বাবুগঞ্জের শত শত প্রান্তিক কৃষক।</a></li>
                        <li style="margin-bottom: 10px;"><a href="#" style="color:#333; text-decoration:none;">বরিশাল বিভাগে শীতের আগমনী বার্তা, রাতের তাপমাত্রা কমল।</a></li>
                    </ul>
                </div>
            </div>
        </div>
    </div>

    <div class="social-bar-fixed">
        [ Adsterra Social Bar Ad Space - এখানে কোড পেস্ট করুন ]
    </div>

    <footer>
        <p>&copy; ২০২৬ দৈনিক বাবুগঞ্জ - সর্বস্বত্ব সংরক্ষিত।</p>
    </footer>

    <script>
        function updateDateTimeAndGreetings() {
            const now = new Date();
            const hours = now.getHours();
            
            let greetingText = "";
            if (hours >= 5 && hours < 12) {
                greetingText = "☀️ শুভ সকাল! আজকের দিনটি আপনার সুন্দর কাটুক।";
            } else if (hours >= 12 && hours < 17) {
                greetingText = "🌤️ শুভ দুপুর! আপনার সময়টি আনন্দদায়ক হোক।";
            } else if (hours >= 17 && hours < 21) {
                greetingText = "🌇 শুভ সন্ধ্যা! আপনার সন্ধ্যাটি শুভ হোক।";
            } else {
                greetingText = "🌙 শুভ রাত্রি!";
            }
            document.getElementById('greetingBanner').innerText = greetingText;

            const options = { year: 'numeric', month: 'long', day: 'numeric', weekday: 'long' };
            const engDate = now.toLocaleDateString('bn-BD', options);
            
            document.getElementById('fullDateDisplay').innerHTML = `ইংরেজি: ${engDate} <br> বাংলা মাস: কার্তিক ১৪৩৩ <br> হিজরী: রবিউস সানি ১৪৪৮ হি.`;
        }

        updateDateTimeAndGreetings();

        function handlePost(e) {
            e.preventDefault();
            const title = document.getElementById('newsTitle').value;
            const cat = document.getElementById('newsCat').value;
            const img = document.getElementById('newsImage').value;
            const desc = document.getElementById('newsDesc').value;

            const feedContainer = document.getElementById('liveNewsFeed');
            
            const newPostHTML = `
                <div style="border-bottom: 1px solid #eee; padding-bottom: 15px; margin-bottom: 15px;">
                    <span style="background: #b30000; color: #fff; padding: 2px 8px; font-size: 12px; border-radius: 3px;">${cat}</span>
                    <h4 style="margin: 8px 0; color: #222;">${title}</h4>
                    <img src="${img}" alt="News Image" style="width: 100%; max-height: 200px; object-fit: cover; border-radius: 4px; margin-bottom: 8px;">
                    <p style="font-size: 14px; color: #555;">${desc}</p>
                    <small style="color: #999;">মাত্র প্রকাশ করা হলো (আফরিন)</small>
                </div>
            `;

            feedContainer.insertAdjacentHTML('afterbegin', newPostHTML);
            alert('সফলভাবে সংবাদ পোস্ট করা হয়েছে!');
            document.getElementById('postSection').querySelector('form').reset();
        }
    </script>
</body>
</html>
