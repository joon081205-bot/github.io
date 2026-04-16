<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>심연의 기록 - 포트폴리오</title>
    <style>
        /* CSS 스타일 시작 */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body, html {
            width: 100%;
            font-family: 'Pretendard', -apple-system, BlinkMacSystemFont, system-ui, Roboto, sans-serif;
            background-color: #000b1a; /* 심해를 상징하는 아주 어두운 파란색 */
            color: #ffffff;
            scroll-behavior: smooth;
        }

        /* 메인 비주얼 섹션 */
        .hero {
            position: relative;
            height: 100vh;
            width: 100%;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            overflow: hidden;
            text-align: center;
        }

        /* 배경 이미지 설정 (드럼통 투하 이미지) */
        .hero-bg {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-image: url('https://img.freepik.com/free-photo/view-wild-nature-with-ocean-cliffs_23-2150700539.jpg'); /* 대체 배경: 동해안 절벽 느낌 */
            background-size: cover;
            background-position: center;
            filter: brightness(0.5); /* 이미지를 어둡게 하여 글자를 강조 */
            z-index: -2;
        }

        /* 드럼통 투하를 상징하는 오버레이 그라데이션 */
        .overlay {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(to bottom, rgba(0,0,0,0.2) 0%, #000b1a 100%);
            z-index: -1;
        }

        .hero-content h1 {
            font-size: clamp(3rem, 10vw, 6rem);
            letter-spacing: 20px;
            text-transform: uppercase;
            margin-bottom: 20px;
            font-weight: 900;
            text-shadow: 0 10px 30px rgba(0,0,0,0.8);
        }

        .hero-content p {
            font-size: 1.2rem;
            letter-spacing: 5px;
            color: #a0c4ff;
            opacity: 0.8;
        }

        /* 섹션 공통 스타일 */
        section {
            padding: 100px 10%;
            min-height: 50vh;
        }

        .section-title {
            font-size: 2.5rem;
            margin-bottom: 50px;
            border-left: 5px solid #0056b3;
            padding-left: 20px;
        }

        /* 소개 섹션 */
        .about-text {
            line-height: 1.8;
            font-size: 1.1rem;
            color: #d1d1d1;
            max-width: 800px;
        }

        /* 프로젝트 카드 그리드 */
        .project-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 50px;
        }

        .card {
            background: rgba(255, 255, 255, 0.05);
            border: 1px solid rgba(255, 255, 255, 0.1);
            padding: 40px;
            border-radius: 15px;
            transition: all 0.4s ease;
            cursor: pointer;
        }

        .card:hover {
            background: rgba(0, 86, 179, 0.2);
            transform: translateY(-15px);
            border-color: #007bff;
        }

        .card h3 {
            font-size: 1.5rem;
            margin-bottom: 15px;
            color: #00bfff;
        }

        /* 푸터 */
        footer {
            text-align: center;
            padding: 50px;
            font-size: 0.8rem;
            color: #444;
            border-top: 1px solid #111;
        }

        /* 드럼통 이미지 위치를 위한 장식 */
        .drum-symbol {
            font-size: 3rem;
            margin-bottom: 20px;
            display: block;
        }
    </style>
</head>
<body>

    <header class="hero">
        <div class="hero-bg"></div>
        <div class="overlay"></div>
        <div class="hero-content">
            <span class="drum-symbol">🛢️</span>
            <h1>CAST AWAY</h1>
            <p>동해 바다 깊이 무거운 과거를 던지다</p>
        </div>
    </header>

    <section id="about">
        <h2 class="section-title">Concept: The Deep Sea</h2>
        <div class="about-text">
            <p>
                무거운 드럼통이 차가운 동해 바다로 떨어지는 순간, <br>
                수면 위의 소란은 사라지고 정적만이 남습니다. <br><br>
                우리는 불필요한 고정관념과 과거의 낡은 습관들을 심연으로 던져버리고, <br>
                오직 본질적인 가치만을 남겨 새로운 프로젝트를 쌓아 올립니다.
            </p>
        </div>
    </section>

    <section id="projects">
        <h2 class="section-title">Projects</h2>
        <div class="project-grid">
            <div class="card">
                <h3>01. 드럼통 로직</h3>
                <p>무거운 데이터를 압축하여 효율적으로 처리하는 백엔드 아키텍처 설계.</p>
            </div>
            <div class="card">
                <h3>02. 심해의 UI</h3>
                <p>사용자에게 깊은 몰입감을 선사하는 다크 모드 기반의 인터페이스 디자인.</p>
            </div>
            <div class="card">
                <h3>03. 계엄령 시스템</h3>
                <p>비상 상황 발생 시 즉각적으로 시스템을 제어하고 보호하는 보안 프로토콜 개발.</p>
            </div>
        </div>
    </section>

    <footer>
        <p>&copy; 2024 DEEP SEA PORTFOLIO. All rights reserved.</p>
    </footer>

</body>
</html>
