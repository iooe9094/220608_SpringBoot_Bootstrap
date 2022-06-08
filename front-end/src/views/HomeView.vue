<template>
  <div id="page-top">
    <!-- Navigation-->
    <a class="menu-toggle rounded mt-5" href="#"><i class="fas fa-bars"></i></a>
    <nav id="sidebar-wrapper">
      <ul class="sidebar-nav">
        <li class="sidebar-brand"><a href="#page-top">Start Bootstrap</a></li>
        <li class="sidebar-nav-item"><a href="#page-top">Home</a></li>
        <li class="sidebar-nav-item"><a href="#about">About</a></li>
        <li class="sidebar-nav-item"><a href="#services">Services</a></li>
        <li class="sidebar-nav-item"><a href="#portfolio">Portfolio</a></li>
        <li class="sidebar-nav-item"><a href="#contact">Contact</a></li>
      </ul>
    </nav>

    <!-- Header -> HeaerCom.vue로 이동-->
    <HeaderCom></HeaderCom>

    <!-- Section -> SectionCom.vue로 이동 -->
    <SectionCom></SectionCom>

    <!-- Footer -> FooterCom.vue로 이동 -->
    <FooterCom></FooterCom>
  </div>
</template>

<script>
// TODO : bootstrap 테마 js 적용
import loadWin from "@/assets/js/scripts.js";
import FooterCom from "@/components/home/FooterCom.vue";
import HeaderCom from "@/components/home/HeaderCom.vue";
import SectionCom from "@/components/home/SectionCom.vue";

export default {
  name: "HomeView",
  components: { FooterCom, HeaderCom, SectionCom },
  // 화면이 뜨자마자 실행되는 이벤트
  mounted() {
    loadWin();
  },
};
</script>

<style>
/* Todo : bootstrap 테마 사용자 css import */
@import "../assets/css/styles.css";
</style>
