<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>クリーンキッチン - 小規模飲食店のHACCP対応をサポート</title>
    <style>
        :root {
            --main-color: #1E88E5;
            --accent-color: #E53935;
            --light-gray: #F5F5F5;
            --dark-gray: #333333;
            --white: #FFFFFF;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Hiragino Sans', 'Hiragino Kaku Gothic ProN', Meiryo, sans-serif;
        }
        
        body {
            line-height: 1.6;
            color: var(--dark-gray);
            background-color: var(--white);
        }
        
        header {
            background-color: var(--white);
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 100;
        }
        
        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 5%;
            max-width: 1200px;
            margin: 0 auto;
        }
        
        .logo {
            font-size: 24px;
            font-weight: bold;
            color: var(--main-color);
        }
        
        .logo span {
            color: var(--accent-color);
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 25px;
        }
        
        nav ul li a {
            text-decoration: none;
            color: var(--dark-gray);
            font-weight: 500;
            transition: color 0.3s;
        }
        
        nav ul li a:hover {
            color: var(--main-color);
        }
        
        .cta-button {
            background-color: var(--accent-color);
            color: var(--white);
            padding: 10px 20px;
            border-radius: 5px;
            text-decoration: none;
            font-weight: bold;
            transition: background-color 0.3s;
        }
        
        .cta-button:hover {
            background-color: #C62828;
        }
        
        main {
            margin-top: 80px;
        }
        
        .hero {
            background: linear-gradient(rgba(30, 136, 229, 0.8), rgba(30, 136, 229, 0.8)), url('/api/placeholder/1200/500') center/cover no-repeat;
            color: var(--white);
            padding: 100px 5%;
            text-align: center;
        }
        
        .hero h1 {
            font-size: 38px;
            margin-bottom: 20px;
        }
        
        .hero p {
            font-size: 18px;
            max-width: 800px;
            margin: 0 auto 30px;
        }
        
        .section {
            padding: 80px 5%;
            max-width: 1200px;
            margin: 0 auto;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 50px;
        }
        
        .section-title h2 {
            font-size: 32px;
            color: var(--main-color);
            margin-bottom: 15px;
        }
        
        .section-title p {
            max-width: 800px;
            margin: 0 auto;
            color: #666;
        }
        
        .haccp-info {
            background-color: var(--light-gray);
        }
        
        .info-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            gap: 40px;
        }
        
        .info-item {
            flex: 1 1 300px;
            text-align: center;
            padding: 30px;
            background-color: var(--white);
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }
        
        .info-item:hover {
            transform: translateY(-10px);
        }
        
        .info-item img {
            width: 80px;
            height: 80px;
            margin-bottom: 20px;
        }
        
        .info-item h3 {
            color: var(--main-color);
            margin-bottom: 15px;
        }
        
        .products {
            background-color: var(--white);
        }
        
        .product-cards {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 30px;
        }
        
        .product-card {
            flex: 1 1 300px;
            background-color: var(--white);
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s;
            max-width: 350px;
        }
        
        .product-card:hover {
            transform: translateY(-10px);
        }
        
        .product-image {
            height: 200px;
            background-size: cover;
            background-position: center;
            position: relative;
        }
        
        .badge {
            position: absolute;
            top: 15px;
            right: 15px;
            background-color: var(--accent-color);
            color: var(--white);
            padding: 5px 10px;
            border-radius: 20px;
            font-size: 12px;
            font-weight: bold;
        }
        
        .product-content {
            padding: 25px;
        }
        
        .product-content h3 {
            color: var(--main-color);
            margin-bottom: 10px;
        }
        
        .price {
            font-size: 24px;
            font-weight: bold;
            margin: 15px 0;
        }
        
        .product-button {
            display: block;
            text-align: center;
            background-color: var(--main-color);
            color: var(--white);
            padding: 10px;
            border-radius: 5px;
            text-decoration: none;
            font-weight: bold;
            transition: background-color 0.3s;
        }
        
        .product-button:hover {
            background-color: #1565C0;
        }
        
        .testimonials {
            background-color: var(--light-gray);
        }
        
        .testimonial-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 30px;
        }
        
        .testimonial {
            flex: 1 1 300px;
            background-color: var(--white);
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            max-width: 350px;
        }
        
        .testimonial-header {
            display: flex;
            align-items: center;
            margin-bottom: 20px;
        }
        
        .testimonial-image {
            width: 60px;
            height: 60px;
            border-radius: 50%;
            margin-right: 15px;
        }
        
        .testimonial-name h4 {
            color: var(--main-color);
        }
        
        .testimonial-name p {
            font-size: 14px;
            color: #666;
        }
        
        .testimonial-text {
            position: relative;
            font-style: italic;
        }
        
        .testimonial-text::before {
            content: """;
            font-size: 60px;
            color: var(--main-color);
            opacity: 0.2;
            position: absolute;
            top: -20px;
            left: -15px;
        }
        
        .cta-section {
            background-color: var(--main-color);
            color: var(--white);
            text-align: center;
            padding: 80px 5%;
        }
        
        .cta-section h2 {
            font-size: 32px;
            margin-bottom: 20px;
        }
        
        .cta-section p {
            max-width: 800px;
            margin: 0 auto 30px;
        }
        
        footer {
            background-color: var(--dark-gray);
            color: var(--white);
            padding: 50px 5%;
        }
        
        .footer-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            max-width: 1200px;
            margin: 0 auto;
        }
        
        .footer-column {
            flex: 1 1 200px;
            margin-bottom: 30px;
        }
        
        .footer-column h3 {
            color: var(--white);
            margin-bottom: 20px;
            font-size: 18px;
        }
        
        .footer-column ul {
            list-style: none;
        }
        
        .footer-column ul li {
            margin-bottom: 10px;
        }
        
        .footer-column ul li a {
            color: #CCC;
            text-decoration: none;
            transition: color 0.3s;
        }
        
        .footer-column ul li a:hover {
            color: var(--white);
        }
        
        .copyright {
            text-align: center;
            padding: 20px 0;
            background-color: #222;
            color: #CCC;
        }
        
        /* レスポンシブデザイン */
        @media (max-width: 768px) {
            .header-container {
                flex-direction: column;
                padding: 10px 5%;
            }
            
            nav {
                margin-top: 15px;
            }
            
            nav ul {
                flex-wrap: wrap;
                justify-content: center;
            }
            
            nav ul li {
                margin: 5px 10px;
            }
            
            main {
                margin-top: 130px;
            }
            
            .hero {
                padding: 60px 5%;
            }
            
            .hero h1 {
                font-size: 28px;
            }
            
            .section {
                padding: 60px 5%;
            }
            
            .section-title h2 {
                font-size: 28px;
            }
            
            .cta-section h2 {
                font-size: 28px;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="header-container">
            <div class="logo">クリーン<span>キッチン</span></div>
            <nav>
                <ul>
                    <li><a href="#home">ホーム</a></li>
                    <li><a href="#haccp">HACCP対応</a></li>
                    <li><a href="#products">商品・サービス</a></li>
                    <li><a href="#testimonials">導入事例</a></li>
                    <li><a href="#about">会社概要</a></li>
                    <li><a href="#faq">よくある質問</a></li>
                    <li><a href="#contact" class="cta-button">無料診断</a></li>
                </ul>
            </nav>
        </div>
    </header>
    
    <main id="home">
        <section class="hero">
            <h1>HACCP対応が簡単に！小規模飲食店の衛生管理をトータルサポート</h1>
            <p>改正食品衛生法によるHACCP義務化に対応。個人・小規模飲食店向けの最適な衛生管理セットで、安全・安心な店舗運営をサポートします。</p>
            <a href="#products" class="cta-button">商品を見る</a>
        </section>
        
        <section id="haccp" class="section haccp-info">
            <div class="section-title">
                <h2>HACCP義務化への対応</h2>
                <p>2020年6月の改正食品衛生法施行により、全ての飲食店でHACCP対応が義務化されました。小規模飲食店でも対応が必要です。</p>
            </div>
            <div class="info-container">
                <div class="info-item">
                    <img src="/api/placeholder/80/80" alt="HACCPとは">
                    <h3>HACCPとは</h3>
                    <p>食品の安全を確保するための衛生管理手法です。原材料の受入から提供までの全工程で危害要因を分析し、重要管理点を定めて監視します。</p>
                </div>
                <div class="info-item">
                    <img src="/api/placeholder/80/80" alt="小規模飲食店の課題">
                    <h3>小規模飲食店の課題</h3>
                    <p>専門知識の不足、人手不足、コスト負担など、小規模飲食店特有の課題があります。簡易な方法でも基準を満たす対応が求められています。</p>
                </div>
                <div class="info-item">
                    <img src="/api/placeholder/80/80" alt="衛生管理のメリット">
                    <h3>衛生管理のメリット</h3>
                    <p>適切な衛生管理は法令遵守だけでなく、食中毒予防、顧客信頼の獲得、従業員の意識向上などのメリットがあります。</p>
                </div>
            </div>
        </section>
        
        <section id="products" class="section products">
            <div class="section-title">
                <h2>安心の衛生管理セット</h2>
                <p>店舗の規模や業態に合わせた最適な衛生管理セットをご用意しています。HACCP対応に必要な道具・記録用紙・マニュアルがセットになった商品です。</p>
            </div>
            <div class="product-cards">
                <div class="product-card">
                    <div class="product-image" style="background-image: url('/api/placeholder/350/200')">
                        <span class="badge">初めての方におすすめ</span>
                    </div>
                    <div class="product-content">
                        <h3>スターターセット</h3>
                        <p>HACCP対応の基本アイテムをセットにしました。初めて衛生管理に取り組む小規模飲食店におすすめです。</p>
                        <ul>
                            <li>衛生管理簡易マニュアル</li>
                            <li>記録用紙（1年分）</li>
                            <li>非接触体温計</li>
                            <li>アルコール消毒液（500ml）</li>
                            <li>調理用手袋（100枚）</li>
                        </ul>
                        <div class="price">¥19,800（税込）</div>
                        <a href="#contact" class="product-button">詳細を見る</a>
                    </div>
                </div>
                <div class="product-card">
                    <div class="product-image" style="background-image: url('/api/placeholder/350/200')">
                        <span class="badge">人気No.1</span>
                    </div>
                    <div class="product-content">
                        <h3>プレミアムセット</h3>
                        <p>本格的な衛生管理を実現する充実のセット。専門家による導入サポート付きで安心です。</p>
                        <ul>
                            <li>詳細衛生管理マニュアル</li>
                            <li>記録用紙（1年分）</li>
                            <li>非接触体温計</li>
                            <li>ATP検査キット（20回分）</li>
                            <li>アルコール消毒液（1L）</li>
                            <li>調理用手袋（200枚）</li>
                            <li>専門家によるオンライン導入サポート（1回）</li>
                        </ul>
                        <div class="price">¥39,800（税込）</div>
                        <a href="#contact" class="product-button">詳細を見る</a>
                    </div>
                </div>
                <div class="product-card">
                    <div class="product-image" style="background-image: url('/api/placeholder/350/200')">
                        <span class="badge">継続的な管理に</span>
                    </div>
                    <div class="product-content">
                        <h3>サブスクリプションプラン</h3>
                        <p>消耗品の定期配送と専門家サポートがセットになった月額プラン。継続的な衛生管理に最適です。</p>
                        <ul>
                            <li>アルコール消毒液（500ml/月）</li>
                            <li>調理用手袋（100枚/月）</li>
                            <li>ATP検査キット（5回分/月）</li>
                            <li>記録用紙（月ごと更新）</li>
                            <li>専門家によるオンラインサポート（月1回）</li>
                            <li>緊急時サポート（24時間対応）</li>
                        </ul>
                        <div class="price">¥9,800（税込）/月</div>
                        <a href="#contact" class="product-button">詳細を見る</a>
                    </div>
                </div>
            </div>
        </section>
        
        <section id="testimonials" class="section testimonials">
            <div class="section-title">
                <h2>導入事例・お客様の声</h2>
                <p>既に多くの小規模・個人飲食店にご利用いただいています。お客様の声をご紹介します。</p>
            </div>
            <div class="testimonial-container">
                <div class="testimonial">
                    <div class="testimonial-header">
                        <img class="testimonial-image" src="/api/placeholder/60/60" alt="田中様">
                        <div class="testimonial-name
