<!DOCTYPE html>
<html lang="zh-TW">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>堂奧圖書 - 英語教材專家</title>
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
        }

        .container {
            max-width: 1280px;
            margin: 0 auto;
            padding: 0 1rem;
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
        }

        .cart-icon {
            position: relative;
            cursor: pointer;
            font-size: 1.2rem;
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

        /* Hero Banner */
        .hero {
            height: 400px;
            background: linear-gradient(135deg, #f5a623 0%, #E84A2B 100%);
            display: flex;
            align-items: center;
            color: white;
            position: relative;
            overflow: hidden;
        }

        .hero::before {
            content: '';
            position: absolute;
            right: 0;
            top: 0;
            width: 50%;
            height: 100%;
            background: url('https://images.unsplash.com/photo-1456513080510-7bf3a84b82f8?w=600&h=400&fit=crop') center/cover;
            opacity: 0.3;
        }

        .hero-content {
            position: relative;
            z-index: 2;
            max-width: 600px;
        }

        .hero h1 {
            font-size: 2.5rem;
            font-family: 'Noto Serif TC', serif;
            margin-bottom: 1rem;
            line-height: 1.2;
        }

        .hero p {
            font-size: 1rem;
            margin-bottom: 1.5rem;
            opacity: 0.95;
        }

        .hero-btn {
            background: white;
            color: #E84A2B;
            border: none;
            padding: 0.75rem 2rem;
            border-radius: 2rem;
            font-weight: 600;
            cursor: pointer;
            transition: transform 0.3s;
        }

        .hero-btn:hover {
            transform: scale(1.05);
        }

        /* Section */
        section {
            padding: 3rem 0;
        }

        section h2 {
            font-size: 2rem;
            font-family: 'Noto Serif TC', serif;
            margin-bottom: 2rem;
            text-align: center;
        }

        .section-label {
            text-align: center;
            color: #E84A2B;
            font-size: 0.85rem;
            font-weight: 600;
            letter-spacing: 0.1rem;
            margin-bottom: 0.5rem;
        }

        /* Category Section */
        .category-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 1.5rem;
            margin: 2rem 0;
        }

        .category-card {
            text-align: center;
            padding: 1.5rem;
            border-radius: 1rem;
            background: #FFF3F0;
            cursor: pointer;
            transition: transform 0.3s, box-shadow 0.3s;
            border: 2px solid #FFD5CC;
        }

        .category-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 5px 15px rgba(232, 74, 43, 0.2);
        }

        .category-icon {
            font-size: 2.5rem;
            margin-bottom: 0.5rem;
        }

        .category-card p {
            font-size: 0.9rem;
            font-weight: 600;
            color: #333;
        }

        /* Books Grid */
        .books-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
            gap: 1.5rem;
            margin: 2rem 0;
        }

        .book-card {
            background: white;
            border: 1px solid #eee;
            border-radius: 0.75rem;
            overflow: hidden;
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .book-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0,0,0,0.1);
        }

        .book-cover {
            width: 100%;
            aspect-ratio: 3/4;
            background: #f5f5f5;
            overflow: hidden;
            position: relative;
        }

        .book-cover img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .book-badge {
            position: absolute;
            top: 0.5rem;
            left: 0.5rem;
            background: #E84A2B;
            color: white;
            padding: 0.25rem 0.75rem;
            border-radius: 1rem;
            font-size: 0.75rem;
            font-weight: 600;
        }

        .book-info {
            padding: 1rem;
        }

        .book-isbn {
            font-size: 0.75rem;
            color: #999;
            margin-bottom: 0.5rem;
        }

        .book-title {
            font-size: 0.95rem;
            font-weight: 600;
            margin-bottom: 0.75rem;
            line-height: 1.3;
            min-height: 2.6rem;
        }

        .book-price {
            display: flex;
            align-items: baseline;
            gap: 0.5rem;
            margin-bottom: 1rem;
        }

        .book-price-current {
            font-size: 1.25rem;
            font-weight: 700;
            color: #E84A2B;
        }

        .book-price-original {
            font-size: 0.85rem;
            color: #999;
            text-decoration: line-through;
        }

        .book-actions {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 0.5rem;
        }

        .btn {
            padding: 0.5rem;
            border: none;
            border-radius: 0.5rem;
            font-size: 0.8rem;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s;
        }

        .btn-primary {
            background: #E84A2B;
            color: white;
        }

        .btn-primary:hover {
            background: #d63d1f;
        }

        .btn-secondary {
            background: #f5f5f5;
            color: #666;
            border: 1px solid #ddd;
        }

        .btn-secondary:hover {
            background: #fff;
            border-color: #E84A2B;
            color: #E84A2B;
        }

        /* News Section */
        .news-list {
            max-width: 800px;
            margin: 2rem auto;
        }

        .news-item {
            display: flex;
            gap: 1rem;
            padding: 1rem;
            border-bottom: 1px solid #eee;
            cursor: pointer;
            transition: background 0.3s;
        }

        .news-item:hover {
            background: #f9f9f9;
        }

        .news-date {
            font-size: 0.8rem;
            color: #999;
            min-width: 80px;
            font-weight: 600;
        }

        .news-tag {
            display: inline-block;
            background: #FFF3F0;
            color: #E84A2B;
            padding: 0.25rem 0.75rem;
            border-radius: 1rem;
            font-size: 0.75rem;
            font-weight: 600;
            min-width: 80px;
            text-align: center;
            margin-right: 0.5rem;
        }

        .news-title {
            flex: 1;
            color: #333;
            text-decoration: none;
        }

        /* Footer */
        footer {
            background: #1e1e1e;
            color: #ccc;
            padding: 2rem 0 1rem;
            margin-top: 3rem;
        }

        .footer-content {
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
        }

        /* Responsive */
        @media (max-width: 768px) {
            .nav-menu {
                display: none;
            }

            .search-box {
                width: 150px;
            }

            .hero {
                height: 300px;
            }

            .hero h1 {
                font-size: 1.75rem;
            }

            .books-grid {
                grid-template-columns: repeat(auto-fill, minmax(150px, 1fr));
            }

            .category-grid {
                grid-template-columns: repeat(3, 1fr);
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container">
            <div class="header-top">
                <a href="#" class="logo">
                    <span class="logo-icon">📚</span>
                    堂奧圖書
                </a>
                <ul class="nav-menu">
                    <li><a href="#books">所有書籍</a></li>
                    <li><a href="#category">分類</a></li>
                    <li><a href="#news">最新消息</a></li>
                    <li><a href="#about">關於我們</a></li>
                </ul>
                <div class="header-actions">
                    <div class="search-box">
                        <input type="text" placeholder="搜尋書名...">
                        <button>🔍</button>
                    </div>
                    <div class="cart-icon">
                        🛒
                        <span class="cart-badge">0</span>
                    </div>
                </div>
            </div>
        </div>
        <div class="nav-secondary">
            <div class="container">
                <a href="#">會員專區</a>
                <a href="#">資源下載</a>
                <a href="#">文章專欄</a>
                <a href="#">常見問題</a>
                <a href="#">聯絡我們</a>
            </div>
        </div>
    </header>

    <!-- Hero Banner -->
    <section class="hero">
        <div class="container">
            <div class="hero-content">
                <p style="font-size: 0.9rem; opacity: 0.9;">英語口說教材</p>
                <h1>Let's Speak! 會聽會說超 easy</h1>
                <p>一套三冊式的英語口說教材，專為以英語為外語的國小學生設計。透過有趣的活動與有結構的對話練習，提升學生的語言學習效果。</p>
                <button class="hero-btn">立即前往 →</button>
            </div>
        </div>
    </section>

    <!-- Category Section -->
    <section id="category">
        <div class="container">
            <div class="section-label">CATEGORY</div>
            <h2>按分類找書籍</h2>
            <div class="category-grid">
                <div class="category-card">
                    <div class="category-icon">🍎</div>
                    <p>啟蒙 Age 0-6</p>
                </div>
                <div class="category-card">
                    <div class="category-icon">📚</div>
                    <p>國小 Age 7-12</p>
                </div>
                <div class="category-card">
                    <div class="category-icon">🎓</div>
                    <p>國高中 Age 13-18</p>
                </div>
                <div class="category-card">
                    <div class="category-icon">📝</div>
                    <p>檢定考試類</p>
                </div>
                <div class="category-card">
                    <div class="category-icon">📖</div>
                    <p>Reading Box讀本</p>
                </div>
                <div class="category-card">
                    <div class="category-icon">🌟</div>
                    <p>橋樑書/繪讀本</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Bestsellers -->
    <section id="books">
        <div class="container">
            <div class="section-label">BEST ITEMS</div>
            <h2>暢銷專區</h2>
            <div class="books-grid">
                <div class="book-card">
                    <div class="book-cover">
                        <img src="https://images.unsplash.com/photo-1544716278-ca5e3f4abd8c?w=300&h=400&fit=crop" alt="A++ 文法通 3">
                        <span class="book-badge">暢銷</span>
                    </div>
                    <div class="book-info">
                        <div class="book-isbn">9789869627146</div>
                        <div class="book-title">A++ 文法通 3</div>
                        <div class="book-price">
                            <span class="book-price-current">$ 152</span>
                            <span class="book-price-original">$ 190</span>
                        </div>
                        <div class="book-actions">
                            <button class="btn btn-primary">加入購物車</button>
                            <button class="btn btn-secondary">了解更多</button>
                        </div>
                    </div>
                </div>

                <div class="book-card">
                    <div class="book-cover">
                        <img src="https://images.unsplash.com/photo-1553729459-efe14ef6055d?w=300&h=400&fit=crop" alt="新全民英檢黃金考題">
                        <span class="book-badge">暢銷</span>
                    </div>
                    <div class="book-info">
                        <div class="book-isbn">9789869888967</div>
                        <div class="book-title">新全民英檢黃金考題：初級閱讀測驗</div>
                        <div class="book-price">
                            <span class="book-price-current">$ 280</span>
                            <span class="book-price-original">$ 350</span>
                        </div>
                        <div class="book-actions">
                            <button class="btn btn-primary">加入購物車</button>
                            <button class="btn btn-secondary">了解更多</button>
                        </div>
                    </div>
                </div>

                <div class="book-card">
                    <div class="book-cover">
                        <img src="https://images.unsplash.com/photo-1497633762265-9d179a990aa6?w=300&h=400&fit=crop" alt="A++ 英語會考高分攻略">
                        <span class="book-badge">暢銷</span>
                    </div>
                    <div class="book-info">
                        <div class="book-isbn">9786269846702</div>
                        <div class="book-title">A++ 英語會考高分攻略</div>
                        <div class="book-price">
                            <span class="book-price-current">$ 224</span>
                            <span class="book-price-original">$ 280</span>
                        </div>
                        <div class="book-actions">
                            <button class="btn btn-primary">加入購物車</button>
                            <button class="btn btn-secondary">了解更多</button>
                        </div>
                    </div>
                </div>

                <div class="book-card">
                    <div class="book-cover">
                        <img src="https://images.unsplash.com/photo-1456513080510-7bf3a84b82f8?w=300&h=400&fit=crop" alt="Let's Speak! 3 with Activity Book">
                        <span class="book-badge">新書</span>
                    </div>
                    <div class="book-info">
                        <div class="book-isbn">9786269954315</div>
                        <div class="book-title">Let's Speak! 3 with Activity Book</div>
                        <div class="book-price">
                            <span class="book-price-current">$ 288</span>
                            <span class="book-price-original">$ 360</span>
                        </div>
                        <div class="book-actions">
                            <button class="btn btn-primary">加入購物車</button>
                            <button class="btn btn-secondary">了解更多</button>
                        </div>
                    </div>
                </div>

                <div class="book-card">
                    <div class="book-cover">
                        <img src="https://images.unsplash.com/photo-1535905557558-afc4877a26fc?w=300&h=400&fit=crop" alt="Dragon Masters 兒童英語橋樑書">
                        <span class="book-badge">暢銷</span>
                    </div>
                    <div class="book-info">
                        <div class="book-isbn">9786269627140</div>
                        <div class="book-title">Dragon Masters 兒童英語橋樑書 Vol.1</div>
                        <div class="book-price">
                            <span class="book-price-current">$ 192</span>
                            <span class="book-price-original">$ 240</span>
                        </div>
                        <div class="book-actions">
                            <button class="btn btn-primary">加入購物車</button>
                            <button class="btn btn-secondary">了解更多</button>
                        </div>
                    </div>
                </div>

                <div class="book-card">
                    <div class="book-cover">
                        <img src="https://images.unsplash.com/photo-1507842217343-583bb7270b66?w=300&h=400&fit=crop" alt="Reading Comprehension 3 CD">
                        <span class="book-badge">特價</span>
                    </div>
                    <div class="book-info">
                        <div class="book-isbn">MK9010009023</div>
                        <div class="book-title">Reading Comprehension 3 CD</div>
                        <div class="book-price">
                            <span class="book-price-current">$ 100</span>
                            <span class="book-price-original">$ 150</span>
                        </div>
                        <div class="book-actions">
                            <button class="btn btn-primary">加入購物車</button>
                            <button class="btn btn-secondary">了解更多</button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- News Section -->
    <section id="news" style="background: #f9f9f9;">
        <div class="container">
            <div class="section-label">LATEST NEWS</div>
            <h2>最新消息</h2>
            <div class="news-list">
                <div class="news-item">
                    <span class="news-date">2025.09.01</span>
                    <span class="news-tag">勵誠公告</span>
                    <span class="news-title">新全民英檢保證班：初級閱讀測驗</span>
                </div>
                <div class="news-item">
                    <span class="news-date">2025.06.04</span>
                    <span class="news-tag">勵誠公告</span>
                    <span class="news-title">My First Reading 101 封面 QR Code 更正</span>
                </div>
                <div class="news-item">
                    <span class="news-date">2025.04.15</span>
                    <span class="news-tag">新書上市</span>
                    <span class="news-title">Let's Speak! with Activity Book 全新上市</span>
                </div>
                <div class="news-item">
                    <span class="news-date">2025.03.20</span>
                    <span class="news-tag">新書上市</span>
                    <span class="news-title">Dragon Masters 橋樑書系列第二冊正式發售</span>
                </div>
                <div class="news-item">
                    <span class="news-date">2025.02.10</span>
                    <span class="news-tag">活動公告</span>
                    <span class="news-title">2025 春季書展優惠活動開跑，全館 8 折起</span>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer id="about">
        <div class="container">
            <div class="footer-content">
                <div class="footer-section">
                    <h3>📚 堂奧圖書</h3>
                    <p style="font-size: 0.85rem; color: #999; margin-bottom: 1rem;">堂奧圖書股份有限公司</p>
                    <p style="font-size: 0.8rem; color: #666;">
                        📍 台中市西屯區環中路二段876號2樓<br>
                        📞 04-27083767<br>
                        📠 04-24522345<br>
                        🕐 週一至週五 09:00~18:00
                    </p>
                </div>
                <div class="footer-section">
                    <h3>關於堂奧</h3>
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
                    </ul>
                </div>
                <div class="footer-section">
                    <h3>其他資訊</h3>
                    <ul>
                        <li><a href="#">資源下載</a></li>
                        <li><a href="#">最新消息</a></li>
                        <li><a href="#">文章專欄</a></li>
                        <li><a href="#">常見問題</a></li>
                        <li><a href="#">會員條款</a></li>
                    </ul>
                </div>
            </div>
            <div class="footer-bottom">
                <p>© 2025 Tang-Ao Book Co., Ltd. 堂奧圖書股份有限公司 | 統編：12719935</p>
            </div>
        </div>
    </footer>

    <script>
        // 簡單的互動功能
        document.querySelectorAll('.btn-primary').forEach(btn => {
            btn.addEventListener('click', function() {
                alert('已加入購物車！');
            });
        });

        document.querySelectorAll('.btn-secondary').forEach(btn => {
            btn.addEventListener('click', function() {
                alert('商品詳情頁即將上線！');
            });
        });

        document.querySelectorAll('.category-card').forEach(card => {
            card.addEventListener('click', function() {
                alert('分類頁面即將上線！');
            });
        });

        document.querySelectorAll('.news-item').forEach(item => {
            item.addEventListener('click', function() {
                alert('文章詳情頁即將上線！');
            });
        });

        document.querySelector('.hero-btn').addEventListener('click', function() {
            alert('商品詳情頁即將上線！');
        });
    </script>
</body>
</html>
