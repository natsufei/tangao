<!DOCTYPE html>
<html lang="zh-TW">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cambridge Young Learners English Tests:Starters(Qrcode版)_TA0045 YLE - Cambridge YLE | 堂奧圖書</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Noto+Serif+TC:wght@400;500;600;700&family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Inter', sans-serif;
            color: #333;
            line-height: 1.6;
            background: #f9f9f9;
        }

        /* Header */
        header {
            background: white;
            box-shadow: 0 1px 3px rgba(0,0,0,0.1);
            position: sticky;
            top: 0;
            z-index: 100;
        }

        .header-top {
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 1rem 0;
            max-width: 1400px;
            margin: 0 auto;
            padding-left: 1rem;
            padding-right: 1rem;
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 0.5rem;
            font-size: 1.25rem;
            font-weight: bold;
            color: #E84A2B;
            font-family: 'Noto Serif TC', serif;
            text-decoration: none;
        }

        .logo-icon {
            width: 2rem;
            height: 2rem;
            background: #E84A2B;
            border-radius: 0.4rem;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 1.2rem;
        }

        .nav-menu {
            display: flex;
            gap: 2rem;
            list-style: none;
        }

        .nav-menu a {
            text-decoration: none;
            color: #666;
            font-size: 0.9rem;
            transition: color 0.3s;
        }

        .nav-menu a:hover {
            color: #E84A2B;
        }

        .header-actions {
            display: flex;
            gap: 1rem;
            align-items: center;
        }

        .search-box {
            display: flex;
            align-items: center;
            background: #f5f5f5;
            border-radius: 2rem;
            padding: 0.5rem 1rem;
            width: 250px;
            border: 2px dashed #ddd;
        }

        .search-box input {
            border: none;
            background: transparent;
            width: 100%;
            font-size: 0.9rem;
            outline: none;
        }

        .search-box button {
            background: none;
            border: none;
            cursor: pointer;
            color: #999;
            font-size: 1rem;
        }

        .cart-icon {
            position: relative;
            cursor: pointer;
            font-size: 1.2rem;
            text-decoration: none;
            color: #333;
        }

        .cart-badge {
            position: absolute;
            top: -0.5rem;
            right: -0.5rem;
            background: #E84A2B;
            color: white;
            width: 1.2rem;
            height: 1.2rem;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 0.7rem;
            font-weight: bold;
        }

        .nav-secondary {
            background: #E84A2B;
            padding: 0.5rem 0;
        }

        .nav-secondary-content {
            max-width: 1400px;
            margin: 0 auto;
            padding: 0 1rem;
            display: flex;
            gap: 0;
        }

        .nav-secondary a {
            color: white;
            text-decoration: none;
            font-size: 0.8rem;
            padding: 0.5rem 1rem;
            display: inline-block;
            transition: background 0.3s;
        }

        .nav-secondary a:hover {
            background: rgba(0,0,0,0.1);
        }

        .menu-toggle {
            display: none;
            background: none;
            border: none;
            font-size: 1.5rem;
            cursor: pointer;
        }

        /* Breadcrumb */
        .breadcrumb {
            max-width: 1400px;
            margin: 0 auto;
            padding: 1rem;
            font-size: 0.85rem;
            color: #666;
        }

        .breadcrumb a {
            color: #E84A2B;
            text-decoration: none;
        }

        .breadcrumb a:hover {
            text-decoration: underline;
        }

        /* Main content */
        .main-container {
            max-width: 1400px;
            margin: 2rem auto;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 2rem;
            padding: 0 1rem;
            background: white;
            border-radius: 0.5rem;
            padding: 2rem;
        }

        /* Product image */
        .product-image-section {
            display: flex;
            flex-direction: column;
            gap: 1rem;
        }

        .product-main-image {
            width: 100%;
            aspect-ratio: 3/4;
            background: linear-gradient(135deg, #f5a623 0%, #E84A2B 100%);
            border-radius: 0.5rem;
            overflow: hidden;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 5rem;
            position: relative;
        }

        .product-main-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .mp3-badge {
            position: absolute;
            top: 1rem;
            right: 1rem;
            background: white;
            padding: 0.5rem 1rem;
            border-radius: 0.3rem;
            font-size: 0.8rem;
            font-weight: 600;
            box-shadow: 0 2px 8px rgba(0,0,0,0.1);
        }

        .image-thumbnails {
            display: grid;
            grid-template-columns: repeat(5, 1fr);
            gap: 0.5rem;
        }

        .thumbnail {
            aspect-ratio: 1;
            background: #f5f5f5;
            border: 2px solid #ddd;
            border-radius: 0.3rem;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5rem;
            transition: all 0.3s;
        }

        .thumbnail:hover,
        .thumbnail.active {
            border-color: #E84A2B;
            background: #fff5f0;
        }

        /* Product info */
        .product-info-section {
            display: flex;
            flex-direction: column;
            gap: 1.5rem;
        }

        .product-header {
            border-bottom: 2px solid #eee;
            padding-bottom: 1rem;
        }

        .product-isbn {
            font-size: 0.85rem;
            color: #999;
            margin-bottom: 0.5rem;
        }

        .product-title {
            font-size: 1.5rem;
            font-family: 'Noto Serif TC', serif;
            font-weight: 600;
            margin-bottom: 1rem;
            line-height: 1.4;
        }

        .product-price {
            display: flex;
            align-items: baseline;
            gap: 1rem;
            margin-bottom: 1rem;
        }

        .price-current {
            font-size: 2rem;
            font-weight: 700;
            color: #E84A2B;
        }

        .price-original {
            font-size: 1rem;
            color: #999;
            text-decoration: line-through;
        }

        .product-share {
            display: flex;
            gap: 1rem;
            align-items: center;
            margin-top: 1rem;
        }

        .share-label {
            font-size: 0.9rem;
            color: #666;
        }

        .share-btn {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 2.5rem;
            height: 2.5rem;
            border-radius: 50%;
            background: #f5f5f5;
            border: 1px solid #ddd;
            cursor: pointer;
            font-size: 1.2rem;
            transition: all 0.3s;
            text-decoration: none;
        }

        .share-btn:hover {
            background: #E84A2B;
            color: white;
            border-color: #E84A2B;
        }

        /* Specs table */
        .specs-table {
            width: 100%;
            border-collapse: collapse;
            font-size: 0.9rem;
        }

        .specs-table tr {
            border-bottom: 1px solid #eee;
        }

        .specs-table td {
            padding: 0.75rem 0;
        }

        .specs-table td:first-child {
            font-weight: 600;
            color: #666;
            width: 30%;
        }

        .specs-table td:last-child {
            color: #333;
        }

        /* Purchase section */
        .purchase-section {
            border: 2px dashed #E84A2B;
            padding: 1.5rem;
            border-radius: 0.5rem;
            background: #fff5f0;
        }

        .quantity-selector {
            display: flex;
            align-items: center;
            gap: 1rem;
            margin-bottom: 1rem;
        }

        .quantity-selector label {
            font-weight: 600;
            color: #333;
        }

        .quantity-selector select {
            padding: 0.5rem 1rem;
            border: 1px solid #ddd;
            border-radius: 0.3rem;
            font-size: 0.9rem;
            cursor: pointer;
        }

        .purchase-buttons {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 1rem;
        }

        .btn {
            padding: 0.8rem;
            border: none;
            border-radius: 0.4rem;
            font-size: 0.95rem;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s;
            text-decoration: none;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 0.5rem;
        }

        .btn-primary {
            background: #E84A2B;
            color: white;
        }

        .btn-primary:hover {
            background: #d63d1f;
        }

        .btn-secondary {
            background: white;
            color: #E84A2B;
            border: 2px solid #E84A2B;
        }

        .btn-secondary:hover {
            background: #fff5f0;
        }

        /* Tabs */
        .tabs-container {
            margin-top: 2rem;
            border-top: 2px solid #eee;
            padding-top: 2rem;
        }

        .tabs-header {
            display: flex;
            gap: 0;
            border-bottom: 2px solid #eee;
            margin-bottom: 2rem;
        }

        .tab-btn {
            padding: 1rem 1.5rem;
            background: none;
            border: none;
            cursor: pointer;
            font-size: 0.95rem;
            font-weight: 600;
            color: #666;
            border-bottom: 3px solid transparent;
            transition: all 0.3s;
            position: relative;
            bottom: -2px;
        }

        .tab-btn:hover {
            color: #E84A2B;
        }

        .tab-btn.active {
            color: #E84A2B;
            border-bottom-color: #E84A2B;
        }

        .tab-content {
            display: none;
        }

        .tab-content.active {
            display: block;
        }

        .tab-content h3 {
            font-size: 1.1rem;
            margin-bottom: 1rem;
            color: #333;
        }

        .tab-content p {
            margin-bottom: 1rem;
            line-height: 1.8;
            color: #666;
        }

        .tab-content ul {
            margin-left: 1.5rem;
            margin-bottom: 1rem;
        }

        .tab-content li {
            margin-bottom: 0.5rem;
            color: #666;
        }

        /* Audio player */
        .audio-player {
            background: #f5f5f5;
            padding: 1.5rem;
            border-radius: 0.5rem;
            margin-bottom: 1rem;
        }

        .audio-item {
            display: flex;
            align-items: center;
            gap: 1rem;
            margin-bottom: 1rem;
        }

        .audio-item:last-child {
            margin-bottom: 0;
        }

        .play-btn {
            width: 2.5rem;
            height: 2.5rem;
            border-radius: 50%;
            background: #E84A2B;
            color: white;
            border: none;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1rem;
            transition: all 0.3s;
        }

        .play-btn:hover {
            background: #d63d1f;
        }

        .audio-info {
            flex: 1;
        }

        .audio-title {
            font-weight: 600;
            color: #333;
            margin-bottom: 0.3rem;
        }

        .audio-duration {
            font-size: 0.85rem;
            color: #999;
        }

        /* Navigation */
        .product-nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-top: 2rem;
            padding-top: 2rem;
            border-top: 1px solid #eee;
        }

        .nav-link {
            text-decoration: none;
            color: #E84A2B;
            font-weight: 600;
            transition: color 0.3s;
        }

        .nav-link:hover {
            color: #d63d1f;
        }

        /* Footer */
        footer {
            background: #1e1e1e;
            color: #ccc;
            padding: 2rem 0 1rem;
            margin-top: 3rem;
        }

        .footer-content {
            max-width: 1400px;
            margin: 0 auto;
            padding: 0 1rem;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 2rem;
            margin-bottom: 2rem;
        }

        .footer-section h3 {
            color: white;
            margin-bottom: 1rem;
            font-size: 0.95rem;
        }

        .footer-section ul {
            list-style: none;
        }

        .footer-section a {
            color: #999;
            text-decoration: none;
            font-size: 0.85rem;
            display: block;
            margin-bottom: 0.5rem;
            transition: color 0.3s;
        }

        .footer-section a:hover {
            color: #E84A2B;
        }

        .footer-bottom {
            border-top: 1px solid #333;
            padding-top: 1rem;
            text-align: center;
            font-size: 0.8rem;
            color: #666;
            max-width: 1400px;
            margin: 0 auto;
            padding-left: 1rem;
            padding-right: 1rem;
        }

        /* Responsive */
        @media (max-width: 1024px) {
            .main-container {
                grid-template-columns: 1fr;
            }

            .purchase-buttons {
                grid-template-columns: 1fr;
            }
        }

        @media (max-width: 768px) {
            .nav-menu {
                display: none;
            }

            .menu-toggle {
                display: block;
            }

            .search-box {
                width: 150px;
            }

            .tabs-header {
                flex-wrap: wrap;
            }

            .tab-btn {
                padding: 0.75rem 1rem;
                font-size: 0.85rem;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="header-top">
            <a href="#" class="logo">
                <span class="logo-icon">📚</span>
                堂奧圖書
        </div>
    </header>

    <!-- Breadcrumb -->
    <div class="breadcrumb">
        <a href="#">首頁</a> > <a href="#">所有書籍</a> > <a href="#">檢定考試類</a> > <a href="#">劍橋兒童英檢 YLE</a> > <a href="#">Cambridge YLE</a> > Cambridge Young Learners English Tests:Starters(Qrcode版)_TA0045 YLE
    </div>

    <!-- Main content -->
    <div class="main-container">
        <!-- Product images -->
        <div class="product-image-section">
            <div class="product-main-image">
                <div class="mp3-badge">🎵 MP3</div>
                📖
            </div>
        </div>

        <!-- Product info -->
        <div class="product-info-section">
            <div class="product-header">
                <div class="product-isbn">9789860619270</div>
                <div class="product-title">Cambridge Young Learners English Tests:Starters(Qrcode版)_TA0045 YLE</div>
                <div class="product-price">
                    <span class="price-current">$ 320</span>
                    <span class="price-original">$ 400</span>
                </div>
                <div class="product-share">
                    <span class="share-label">share</span>
                    <a href="#" class="share-btn">f</a>
                    <a href="#" class="share-btn">L</a>
                </div>
            </div>

            <!-- Specs table -->
            <table class="specs-table">
                <tr>
                    <td>ISBN</td>
                    <td>9789860619270</td>
                </tr>
                <tr>
                    <td>作者</td>
                    <td>written by Sue E. Leeward</td>
                </tr>
                <tr>
                    <td>出版</td>
                    <td>Skyline Research Team</td>
                </tr>
                <tr>
                    <td>頁數</td>
                    <td>88</td>
                </tr>
                <tr>
                    <td>尺寸</td>
                    <td>210mm x 297mm</td>
                </tr>
                <tr>
                    <td>規格</td>
                    <td>彩色/平裝</td>
                </tr>
                <tr>
                    <td>書系</td>
                    <td>YLE Exams</td>
                </tr>
                <tr>
                    <td>級數</td>
                    <td>Starters/A1</td>
                </tr>
                <tr>
                    <td>應用程度</td>
                    <td>國小</td>
                </tr>
                <tr>
                    <td>出版日期</td>
                    <td>2021年03月</td>
                </div>
            </div>
        </div>
    </div>

    <!-- Tabs section -->
    <div class="main-container" style="margin-top: 0; padding-top: 0;">
        <div class="tabs-container" style="grid-column: 1 / -1;">
            <div class="tabs-header">
                <button class="tab-btn active" onclick="switchTab(event, 'details')">詳細說明</button>
                <button class="tab-btn" onclick="switchTab(event, 'download')">文件檔下載</button>
                <button class="tab-btn" onclick="switchTab(event, 'audio')">線上音檔</button>
                <button class="tab-btn" onclick="switchTab(event, 'audio-download')">音檔下載</button>
            </div>

            <!-- Details tab -->
            <div id="details" class="tab-content active">
                <h3>教材說明</h3>
                <p>Cambridge Young Learners English Tests系列包含三個測驗級數：Starters, Movers, Flyers。每冊提供四回完整的模擬試題，適合準備劍橋兒童英檢的學習者。</p>
                
                <h3>試題本</h3>
                <p>試題本：四回測驗（每回含 Listening, Reading &Writing, Speaking Test）</p>
                <p>能力&口說MP3上線</p>
                
                <h3>解答本</h3>
                <p>解答本：QR Code 下載/搜尋、詳細內容、口說測驗試題、級數測驗字彙範圍。</p>
                
                <h3>系列特點</h3>
                <ul>
                    <li>完全仿真題型，實戰模擬試題</li>
                    <li>提供英式音聲，模擬原考場情境</li>
                    <li>完整的下載答案、詳音、口說測驗試題、級數測驗字彙範圍。</li>
                </ul>
            </div>

            <!-- Download tab -->
            <div id="download" class="tab-content">
                <h3>文件檔下載</h3>
                <p>本產品提供以下文件檔供下載：</p>
                <ul>
                    <li><a href="#" style="color: #E84A2B;">解答本 PDF</a></li>
                    <li><a href="#" style="color: #E84A2B;">詳細內容 PDF</a></li>
                    <li><a href="#" style="color: #E84A2B;">試題內容 PDF</a></li>
                </ul>
            </div>

            <!-- Audio tab -->
            <div id="audio" class="tab-content">
                <h3>線上音檔</h3>
                <p>以下為本產品的線上音檔，可直接在線上聆聽：</p>
                <div class="audio-player">
                    <div class="audio-item">
                        <button class="play-btn">▶</button>
                        <div class="audio-info">
                            <div class="audio-title">Test 1 - Listening Part 1</div>
                            <div class="audio-duration">3:45</div>
                        </div>
                    </div>
                    <div class="audio-item">
                        <button class="play-btn">▶</button>
                        <div class="audio-info">
                            <div class="audio-title">Test 1 - Listening Part 2</div>
                            <div class="audio-duration">4:20</div>
                        </div>
                    </div>
                    <div class="audio-item">
                        <button class="play-btn">▶</button>
                        <div class="audio-info">
                            <div class="audio-title">Test 2 - Listening Part 1</div>
                            <div class="audio-duration">3:50</div>
                        </div>
                    </div>
                    <div class="audio-item">
                        <button class="play-btn">▶</button>
                        <div class="audio-info">
                            <div class="audio-title">Test 2 - Listening Part 2</div>
                            <div class="audio-duration">4:15</div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Audio download tab -->
            <div id="audio-download" class="tab-content">
                <h3>音檔下載</h3>
                <p>可供下載的音檔列表：</p>
                <ul>
                    <li><a href="#" style="color: #E84A2B;">Test 1 - Listening (MP3)</a></li>
                    <li><a href="#" style="color: #E84A2B;">Test 2 - Listening (MP3)</a></li>
                    <li><a href="#" style="color: #E84A2B;">Test 3 - Listening (MP3)</a></li>
                    <li><a href="#" style="color: #E84A2B;">Test 4 - Listening (MP3)</a></li>
                    <li><a href="#" style="color: #E84A2B;">所有音檔 (ZIP)</a></li>
                </ul>
            </div>
        </div>

        <!-- Navigation -->
        <div class="product-nav" style="grid-column: 1 / -1;">
            <a href="#" class="nav-link">← PREV</a>
            <a href="#" class="nav-link">返回列表頁</a>
            <a href="#" class="nav-link">NEXT →</a>
        </div>
    </div>

    <!-- Footer -->
    <footer>
        <div class="footer-content">
            <div class="footer-section">
                <h3>📚 堂奧圖書</h3>
                <p style="font-size: 0.85rem; color: #999; margin-bottom: 1rem;">堂奧圖書股份有限公司</p>
                <p style="font-size: 0.8rem; color: #666;">
                    統編：12719935<br>
                    TEL：04-27083767<br>
                    FAX：04-24522345<br>
                    台中市西屯區環中路二段876號2樓<br>
                    (週一至週五 09:00~18:00)
                </p>
            </div>
            <div class="footer-section">
                <h3>關於堂奧圖書</h3>
                <ul>
                    <li><a href="#">關於堂奧</a></li>
                    <li><a href="#">購物流程</a></li>
                    <li><a href="#">購物須知</a></li>
                    <li><a href="#">付款方式</a></li>
                    <li><a href="#">聯絡我們</a></li>
                </ul>
            </div>
            <div class="footer-section">
                <h3>所有書籍</h3>
                <ul>
                    <li><a href="#">啟蒙 Age 0-6</a></li>
                    <li><a href="#">國小 Age 7-12</a></li>
                    <li><a href="#">國高中 Age 13-18</a></li>
                    <li><a href="#">檢定考試類</a></li>
                    <li><a href="#">Reading Box讀本</a></li>
                    <li><a href="#">橋樑書/繪讀本</a></li>
                </ul>
            </div>
            <div class="footer-section">
                <h3>會員專區</h3>
                <ul>
                    <li><a href="#">我的帳戶</a></li>
                    <li><a href="#">最愛清單</a></li>
                    <li><a href="#">歷史訂單</a></li>
                    <li><a href="#">我的優惠券</a></li>
                    <li><a href="#">資源下載</a></li>
                </ul>
            </div>
            <div class="footer-section">
                <h3>其他資訊</h3>
                <ul>
                    <li><a href="#">最新消息</a></li>
                    <li><a href="#">文章專欄</a></li>
                    <li><a href="#">常見問題</a></li>
                    <li><a href="#">會員條款</a></li>
                </ul>
            </div>
        </div>
        <div class="footer-bottom">
            <p>© Tang-Ao Book Co., Ltd. | WEBDESIGN</p>
        </div>
    </footer>

    <script>
        // Tab switching
        function switchTab(event, tabName) {
            event.preventDefault();
            
            // Hide all tabs
            const tabs = document.querySelectorAll('.tab-content');
            tabs.forEach(tab => tab.classList.remove('active'));
            
            // Remove active class from all buttons
            const buttons = document.querySelectorAll('.tab-btn');
            buttons.forEach(btn => btn.classList.remove('active'));
            
            // Show selected tab
            document.getElementById(tabName).classList.add('active');
            event.target.classList.add('active');
        }

        // Thumbnail click
        document.querySelectorAll('.thumbnail').forEach(thumb => {
            thumb.addEventListener('click', function() {
                document.querySelectorAll('.thumbnail').forEach(t => t.classList.remove('active'));
                this.classList.add('active');
            });
        });

        // Purchase button
        document.querySelector('.btn-primary').addEventListener('click', function() {
            alert('已加入購物車！');
        });

        // Favorite button
        document.querySelector('.btn-secondary').addEventListener('click', function() {
            this.style.background = this.style.background === 'rgb(232, 74, 43)' ? 'white' : '#E84A2B';
            this.style.color = this.style.color === 'white' ? '#E84A2B' : 'white';
        });

        // Audio player
        document.querySelectorAll('.play-btn').forEach(btn => {
            btn.addEventListener('click', function(e) {
                e.preventDefault();
                alert('音檔播放功能 - 請上傳您的音檔 URL');
            });
        });
    </script>
</body>
</html>
