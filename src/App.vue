<template>
  <div class="container">
    <h1 class="title">🌌 나만의 앱 아이디어 11선</h1>

    <div class="grid">
      <div v-for="(app, index) in apps" :key="index" class="card">
        <h2 class="card-title">{{ app.title }}</h2>
        <p class="card-desc">{{ app.description }}</p>
      </div>
    </div>

    <footer class="footer">
      © 2025 My Gentle Projects – Crafted with 💡
    </footer>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      apps: [
        { title: "🎨 비주얼 To-Do 앱", description: "감정 기반 색상과 연동된 캘린더와 할 일 추적 기능" },
        { title: "🔮 하루 운세 리포트", description: "타로/주역/심리학 기반으로 하루의 흐름을 예측해주는 리포트" },
        { title: "🧘 마음챙김 AI 코치", description: "스트레스 추적, 호흡 안내 및 명상 가이드" },
        { title: "📚 독서 추적기", description: "읽은 책을 시각화하고 AI와 독서 토론을 할 수 있는 기능" },
        { title: "🤖 나만의 캐릭터 AI", description: "성장형 감성 AI 비서로 나의 감정과 일상을 함께함" },
        { title: "🧭 명언 검색 앱", description: "명언의 의미, 배경, 인용자 정보를 정리해주는 탐색 앱" },
        { title: "📘 영어 단어 암기장", description: "이미지와 문맥 기반으로 단어를 연상하고 기억하는 AI 도우미" },
        { title: "🎓 개인 학습 AI 튜터", description: "개인 학습 스타일 분석 후 맞춤형 콘텐츠 제공" },
        { title: "📈 주가 예측 앱", description: "GPT와 금융 데이터의 융합을 통한 주가 예측 및 분석" },
        { title: "💼 스마트 투자 포트폴리오 빌더", description: "위험도에 맞는 투자전략 + 초보자 가이드 제공" },
        { title: "🛍️ AR 쇼핑 어시스턴트", description: "제품 정보, 가격 비교, 가상 피팅을 도와주는 쇼핑 파트너" }
      ]
    }
  }
}
</script>

<style>
body {
  margin: 0;
  padding: 0;
  font-family: 'Helvetica Neue', sans-serif;
  background-color: #f0f2f5;
  color: #111827;
}

.container {
  max-width: 1000px;
  margin: 0 auto;
  padding: 60px 20px;
}

.title {
  text-align: center;
  font-size: 2.5rem;
  color: #111827;
  margin-bottom: 40px;
}

.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 20px;
}

.card {
  background-color: #ffffff;
  border: 1px solid #ddd;
  border-radius: 12px;
  padding: 20px;
  transition: box-shadow 0.3s ease;
}

.card:hover {
  box-shadow: 0 6px 18px rgba(0, 0, 0, 0.1);
}

.card-title {
  font-size: 1.2rem;
  color: #3b82f6;
  margin-bottom: 10px;
}

.card-desc {
  font-size: 0.95rem;
  color: #333;
}

.footer {
  text-align: center;
  font-size: 0.85rem;
  color: #777;
  margin-top: 60px;
}
</style>
