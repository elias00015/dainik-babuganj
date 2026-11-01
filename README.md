<!DOCTYPE html>
<html lang="bn">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>দৈনিক বাবুগঞ্জ - অনলাইন নিউজ পোর্টাল</title>
    
    <!-- ফেসবুক SDK -->
    <div id="fb-root"></div>
    <script async defer crossorigin="anonymous" src="https://connect.facebook.net/bn_IN/sdk.js#xfbml=1&version=v18.0"></script>
    
    <!-- ================================================= -->
    <!-- ১. Popunder Ad Code (এখানে Popunder কোড বসান) -->
    <!-- ================================================= -->
    <!-- Popunder script starts here -->

    <!-- Popunder script ends here -->

    <!-- ================================================= -->
    <!-- ২. Social Bar Ad Code (এখানে Social Bar কোড বসান) -->
    <!-- ================================================= -->
    <!-- Social Bar script starts here -->

    <!-- Social Bar script ends here -->

    <style>
        * { box-sizing: border-box; margin: 0; padding: 0; font-family: 'SolaimanLipi', Arial, sans-serif; }
        body { background-color: #f0f2f5; color: #333; line-height: 1.6; }
        
        header { background: linear-gradient(135deg, #b30000, #800000); color: #fff; padding: 20px; text-align: center; box-shadow: 0 4px 10px rgba(0,0,0,0.15); }
        header h1 { font-size: 32px; margin-bottom: 5px; font-weight: bold; letter-spacing: 1px; }
        header p { font-size: 15px; opacity: 0.9; }
        .date-time { font-size: 13px; background: rgba(0,0,0,0.2); display: inline-block; padding: 5px 15px; border-radius: 20px; margin-top: 10px; border: 1px solid rgba(255,255,255,0.1); }

        .container { max-width: 900px; margin: 25px auto; padding: 0 15px; }
        .main-layout { display: flex; flex-wrap: wrap; gap: 20px; }
        .content-area { flex: 1; min-width: 280px; }
        .sidebar { width: 180px; min-width: 160px; }

        @media (max-width: 768px) {
            .sidebar { width: 100%; }
        }

        .card { background: #fff; padding: 22px; border-radius: 10px; box-shadow: 0 2px 8px rgba(0,0,0,0.06); margin-bottom: 20px; border-top: 4px solid #b30000; }
        .card h3 { color: #b30000; margin-bottom: 15px; font-size: 19px; border-bottom: 2px solid #f0f2f5; padding-bottom: 8px; display: flex; align-items: center; gap: 8px; }

        input, textarea { width: 100%; padding: 12px; margin-bottom: 14px; border: 1px solid #ddd; border-radius: 6px; font-size: 15px; background: #fafafa; transition: all 0.3s ease; }
        input:focus, textarea:focus { border-color: #b30000; background: #fff; outline: none; box-shadow: 0 0 5px rgba(179, 0, 0, 0.2); }
        button, .smartlink-btn { background: #b30000; color: #fff; border: none; padding: 12px 20px; font-size: 16px; border-radius: 6px; cursor: pointer; width: 100%; font-weight: bold; text-align: center; display: inline-block; text-decoration: none; box-sizing: border-box; }
        button:hover, .smartlink-btn:hover { background: #900; }

        .news-item { border-bottom: 1px solid #eee; padding: 15px 0; }
        .news-item:last-child { border-bottom: none; }
        .news-item h4 { color: #111; font-size: 18px; margin-bottom: 6px; }
        .news-item a { color: #b30000; text-decoration: none; font-weight: bold; }
        .news-item a:hover { text-decoration: underline; }
        .news-time { font-size: 12px; color: #887; margin-bottom: 8px; font-style: italic; }
        .news-item p { color: #444; font-size: 15px; }

        .ad-box { background: #fff; border: 2px dashed #b30000; padding: 15px; text-align: center; color: #b30000; margin: 15px 0; border-radius: 8px; font-size: 13px; font-weight: bold; box-shadow: 0 2px 5px rgba(0,0,0,0.03); word-break: break-all; }
        .fb-post-wrapper { text-align: center; margin-top: 15px; overflow-x: auto; }

        footer { text-align: center; padding: 20px; background: #1a1a1a; color: #fff; font-size: 14px; margin-top: 40px; box-shadow: inset 0 3px 5px rgba(0,0,0,0.2); }
    </style>
</head>
<body>

    <header>
        <h1>দৈনিক বাবুগঞ্জ</h1>
        <p>সত্য ও বস্তুনিষ্ঠ সংবাদ প্রকাশে অঙ্গীকারাবদ্ধ</p>
        <div class="date-time" id="liveDateTime">লোড হচ্ছে...</div>
    </header>

    <div class="container">

        <!-- ৩. Banner 728x90 (হেডার ব্যানার) -->
        <div class="ad-box">
            [ Adsterra Banner 728x90: এখানে কোড বসান ]
        </div>

        <!-- ৪. Banner 320x50 (মোবাইল ব্যানার) -->
        <div class="ad-box">
            [ Adsterra Banner 320x50: এখানে কোড বসান ]
        </div>

        <div class="main-layout">
            
            <div class="content-area">

                <!-- ৫. Native Banner (নেটিভ ব্যানার) -->
                <div class="ad-box" style="border-color: #28a745; color: #28a745;">
                    [ Adsterra Native Banner: এখানে কোড বসান ]
                </div>

                <!-- ফেসবুক পোস্ট এম্বেড ফর্ম -->
                <div class="card">
                    <h3>🌐 ফেসবুক পোস্ট যুক্ত করুন</h3>
                    <input type="text" id="fbPostUrl" placeholder="ফেসবুক পোস্টের লিংক এখানে পেস্ট করুন (https://facebook.com/...)">
                    <button onclick="embedFacebookPost()">পোস্ট যুক্ত করুন</button>
                    <div id="fbPostDisplay" class="fb-post-wrapper"></div>
                </div>

                <!-- ৬. Banner 468x60 (মাঝারি ব্যানার) -->
                <div class="ad-box">
                    [ Adsterra Banner 468x60: এখানে কোড বসান ]
                </div>

                <!-- সংবাদ প্রকাশের ফর্ম -->
                <div class="card">
                    <h3>✍️ নতুন সংবাদ প্রকাশ করুন</h3>
                    <input type="text" id="newsTitle" placeholder="খবরের শিরোনাম এখানে লিখুন...">
                    <textarea id="newsContent" rows="4" placeholder="খবরের বিস্তারিত বিবরণ এখানে লিখুন..."></textarea>
                    <button onclick="publishNews()">প্রকাশ করুন</button>
                </div>

                <!-- ৭. Smartlink (স্মার্টলিঙ্ক বাটন) -->
                <div class="card" style="text-align: center; background: #fff8e1; border-top-color: #ff9800;">
                    <h3>🔥 বিশেষ অফার / এক্সক্লুসিভ নিউজ</h3>
                    <p style="margin-bottom: 10px; font-size: 14px;">সর্বশেষ আপডেট দেখতে নিচের বাটনে ক্লিক করুন:</p>
                    <a href="YOUR_SMARTLINK_URL_HERE" target="_blank" class="smartlink-btn">এখানে ক্লিক করুন (Smartlink)</a>
                </div>

                <!-- আন্তর্জাতিক সংবাদ -->
                <div class="card">
                    <h3>🌍 স্বয়ংক্রিয় আন্তর্জাতিক সংবাদ (BBC World)</h3>
                    <div id="intlNewsFeed">
                        <p style="color: #666; text-align: center; padding: 10px;">আন্তর্জাতিক সংবাদ লোড হচ্ছে...</p>
                    </div>
                </div>

                <!-- সর্বশেষ সংবাদ ফিড -->
                <div class="card">
                    <h3>📢 সর্বশেষ নিজস্ব সংবাদ ফিড</h3>
                    <div id="newsFeed">
                        <p style="color: #666; text-align: center; padding: 10px;">এখনও কোনো নতুন পোস্ট করা হয়নি। উপরের ফরম থেকে পোস্ট করুন।</p>
                    </div>
                </div>

            </div>

            <!-- সাইডবার -->
            <div class="sidebar">
                <!-- ৮. Banner 300x250 (স্কয়ার ব্যানার) -->
                <div class="ad-box" style="min-height: 250px;">
                    [ Adsterra Banner 300x250: এখানে কোড বসান ]
                </div>
            </div>

        </div>

    </div>

    <footer>
        <p>&copy; ২০২৬ দৈনিক বাবুগঞ্জ - সর্বস্বত্ব সংরক্ষিত</p>
    </footer>

    <script>
        function updateDateTime() {
            const now = new Date();
            const options = { year: 'numeric', month: 'long', day: 'numeric', weekday: 'long', hour: '2-digit', minute: '2-digit', second: '2-digit' };
            document.getElementById('liveDateTime').innerText = now.toLocaleDateString('bn-BD', options);
        }
        setInterval(updateDateTime, 1000);
        updateDateTime();

        function embedFacebookPost() {
            const url = document.getElementById('fbPostUrl').value.trim();
            if(!url) {
                alert('দয়া করে একটি সঠিক ফেসবুক পোস্টের লিংক দিন!');
                return;
            }
            const displayArea = document.getElementById('fbPostDisplay');
            displayArea.innerHTML = `<div class="fb-post" data-href="${url}" data-width="500"></div>`;
            if (window.FB) {
                FB.XFBML.parse(displayArea);
            }
            alert('ফেসবুক পোস্টটি যুক্ত করা হয়েছে!');
        }

        function fetchIntlNews() {
            const feedContainer = document.getElementById('intlNewsFeed');
            const rssUrl = 'https://feeds.bbci.co.uk/news/world/rss.xml';
            const apiUrl = `https://api.rss2json.com/v1/api.json?rss_url=${encodeURIComponent(rssUrl)}`;

            fetch(apiUrl)
                .then(res => res.json())
                .then(data => {
                    if (data.status === 'ok') {
                        let html = '';
                        data.items.slice(0, 5).forEach(item => {
                            html += `
                                <div class="news-item">
                                    <h4><a href="${item.link}" target="_blank">${item.title}</a></h4>
                                    <div class="news-time">প্রকাশিত: ${new Date(item.pubDate).toLocaleString('bn-BD')}</div>
                                    <p>${item.description}</p>
                                </div>
                            `;
                        });
                        feedContainer.innerHTML = html;
                    } else {
                        feedContainer.innerHTML = '<p style="color:red; text-align:center;">আন্তর্জাতিক সংবাদ লোড করা সম্ভব হয়নি।</p>';
                    }
                })
                .catch(() => {
                    feedContainer.innerHTML = '<p style="color:red; text-align:center;">সংবাদ লোড করতে সমস্যা হয়েছে।</p>';
                });
        }

        window.onload = function() {
            loadNews();
            fetchIntlNews();
        };

        function publishNews() {
            const title = document.getElementById('newsTitle').value.trim();
            const content = document.getElementById('newsContent').value.trim();

            if(!title || !content) {
                alert('দয়া করে খবরের শিরোনাম এবং বিস্তারিত উভয়ই লিখুন!');
                return;
            }

            const newsItem = {
                title: title,
                content: content,
                date: new Date().toLocaleString('bn-BD')
            };

            let allNews = JSON.parse(localStorage.getItem('dainik_babuganj_news')) || [];
            allNews.unshift(newsItem);
            localStorage.setItem('dainik_babuganj_news', JSON.stringify(allNews));

            document.getElementById('newsTitle').value = '';
            document.getElementById('newsContent').value = '';

            loadNews();
            alert('সংবাদটি সফলভাবে প্রকাশিত হয়েছে!');
        }

        function loadNews() {
            const feed = document.getElementById('newsFeed');
            let allNews = JSON.parse(localStorage.getItem('dainik_babuganj_news')) || [];

            if(allNews.length === 0) {
                feed.innerHTML = '<p style="color: #666; text-align: center; padding: 10px;">এখনও কোনো নতুন পোস্ট করা হয়নি। উপরের ফরম থেকে পোস্ট করুন।</p>';
                return;
            }

            let html = '';
            allNews.forEach(item => {
                html += `
                    <div class="news-item">
                        <h4>${item.title}</h4>
                        <div class="news-time">প্রকাশিত: ${item.date}</div>
                        <p>${item.content}</p>
                    </div>
                `;
            });
            feed.innerHTML = html;
        }
    </script>
</body>
</html>
