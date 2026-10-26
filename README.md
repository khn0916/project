<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>나의 한 페이지</title>
  <style>
    /* ① 배경색을 아이보리로 */
    body {
      font-family: sans-serif;
      max-width: 1100px; /* 큰 모니터에서도 안정감 있게 */
      margin: 0 auto;
      padding: 30px 20px;
      line-height: 1.7;
      color: #333;
      background-color: ivory; /* 아이보리 */
    }
    h1 {
      font-size: 2.2rem;
      margin-bottom: 0.2rem;
    }
    .subtitle {
      color: #777;
      margin-top: 0;
    }
    h2 {
      margin-top: 2rem;
      margin-bottom: 0.5rem;
      border-bottom: 2px solid #ddd;
      padding-bottom: 0.3rem;
    }
    a {
      color: #0066cc;
    }

    /* ② 첫 화면에 소개·활동·근거가 다 보이게 하는 그리드 */
    .first-screen {
      display: grid;
      grid-template-columns: 1fr 1fr 1fr; /* 3칸 */
      gap: 20px;
      margin-top: 1.5rem;
    }
    .card {
      background: #fff;
      border: 1px solid #eee;
      border-radius: 8px;
      padding: 1.2rem;
      box-shadow: 0 1px 3px rgba(0,0,0,0.05);
    }
    .card h3 {
      margin-top: 0;
      font-size: 1.1rem;
      color: #222;
    }
    .sar {
      font-size: 0.9rem;
      color: #555;
      margin-bottom: 0.8rem;
    }
    .sar strong {
      color: #222;
    }
    .evidence {
      font-size: 0.85rem;
      background: #f7f7f7;
      border-left: 3px solid #ccc;
      padding: 0.5rem 0.8rem;
      color: #444;
    }

    /* ③ 화면이 작을 때(좁은 화면)는 1칸으로 */
    @media (max-width: 900px) {
      .first-screen {
        grid-template-columns: 1fr;
      }
    }

    .contact {
      background: #fff;
      border: 1px solid #eee;
      border-radius: 8px;
      padding: 1rem;
      margin-top: 2rem;
    }
  </style>
</head>
<body>

  <!-- 첫인상 -->
  <h1>안녕, 나는 [네 이름]이야</h1>
  <p class="subtitle">조교와 알바를 하며 사람을 돕는 일을 좋아하는, 지금 AI를 배우는 사람.</p>

  <!-- ④ 첫 화면: 강점/취향 3개 (SAR + 근거) -->
  <div class="first-screen">

    <!-- 강점 1 -->
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

    <!-- 강점 2 -->
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

    <!-- 강점 3 -->
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

  <!-- ⑤ 나머지: 경험, 배우는 것, 앞으로 -->
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

  <!-- ⑥ 연락 -->
  <h2>연락</h2>
  <div class="contact">
    <p>
      GitHub: <a href="https://github.com/[네아이디]">github.com/[네아이디]</a><br>
      Email: [네 이메일]
    </p>
  </div>

</body>
</html>

  </div>

</body>
</html>
