<html lang="ko">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>나를 소개하는 한 페이지</title>
  <style>
    body {
      font-family: sans-serif;
      max-width: 1100px;
      margin: 0 auto;
      padding: 30px 20px;
      line-height: 1.7;
      color: #222222; 
      background-color: #e9e5dd; /* 요청한 배경색 */
    }
    
    /* 1. 상단 로고(project01) 변경 및 색상 적용 */
    .logo {
      font-size: 1.5rem;
      font-weight: bold;
      margin-bottom: 1.5rem;
      /* 하단에 구분선을 추가하여 깔끔하게 분리 */
      padding-bottom: 10px;
      border-bottom: 1px solid #ccc; 
    }
    .logo-skt {
      color: #E1002A; /* SKT 색상 */
    }
    .logo-aleph {
      color: #FF7A00; /* ALEPH 색상 */
    }

    h1 {
      font-size: 2.2rem;
      margin-bottom: 0.2rem;
      color: #111111;
    }
    .subtitle {
      color: #444444;
      margin-top: 0;
      margin-bottom: 1.5rem; /* 4번: 아래 한 줄 소개 공간 확보 */
    }
    h2 {
      margin-top: 2rem;
      margin-bottom: 0.5rem;
      border-bottom: 2px solid #b0a89a;
      padding-bottom: 0.3rem;
      color: #111111;
    }
    
    a {
      color: #004488;
      text-decoration: underline;
      font-weight: bold;
    }
    a:focus, [tabindex]:focus {
      outline: 3px solid #111111;
      outline-offset: 3px;
    }

    .first-screen {
      display: grid;
      grid-template-columns: 1fr 1fr 1fr;
      gap: 20px;
      margin-top: 1.5rem;
    }
    .card {
      background: #ffffff;
      border: 1px solid #d0c9bd;
      border-radius: 8px;
      padding: 1.2rem;
      box-shadow: 0 1px 3px rgba(0,0,0,0.05);
    }
    .card h3 {
      margin-top: 0;
      font-size: 1.1rem;
      color: #111111;
    }
    .sar {
      font-size: 0.95rem;
      color: #222222;
      margin-bottom: 0.8rem;
    }
    .sar strong {
      color: #000000;
    }
    .evidence {
      font-size: 0.9rem;
      background: #f4f1ec;
      border-left: 4px solid #6c6357;
      padding: 0.5rem 0.8rem;
      color: #222222;
    }

    /* 6. 연락처 구분선 및 여백 철저히 조정 */
    .contact-section {
      margin-top: 3rem; /* 위쪽 여백을 넓혀 확실히 띄움 */
      padding-top: 2rem;
      border-top: 1px solid #ccc; /* 연한 구분선 추가 */
    }
    .contact-section h2 {
      margin-top: 0; /* 구분선 바로 아래에 제목이 오도록 */
      border-bottom: none; /* 기존 h2의 밑줄 제거 */
    }
    
    /* 6. 흰 칸(배경) 삭제 및 폰트 사이즈 2p 축소 */
    .contact-content {
      background: transparent; /* 흰색 배경 삭제 */
      border: none; /* 테두리 삭제 */
      padding: 0; /* 패딩 삭제 */
      font-size: 0.9rem; /* 기존 1rem에서 0.9rem으로 축소 (약 2px) */
      color: #222222;
    }

    @media (max-width: 900px) {
      .first-screen {
        grid-template-columns: 1fr;
      }
    }
  </style>
</head>
<body>

  <!-- 1. 상단 로고 변경 -->
  <div class="logo">
    <span class="logo-skt">SKT</span> <span class="logo-aleph">ALEPH K-뉴딜 아카데미</span>
  </div>

  <!-- 3. 메인 제목 변경 (크기와 색상은 유지) -->
  <h1>나를 소개하는 한 페이지</h1>
  
  <!-- 4. 한 줄 소개 -->
  <p class="subtitle"> AI와 친해지고싶은 김하늘입니다.</p>

  <!-- 강점/취향 카드 -->
  <div class="first-screen">
    <div class="card">
      <h3>[강점/취향 1]</h3>
      <p class="sar">
        <strong>상황:</strong> [어떤 상황이었나요? 예: 동아리 발표 준비가 늦어졌을 때]<br>
        <strong>행동:</strong> [내가 무엇을 했나요? 예: 역할표를 만들어 일을 나눴어요]<br>
        <strong>결과:</strong> [어떻게 됐나요? 예: 발표 자료를 하루 일찍 끝냈어요]
      </p>
      <p class="evidence">
        <strong>근거:</strong> [눈으로 확인할 수 있는 근거. 예: "3일 걸리던 일을 하루 만에 끝냈다" / 사진 / 결과 문장]
      </p>
    </div>
    <div class="card">
      <h3>[강점/취향 2]</h3>
      <p class="sar">
        <strong>상황:</strong> [상황]<br>
        <strong>행동:</strong> [행동]<br>
        <strong>결과:</strong> [결과]
      </p>
      <p class="evidence">
        <strong>근거:</strong> [근거]
      </p>
    </div>
    <div class="card">
      <h3>[강점/취향 3]</h3>
      <p class="sar">
        <strong>상황:</strong> [상황]<br>
        <strong>행동:</strong> [행동]<br>
        <strong>결과:</strong> [결과]
      </p>
      <p class="evidence">
        <strong>근거:</strong> [근거]
      </p>
    </div>
  </div>

  <!-- 경험 -->
  <h2>경험</h2>
  <p>
    - [조교/알바 경험을 한 줄로]<br>
    - [그 경험에서 배운 것을 한 줄로]
  </p>

  <!-- 5. '지금 배우는 것' -> '현재' -->
  <h2>현재</h2>
  <p>
    Python · AI 기초 · 웹 만들기<br>
    [지금 하고 있는 공부나 프로젝트를 한 줄로]
  </p>

  <!-- 5. '앞으로' -> '미래' -->
  <h2>미래</h2>
  <p>
    [되고 싶은 것 / 해보고 싶은 것을 한 줄로]
  </p>

  <!-- 6. '연락' -> '연락처', 구분선 추가, 흰칸 삭제, 폰트 축소 -->
  <div class="contact-section">
    <h2>연락처</h2>
    <div class="contact-content">
      <p>
        GitHub: <a href="https://github.com/[네아이디]">github.com/[khn0916]</a><br>
        Email: <a href="mailto:[네 이메일]">[vorysi@naver.com]</a>
      </p>
    </div>
  </div>

</body>
</html>
