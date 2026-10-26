<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>나의 한 페이지</title>
  <style>
    /* T01-C16: 텍스트 대비율 확보를 위한 색상 설계 */
    /* 배경(#e9e5dd) 위에 어두운 회색 글자(#222)를 써서 대비율을 4.5:1 이상으로 만듦 */
    body {
      font-family: sans-serif;
      max-width: 1100px;
      margin: 0 auto;
      padding: 30px 20px;
      line-height: 1.7;
      color: #222222; /* 아주 진한 회색 (대비율 매우 높음) */
      background-color: #e9e5dd; /* 요청한 배경색 코드 */
    }
    h1 {
      font-size: 2.2rem;
      margin-bottom: 0.2rem;
      color: #111111; /* 제목은 더 진하게 */
    }
    .subtitle {
      color: #444444; /* 대비율을 위해 기존 #777에서 더 어둡게 변경 */
      margin-top: 0;
    }
    h2 {
      margin-top: 2rem;
      margin-bottom: 0.5rem;
      border-bottom: 2px solid #b0a89a; /* 배경색과 어울리는 테두리 */
      padding-bottom: 0.3rem;
      color: #111111;
    }
    
    /* T01-C13: 링크의 시각적 명확성 및 대비 확보 */
    a {
      color: #004488; /* 파란색을 더 진하게 해서 배경색과의 대비율을 높임 */
      text-decoration: underline; /* 색맹/색약 사용자도 링크임을 알 수 있게 밑줄 추가 */
      font-weight: bold;
    }
    /* T01-C14: Tab 키 이동 시 포커스가 명확히 보이도록 설정 */
    a:focus, button:focus, [tabindex]:focus {
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
      background: #ffffff; /* 카드 배경을 흰색으로 해서 텍스트 대비 확보 */
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
      background: #f4f1ec; /* 근거 영역도 대비 확보 */
      border-left: 4px solid #6c6357;
      padding: 0.5rem 0.8rem;
      color: #222222;
    }

    @media (max-width: 900px) {
      .first-screen {
        grid-template-columns: 1fr;
      }
    }

    .contact {
      background: #ffffff;
      border: 1px solid #d0c9bd;
      border-radius: 8px;
      padding: 1rem;
      margin-top: 2rem;
    }
  </style>
</head>
<body>

  <!-- T01-C15: 제목 단계는 h1 -> h2 -> h3 순서로 건너뛰지 않음 -->
  <h1>안녕, 나는 [네 이름]이야</h1>
  <p class="subtitle"> AI를 배우는 사람.</p>

  <div class="first-screen">

    <div class="card">
      <h3>[강점/취향 1]</h3>
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

  <h2>경험</h2>
  <p>
    - [조교/알바 경험을 한 줄로]<br>
    - [그 경험에서 배운 것을 한 줄로]
  </p>

  <h2>지금 배우는 것</h2>
  <p>
    Python · AI 기초 · 웹 만들기<br>
    [지금 하고 있는 공부나 프로젝트를 한 줄로]
  </p>

  <h2>앞으로</h2>
  <p>
    [되고 싶은 것 / 해보고 싶은 것을 한 줄로]
  </p>

  <h2>연락</h2>
  <div class="contact">
    <p>
      GitHub: <a href="https://github.com/[네아이디]">github.com/[네아이디]</a><br>
      Email: <a href="mailto:[네 이메일]">[네 이메일]</a>
    </p>
  </div>

</body>
</html>
