<template>
  <div class="home">
    <section id="intro" class="intro" ref="intro">
      <div class="contents">
        <h3>안전한 주차장 진입로</h3>
        <h1>성원TPS</h1>
        <p>"아슬아슬 주차장 진입로,
          초보운전자도 편안하게"</p>
        <button type="button" class="btn btn-round js-contact"
                @click="handleLocation('contact')">
          <span>문의하기</span>
        </button>
      </div>
    </section>
    <section id="company" class="company" ref="company">
      <div class="contents">
        <h2>성원 TPS Inc.</h2>
        <p class="ment">Technological Parking System</p>
        <span class="line"></span>
        <p class="script">
          좁은 주차장 진입로 때문에 고통 받고 계신가요?
          성원 TPS의 VDGS는 주차장 진입로를 쉽게 통과할 수
          있도록 돕는 하드웨어 시스템입니다.
        </p>

        <ul>
          <li>
            <img alt="" src="@/assets/images/company-1.png" />
            <h4>세계 최초
              레이저 가이드 시스템</h4>
          </li>
          <li>
            <img alt="" src="@/assets/images/company-2.png" />
            <h4>초보 운전자도 편안하고
              안전하게 주차장 진입로 통과</h4>
          </li>
          <li>
            <img alt="" src="@/assets/images/company-3.png" />
            <h4>다양한 가이드
              시스템 제공</h4>
          </li>
        </ul>

      </div>
    </section>
    <section id="product" class="product" ref="product">
      <div class="contents">
        <h2>성원 TPS Inc.</h2>
        <span class="line"></span>
        <p class="script">
          <span class="iB">성원 TPS만의 독자적인</span> <span class="iB">레이저 가이드 시스템을 소개합니다.</span>
        </p>

        <div class="cell">
          <div class="video">
            <div class="video-cell">
              <iframe width="100%" height="100%" src="https://www.youtube.com/embed/P-78mkYSYUI?rel=0&playlist=P-78mkYSYUI" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
            </div>
          </div>
          <h4>자동차주행유도시스템 (VDGS)</h4>
          <p><span class="iB">녹색 레이저 라인으로 주차장 진출입로의</span> <span class="iB">"중앙선"을 표시합니다.</span>
            레이저를 차량 데시보드 중앙에 맞추며 운전하면 됩니다.</p>
        </div>

      </div>
    </section>
    <section id="performance" class="performance" ref="performance">
      <div class="contents">
        <h2>성원 TPS의 실적</h2>
        <p class="ment">VDGS 설치 전과 후 비교</p>
        <span class="line"></span>
        <p class="script">
          성원TPS와 함께하는 고객사중 하나인 "코엑스 주차장" VDGS 설치 전, 후 비교 영상입니다.
        </p>
        <ul>
          <li>
            <h3>Before</h3>

            <div class="video">
              <div class="video-cell">
                <iframe width="100%" height="100%" src="https://www.youtube.com/embed/B5UgFEOwM1I?rel=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
              </div>
            </div>
          </li>
          <li>
            <h3>After</h3>

            <div class="video">
              <div class="video-cell">
                <iframe width="100%" height="100%" src="https://www.youtube.com/embed/9xdB_AVALSU?rel=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
              </div>
            </div>
          </li>
        </ul>
        <ul>
          <li>
            <h3>운전자 시각</h3>

            <div class="video">
              <div class="video-cell">
                <iframe width="100%" height="100%" src="https://www.youtube.com/embed/fwN9PG08z6c?rel=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
              </div>
            </div>
          </li>
          <li>
            <h3>블라인드 주행</h3>

            <div class="video">
              <div class="video-cell">
                <iframe width="100%" height="100%" src="https://www.youtube.com/embed/YJiOJ3_gH4s?rel=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
              </div>
            </div>
          </li>
        </ul>
      </div>
    </section>
    <section id="chart" class="chart" ref="chart">
      <div class="contents">
        <h2>확실한 결과를 보여주는 VDGS</h2>
        <h3 class="ment">코엑스 주차장 VDGS 전,후 비교표</h3>
        <div class="chartBox">
          <img alt="" src="@/assets/images/graph.png" />
        </div>
        <p class="script">
          "VDGS를 설치하고나니 어둡고 칙칙하기만 하던
          주차장 진입로가 아름다워져서 고객들 반응이 좋습니다."
        </p>
      </div>
    </section>
    <section id="partner" class="partner" ref="partner">
      <div class="contents">
        <h2>성원 TPS 파트너</h2>
        <p class="ment">성원 TPS과 함께하는 고객사입니다.</p>
        <ul>
          <li><img alt="coex" src="/static/partners/partner-coex.png" /></li>
          <li><img alt="posco" src="/static/partners/partner-posco.png" /></li>
          <li><img alt="severance" src="/static/partners/partner-severance.png" /></li>
          <li><img alt="hyundai" src="/static/partners/partner-hyundai.png" /></li>
          <li><img alt="The-K" src="/static/partners/partner-theK.png" /></li>
        </ul>
      </div>
    </section>
    <section id="estimate" class="estimate" ref="estimate">
      <div class="v-box">
        <div class="contents">
          <h1>오늘부터 접촉사고 끝</h1>
          <p class="ment">당신의 브랜드 이미지 UP, 유저들의 불만 DOWN</p>
          <a href="https://docs.google.com/forms/d/1tD1y5DJ0mPDmVyEfk_V7ORJL1rWTpz7H7MUB4RDYC1o/edit"
             target="_blank"
             class="btn btn-round js-contact">
            <span>견적문의하기</span>
          </a>
        </div>
      </div>
    </section>
    <section id="certificate" class="certificate" ref="certificate">
      <div class="contents">
        <h1>인증서와 보유특허</h1>
        <ul class="list">
          <li>
            <img alt="" src="@/assets/images/authentication_koita.jpg" />
            <h5>벤처기업확인서</h5>
          </li>
          <li>
            <img alt="" src="@/assets/images/authentication_kibo.jpg" />
            <h5>기업부설연구소 인정서</h5>
          </li>
        </ul>
        <ul class="list">
          <li>
            <img alt="" src="@/assets/images/certificate_patent_1.jpg" />
            <p><b>제 10-1799527호</b>
              레이저 광원장치 및 이를 포함하는
              주차 지시등 시스템</p>
          </li>
          <li>
            <img alt="" src="@/assets/images/certificate_patent_2.jpg" />
            <p><b>제 10-1693262호</b>
              자동차 운행 가이드 시스템</p>
          </li>
          <li>
            <img alt="" src="@/assets/images/certificate_patent_3.jpg" />
            <p><b>제 10-1794235호</b>
              주차장 안전거리 유도 장치 및 방법</p>
          </li>
          <li>
            <img alt="" src="@/assets/images/certificate_patent_4.jpg" />
            <p><b>제 10-1561668호</b>
              주차장의 충돌 방지 및 시스템</p>
          </li>
          <li>
            <img alt="" src="@/assets/images/certificate_patent_5.jpg" />
            <p><b>제 10-1931539 호</b>
              곡선형 레이저빔 변환장치</p>
          </li>
          <li>
            <img alt="" src="@/assets/images/certificate_patent_6.jpg" />
            <p><b>제 10-2007799 호</b>
              차량 자율주행 보조 장치 및<br> 이를 포함하는 차량 자율주행 보조 시스템</p>
          </li>
        </ul>

      </div>
    </section>
    <section id="contact" class="contact" ref="contact">
      <div class="contents">
        <h1>VDGS에 대해 더 궁금하신가요?</h1>
        <ol class="contact-target">
          <li>1. 주차장 진입로 때문에 스트레스가 크셨던 분</li>
          <li>2. 건물에 더 많은 방문객을 유치하고 싶으신 분</li>
        </ol>

        <p>문의를 남겨주시면 연락 드리겠습니다.</p>
        <ul>
          <li>
            <h4>전화 문의</h4>
            <a href="tel:02-2013-8610" class="btn btn-round js-contact">
              <span>02-2013-8610</span>
            </a>
          </li>
          <li>
            <h4>이메일 문의</h4>
            <a href="mailto:contact@swtps.com" class="btn btn-round js-contact">
              <span>contact@swtps.com</span>
            </a>
          </li>
        </ul>
      </div>
    </section>
  </div>
</template>

<script>

  export default {
    name: 'Home',
  }
</script>
