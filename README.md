<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>エコラックス ボタニカルボディソープ | 12時間持続の贅沢な香り</title>
    <style>
        :root {
            --primary: #2c7d50;
            --primary-light: #4c9d70;
            --secondary: #f8f5e9;
            --accent: #d6a75c;
            --text: #333333;
            --light-text: #666666;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Noto Sans JP', sans-serif;
        }
        
        body {
            color: var(--text);
            line-height: 1.6;
            background-color: #ffffff;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* ヘッダー */
        header {
            background: linear-gradient(rgba(44, 125, 80, 0.8), rgba(44, 125, 80, 0.8)), url("/api/placeholder/1200/600") center/cover;
            color: white;
            padding: 120px 0 80px;
            text-align: center;
        }
        
        .catchcopy {
            font-size: 2.8rem;
            font-weight: 700;
            margin-bottom: 20px;
            line-height: 1.3;
        }
        
        .subcopy {
            font-size: 1.4rem;
            margin-bottom: 30px;
            font-weight: 300;
        }
        
        .product-title {
            font-size: 2rem;
            margin-bottom: 40px;
            font-weight: 500;
        }
        
        .product-image {
            max-width: 80%;
            margin: 0 auto 40px;
            border-radius: 8px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.15);
        }
        
        .cta-buttons {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-top: 30px;
            flex-wrap: wrap;
        }
        
        .cta-button {
            display: inline-block;
            padding: 15px 35px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            font-size: 1.1rem;
            transition: all 0.3s ease;
        }
        
        .primary-cta {
            background-color: var(--accent);
            color: white;
        }
        
        .primary-cta:hover {
            background-color: #c0903e;
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(214, 167, 92, 0.4);
        }
        
        .secondary-cta {
            background-color: transparent;
            color: white;
            border: 2px solid white;
        }
        
        .secondary-cta:hover {
            background-color: rgba(255, 255, 255, 0.1);
            transform: translateY(-3px);
        }
        
        /* セクション共通 */
        section {
            padding: 80px 0;
        }
        
        .section-title {
            text-align: center;
            font-size: 2.2rem;
            margin-bottom: 50px;
            position: relative;
            color: var(--primary);
        }
        
        .section-title:after {
            content: "";
            display: block;
            width: 60px;
            height: 3px;
            background-color: var(--accent);
            margin: 15px auto 0;
        }
        
        /* 導入文 */
        .intro {
            background-color: var(--secondary);
            text-align: center;
            padding: 60px 0;
        }
        
        .intro p {
            font-size: 1.3rem;
            max-width: 800px;
            margin: 0 auto;
            color: var(--primary);
        }
        
        /* 商品特徴 */
        .features {
            background-color: white;
        }
        
        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            margin-top: 40px;
        }
        
        .feature-item {
            text-align: center;
            padding: 30px 20px;
            border-radius: 10px;
            transition: all 0.3s ease;
            background-color: #f9f9f9;
        }
        
        .feature-item:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.1);
        }
        
        .feature-icon {
            width: 80px;
            height: 80px;
            margin: 0 auto 20px;
            display: flex;
            align-items: center;
            justify-content: center;
            background-color: var(--primary-light);
            border-radius: 50%;
        }
        
        .feature-icon svg {
            width: 40px;
            height: 40px;
            fill: white;
        }
        
        .feature-title {
            font-size: 1.2rem;
            margin-bottom: 15px;
            color: var(--primary);
        }
        
        .feature-desc {
            color: var(--light-text);
            font-size: 0.95rem;
        }
        
        /* 使用方法 */
        .usage {
            background-color: var(--secondary);
        }
        
        .usage-content {
            display: flex;
            align-items: center;
            gap: 50px;
            flex-wrap: wrap;
        }
        
        .usage-video {
            flex: 1;
            min-width: 300px;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
        }
        
        .usage-steps {
            flex: 1;
            min-width: 300px;
        }
        
        .step {
            margin-bottom: 25px;
            display: flex;
            align-items: flex-start;
        }
        
        .step-number {
            background-color: var(--primary);
            color: white;
            width: 30px;
            height: 30px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
            margin-right: 15px;
            flex-shrink: 0;
        }
        
        .step-content h4 {
            margin-bottom: 5px;
            color: var(--primary);
        }
        
        /* 成分説明 */
        .ingredients {
            background-color: white;
        }
        
        .ingredients-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
        }
        
        .ingredient-card {
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: all 0.3s ease;
        }
        
        .ingredient-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
        }
        
        .ingredient-image {
            height: 200px;
            background-color: #f0f0f0;
        }
        
        .ingredient-info {
            padding: 20px;
        }
        
        .ingredient-name {
            font-size: 1.2rem;
            margin-bottom: 10px;
            color: var(--primary);
        }
        
        .qr-info {
            margin-top: 40px;
            text-align: center;
            padding: 20px;
            background-color: #f9f9f9;
            border-radius: 10px;
        }
        
        .qr-code {
            max-width: 120px;
            margin: 0 auto 15px;
        }
        
        /* 香り */
        .fragrances {
            background-color: var(--secondary);
        }
        
        .fragrance-cards {
            display: flex;
            gap: 30px;
            justify-content: center;
            flex-wrap: wrap;
            margin-bottom: 50px;
        }
        
        .fragrance-card {
            background-color: white;
            border-radius: 10px;
            overflow: hidden;
            width: 300px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: all 0.3s ease;
        }
        
        .fragrance-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
        }
        
        .fragrance-image {
            height: 180px;
            background-color: #f0f0f0;
        }
        
        .fragrance-info {
            padding: 20px;
        }
        
        .fragrance-name {
            font-size: 1.2rem;
            margin-bottom: 10px;
            color: var(--primary);
        }
        
        .ar-feature {
            text-align: center;
            padding: 30px;
            background-color: white;
            border-radius: 10px;
            margin-top: 40px;
        }
        
        .ar-icon {
            width: 60px;
            height: 60px;
            margin: 0 auto 20px;
        }
        
        /* 顧客の声 */
        .testimonials {
            background-color: white;
        }
        
        .testimonial-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .testimonial-card {
            background-color: #f9f9f9;
            border-radius: 10px;
            padding: 30px;
            position: relative;
        }
        
        .testimonial-card:before {
            content: """;
            position: absolute;
            top: 10px;
            left: 20px;
            font-size: 5rem;
            color: rgba(44, 125, 80, 0.1);
            font-family: serif;
        }
        
        .testimonial-content {
            margin-bottom: 20px;
            position: relative;
            z-index: 1;
        }
        
        .testimonial-author {
            display: flex;
            align-items: center;
        }
        
        .author-avatar {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            margin-right: 15px;
            background-color: #e0e0e0;
        }
        
        .expert-card {
            margin-top: 50px;
            background-color: var(--primary-light);
            color: white;
            border-radius: 10px;
            padding: 30px;
            display: flex;
            align-items: center;
            gap: 30px;
            flex-wrap: wrap;
        }
        
        .expert-image {
            width: 120px;
            height: 120px;
            border-radius: 50%;
            background-color: white;
            flex-shrink: 0;
        }
        
        /* サステナビリティ */
        .sustainability {
            background-color: var(--secondary);
        }
        
        .sustainability-content {
            display: flex;
            gap: 50px;
            flex-wrap: wrap;
        }
        
        .sustainability-info {
            flex: 1;
            min-width: 300px;
        }
        
        .sustainability-image {
            flex: 1;
            min-width: 300px;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
        }
        
        .eco-item {
            margin-bottom: 25px;
            display: flex;
            align-items: flex-start;
        }
        
        .eco-icon {
            width: 40px;
            height: 40px;
            margin-right: 15px;
            display: flex;
            align-items: center;
            justify-content: center;
            background-color: var(--primary);
            border-radius: 50%;
            flex-shrink: 0;
        }
        
        .eco-icon svg {
            width: 20px;
            height: 20px;
            fill: white;
        }
        
        /* 価格 */
        .pricing {
            background-color: white;
        }
        
        .price-options {
            display: flex;
            justify-content: center;
            gap: 30px;
            flex-wrap: wrap;
            margin-bottom: 50px;
        }
        
        .price-card {
            background-color: white;
            border-radius: 10px;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.08);
            padding: 40px 30px;
            width: 300px;
            transition: all 0.3s ease;
            border: 2px solid transparent;
        }
        
        .price-card:hover {
            transform: scale(1.03);
            border-color: var(--primary-light);
        }
        
        .price-card.featured {
            border-color: var(--primary);
            position: relative;
        }
        
        .price-card.featured:before {
            content: "おすすめ";
            position: absolute;
            top: -15px;
            right: 30px;
            background-color: var(--accent);
            color: white;
            padding: 5px 15px;
            border-radius: 20px;
            font-size: 0.8rem;
            font-weight: bold;
        }
        
        .price-title {
            font-size: 1.3rem;
            margin-bottom: 10px;
            color: var(--primary);
            text-align: center;
        }
        
        .price-amount {
            font-size: 2.5rem;
            text-align: center;
            margin-bottom: 20px;
            color: var(--text);
        }
        
        .price-amount small {
            font-size: 1rem;
            color: var(--light-text);
        }
        
        .price-features {
            margin-bottom: 30px;
        }
        
        .price-feature {
            margin-bottom: 10px;
            display: flex;
            align-items: center;
        }
        
        .price-feature svg {
            width: 16px;
            height: 16px;
            fill: var(--primary);
            margin-right: 10px;
            flex-shrink: 0;
        }
        
        .price-cta {
            text-align: center;
        }
        
        .guarantee {
            text-align: center;
            margin-top: 50px;
            padding: 30px;
            background-color: #f9f9f9;
            border-radius: 10px;
        }
        
        .guarantee-icon {
            width: 60px;
            height: 60px;
            margin: 0 auto 20px;
        }
        
        .sample-form {
            max-width: 600px;
            margin: 50px auto 0;
            background-color: white;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.08);
        }
        
        .form-title {
            text-align: center;
            margin-bottom: 30px;
            color: var(--primary);
        }
        
        .form-group {
            margin-bottom: 20px;
        }
        
        .form-label {
            display: block;
            margin-bottom: 5px;
            font-weight: 500;
        }
        
        .form-input {
            width: 100%;
            padding: 12px 15px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 1rem;
        }
        
        .form-submit {
            display: block;
            width: 100%;
            padding: 15px;
            background-color: var(--primary);
            color: white;
            border: none;
            border-radius: 5px;
            font-size: 1rem;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
        }
        
        .form-submit:hover {
            background-color: var(--primary-light);
        }
        
        /* FAQ */
        .faq {
            background-color: var(--secondary);
        }
        
        .faq-list {
            max-width: 800px;
            margin: 0 auto;
        }
        
        .faq-item {
            margin-bottom: 20px;
            border-radius: 10px;
            overflow: hidden;
            background-color: white;
            box-shadow: 0 3px 10px rgba(0, 0, 0, 0.05);
        }
        
        .faq-question {
            padding: 20px;
            cursor: pointer;
            position: relative;
            font-weight: 500;
            color: var(--primary);
        }
        
        .faq-question:after {
            content: "+";
            position: absolute;
            right: 20px;
            top: 50%;
            transform: translateY(-50%);
            font-size: 1.5rem;
        }
        
        .faq-answer {
            padding: 0 20px 20px;
            color: var(--light-text);
        }
        
        /* 最終CTA */
        .final-cta {
            background: linear-gradient(rgba(44, 125, 80, 0.9), rgba(44, 125, 80, 0.9)), url("/api/placeholder/1200/600") center/cover;
            color: white;
            padding: 80px 0;
            text-align: center;
        }
        
        .final-cta-title {
            font-size: 2.2rem;
            margin-bottom: 20px;
        }
        
        .final-cta-desc {
            max-width: 700px;
            margin: 0 auto 40px;
            font-size: 1.1rem;
        }
        
        .eco-points {
            margin-top: 50px;
            padding: 30px;
            background-color: rgba(255, 255, 255, 0.1);
            border-radius: 10px;
            max-width: 700px;
            margin-left: auto;
            margin-right: auto;
        }
        
        .eco-points-title {
            margin-bottom: 20px;
            font-size: 1.3rem;
        }
        
        /* フッター */
        footer {
            background-color: #333;
            color: white;
            padding: 60px 0 30px;
        }
        
        .footer-content {
            display: flex;
            flex-wrap: wrap;
            gap: 50px;
            margin-bottom: 40px;
        }
        
        .footer-company {
            flex: 2;
            min-width: 300px;
        }
        
        .footer-logo {
            font-size: 1.5rem;
            font-weight: 700;
            margin-bottom: 15px;
        }
        
        .footer-desc {
            color: #aaa;
            margin-bottom: 20px;
        }
        
        .footer-nav {
            flex: 1;
            min-width: 200px;
        }
        
        .footer-heading {
            font-size: 1.1rem;
            margin-bottom: 20px;
            position: relative;
        }
        
        .footer-heading:after {
            content: "";
            display: block;
            width: 30px;
            height: 2px;
            background-color: var(--accent);
            margin-top: 10px;
        }
        
        .footer-links {
            list-style: none;
        }
        
        .footer-links li {
            margin-bottom: 10px;
        }
        
        .footer-links a {
            color: #aaa;
            text-decoration: none;
            transition: color 0.3s ease;
        }
        
        .footer-links a:hover {
            color: white;
        }
        
        .certificates {
            display: flex;
            gap: 20px;
            margin-top: 20px;
            flex-wrap: wrap;
        }
        
        .certificate {
            width: 50px;
            height: 50px;
            background-color: #444;
            border-radius: 5px;
        }
        
        .social-links {
            display: flex;
            gap: 15px;
            margin-top: 20px;
        }
        
        .social-link {
            width: 40px;
            height: 40px;
            background-color: #444;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.3s ease;
        }
        
        .social-link:hover {
            background-color: var(--primary);
        }
        
        .social-link svg {
            width: 20px;
            height: 20px;
            fill: white;
        }
        
        .footer-bottom {
            text-align: center;
            padding-top: 30px;
            border-top: 1px solid #444;
            color: #aaa;
            font-size: 0.9rem;
        }
        
        /* レスポンシブ */
        @media (max-width: 768px) {
            .catchcopy {
                font-size: 2rem;
            }
            
            .subcopy {
                font-size: 1.1rem;
            }
            
            .section-title {
                font-size: 1.8rem;
            }
            
            .cta-buttons {
                flex-direction: column;
                align-items: center;
            }
            
            .expert-card {
                text-align: center;
                flex-direction: column;
            }
            
            .final-cta-title {
                font-size: 1.8rem;
            }
        }
    </style>
</head>
<body>
    <!-- ヘッダー -->
    <header>
        <div class="container">
            <h1 class="catchcopy">自然の恵みで、あなたの肌を包み込む12時間持続の贅沢</h1>
            <p class="subcopy">100%植物由来成分 × 12時間持続香りカプセル技術</p>
            <h2 class="product-title">エコラックス ボタニカルボディソープ</h2>
            <img src="/api/placeholder/800/400" alt="エコラックス ボタニカルボディソープ" class="product-image">
            <div class="cta-buttons">
                <a href="#pricing" class="cta-button primary-cta">今すぐ購入</a>
                <a href="#sample" class="cta-button secondary-cta">無料サンプル請求</a>
            </div>
        </div>
    </header>
    
    <!-- 導入文 -->
    <section class="intro">
        <div class="container">
            <p>忙しい毎日に、贅沢なバスタイムを。エコラックスが叶える、肌と地球に優しい新しいボディケア。</p>
        </div>
    </section>
    
    <!-- 商品特徴 -->
    <section class="features" id="features">
        <div class="container">
            <h2 class="section-title">特徴</h2>
            <div class="features-grid">
                <div class="feature-item">
                    <div class="feature-icon">
                        <svg viewBox="0 0 24 24">
                            <path d="M12,2C6.5,2,2,6.5,2,12s4.5,10,10,10s10-4.5,10-10S17.5,2,12,2z M12,20c-4.4,0-8-3.6-8-8s3.6-8,8-8s8,3.6,8,8S16.4,20,12,20z M12,6c-3.3,0-6,2.7-6,6s2.7,6,6,6s6-2.7,6-6S15.3,6,12,6z M12,16c-2.2,0-4-1.8-4-4s1.8-4,4-4s4,1.8,4,4S14.2,16,12,16z M12,10c-1.1,0-2,0.9-2,2s0.9,2,2,2s2-0.9,2-2S13.1,10,12,10z"/>
                        </svg>
                    </div>
                    <h3 class="feature-title">100%植物由来成分</h3>
                    <p class="feature-desc">オーガニック認証済みの植物から抽出した天然成分のみ使用。合成界面活性剤、鉱物油、パラベン、シリコンは一切不使用。</p>
                </div>
                <div class="feature-item">
                    <div class="feature-icon">
                        <svg viewBox="0 0 24 24">
                            <path d="M12,2C6.5,2,2,6.5,2,12s4.5,10,10,10s10-4.5,10-10S17.5,2,12,2z M12,20c-4.4,0-8-3.6-8-8s3.6-8,8-8s8,3.6,8,8S16.4,20,12,20z M12,6c-3.3,0-6,2.7-6,6s2.7,6,6,6s6-2.7,6-6S15.3,6,12,6z M12,16c-2.2,0-4-1.8-4-4s1.8-4,4-4s4,1.8,4,4S14.2,16,12,16z M12,10c-1.1,0-2,0.9-2,2s0.9,2,2,2s2-0.9,2-2S13.1,10,12,10z"/>
                        </svg>
                    </div>
                    <h3 class="feature-title">12時間持続する香りカプセル技術</h3>
                    <p class="feature-desc">独自開発のマイクロカプセルが肌に留まり、体温や湿度に反応して香りを徐々に放出。一日中、心地よい香りが続きます。</p>
                </div>
                <div class="feature-item">
                    <div class="feature-icon">
                        <svg viewBox="0 0 24 24">
                            <path d="M12,2C6.5,2,2,6.5,2,12s4.5,10,10,10s10-4.5,10-10S17.5,2,12,2z M12,20c-4.4,0-8-3.6-8-8s3.6-8,8-8s8,3.6,8,8S16.4,20,12,20z M12,6c-3.3,0-6,2.7-6,6s2.7,6,6,6s6-2.7,6-6S15.3,6,12,6z M12,16c-2.2,0-4-1.8-4-4s1.8-4,4-4s4,1.8,4,4S14.2,16,12,16z M12,10c-1.1,0-2,0.9-2,2s0.9,2,2,2s2-0.9,2-2S13.1,10,12,10z"/>
                        </svg>
                    </div>
                    <h3 class="feature-title">生分解性容器95%使用</h3>
                    <p class="feature-desc">海洋プラスチック問題に配慮した生分解性容器を採用。使用後は自然に還り、地球環境への負荷を最小限に抑えます。</p>
                </div>
                <div class="feature-item">
                    <div class="feature-icon">
                        <svg viewBox="0 0 24 24">
                            <path d="M12,2C6.5,2,2,6.5,2,12s4.5,10,10,10s10-4.5,10-10S17.5,2,12,2z M12,20c-4.4,0-8-3.6-8-8s3.6-8,8-8s8,3.6,8,8S16.4,20,12,20z M12,6c-3.3,0-6,2.7-6,6s2.7,6,6,6s6-2.7,6-6S15.3,6,12,6z M12,16c-2.2,0-4-1.8-4-4s1.8-4,4-4s4,1.8,4,4S14.2,16,12,16z M12,10
