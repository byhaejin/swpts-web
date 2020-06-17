<template>
  <div class="app">
    <header ref="header">
      <div class="header" :class="{ 'scroll': isTopScroll }">
        <div class="container row">
          <div class="header__info">
            <div class="logo">
              <a class="hand" v-scroll-to="'#intro'">
                <img alt="SW TPS" src="@/assets/images/sw-logo.png" />
              </a>
            </div>
            <div class="title">
              <a class="hand" v-scroll-to="'#intro'">
                성원 TPS
              </a>
            </div>
            <div class="hamburger">
              <button type="button"
                      class="btn menu-trigger"
                      :class="{ active:isMbMenu }"
                      @click="toggleMobileMenu">
                <span> </span>
                <span> </span>
                <span> </span>
              </button>
            </div>
          </div>

          <nav>
            <ul class="top-nav" :class="{ 'on': isMbMenu }">
              <li v-for="item in aryMenu" :key="item.id">
                <a class="hand"
                   :class="{on: item.id === aryMenuSelected }"
                   @click="handleLocation(item.id)">
                  {{ item.name }}
                </a>
              </li>
            </ul>
          </nav>
        </div>
      </div>
    </header>

    <router-view/>

    <footer>
      <div id="footer" class="footer">
        <div class="contents">
          <ul>
            <li class="footer-info">
              <address>(주)성원TPS ㅣ 주소: 서울시 강서구 양천로 551-24, 한화비즈메트로2차 1307호</address>
              대표이사: 이영철 ㅣ 사업자등록번호: 669-87-00775 ㅣ Tel: 02-2013-8610
              <p class="copyright">
                © 2018 Seongwon TPS Inc. All Rights Reserved
              </p>
            </li>
            <li class="footer-social">
              <h5>Follow Us</h5>
              <ul>
                <li>
                  <a href="https://www.facebook.com/pg/성원TPS-516889785440906/" target="_blank">
                    <img alt="facebook" src="@/assets/images/icon-facebook.png" />
                  </a>
                </li>
                <li>
                  <a href="https://www.youtube.com/channel/UCSrewwHUnXSAwVkfSww-OmA" target="_blank">
                    <img alt="youtube" src="@/assets/images/icon-youtube.png" />
                  </a>
                </li>
                <li>
                  <a href="http://pf.kakao.com/_GxdLCj" target="_blank">
                    <img alt="kakaotok" src="@/assets/images/icon-kakao.png" />
                  </a>
                </li>
              </ul>
            </li>
          </ul>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>

  export default {
    name: 'app',
    data () {
      return {
        isPC: false,
        isTopScroll: false,
        isMbMenu: false,
        aryMenuSelected: 0,
        staymail: '',
        aryMenu: [
          {id: 'company', name: '성원 TPS'},
          {id: 'product', name: '제품소개'},
          {id: 'performance', name: '실적'},
          {id: 'partner', name: '파트너십'},
          {id: 'estimate', name: '견적문의'},
          {id: 'contact', name: 'CONTACT US'}
        ]
      }
    },
    beforeMount () {
      this.checkWindowWidth()
      window.addEventListener('resize', this.checkWindowWidth)
      window.addEventListener('scroll', this.handleScroll)
    },
    beforeDestroy () {
      window.removeEventListener('resize', this.checkWindowWidth)
      window.removeEventListener('scroll', this.handleScroll)
    },
    methods: {
      checkWindowWidth () {
        this.isPC = (window.innerWidth > 768)
      },
      /**
       * event scroll catch
       * */
      handleScroll () {
        this.isTopScroll = window.scrollY > 0
      },
      /**
       * topmenu scroll
       **/
      handleLocation (targetId) {
        this.isMbMenu = false
        this.$scrollTo(`#${targetId}`)
      },
      /**
       * 모바일 메뉴 활성화 toggle
       * */
      toggleMobileMenu () {
        this.isMbMenu = !this.isMbMenu
      }
    }
  }
</script>

<style lang="scss">
  @import './assets/styles/app.scss';
</style>
