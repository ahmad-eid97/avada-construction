<template>
  <section class="count-container">
    <div class="count"></div>
    <div class="count-inner">
      <div class="count-sperator">
        <svg
          class="fusion-big-half-circle-candy"
          xmlns="http://www.w3.org/2000/svg"
          version="1.1"
          width="100%"
          height="100"
          viewBox="0 0 100 100"
          preserveAspectRatio="none"
          style="padding: 0"
          fill="rgba(255,255,255,1)"
        >
          <path d="M0 0 C55 180 100 0 100 0 Z"></path>
        </svg>
      </div>
      <div class="count-content">
        <div class="row justify-content-around">
          <div class="count-item col-sm-6 col-lg-3">
            <font-awesome-icon icon="fa-solid fa-suitcase" />
            <span class="display-counter">
              <VueJsCounter
                class="d-inline"
                :startVal="0"
                :endVal="4205"
                separator=","
              ></VueJsCounter>
            </span>
            <div class="counter-text">PLANNING APPLICATIONS</div>
          </div>
          <div class="count-item col-sm-6 col-lg-3">
            <font-awesome-icon icon="fa-solid fa-building" />
            <span class="display-counter">
              <VueJsCounter
                class="d-inline"
                :startVal="0"
                :endVal="896"
                separator=","
              ></VueJsCounter>
            </span>
            <div class="counter-text">PLANNING APPLICATIONS</div>
          </div>
          <div class="count-item col-sm-6 col-lg-3">
            <font-awesome-icon icon="fa-solid fa-users" />
            <span class="display-counter">
              <VueJsCounter
                class="d-inline"
                :startVal="0"
                :endVal="172"
                separator=","
              ></VueJsCounter>
            </span>
            <div class="counter-text">PLANNING APPLICATIONS</div>
          </div>
          <div class="count-item col-sm-6 col-lg-3">
            <font-awesome-icon icon="fa-solid fa-globe" />
            <span class="display-counter">
              <VueJsCounter
                class="d-inline"
                :startVal="0"
                :endVal="19"
                separator=","
              ></VueJsCounter>
            </span>
            <div class="counter-text">PLANNING APPLICATIONS</div>
          </div>
        </div>
      </div>
      <div class="count-sperator">
        <svg
          class="fusion-big-half-circle-candy"
          xmlns="http://www.w3.org/2000/svg"
          version="1.1"
          width="100%"
          height="100"
          viewBox="0 0 100 100"
          preserveAspectRatio="none"
          style="padding: 0"
          fill="rgba(255,255,255,1)"
        >
          <path d="M0 100 C40 0 60 0 100 100 Z"></path>
        </svg>
      </div>
    </div>
  </section>
</template>

<script>
import VueJsCounter from "vue-count-to";

export default {
  name: "AppHomeCount",
  components: {
    VueJsCounter
  },
  data() {
    return {};
  },
};
</script>
<style lang="scss">
.count-container {
  background-color: rgba(255, 255, 255, 0);
  background-position: center center;
  background-repeat: no-repeat;
  border-width: 0px;
  border-color: var(--awb-color2);
  border-style: solid;
  background-size: cover;
  position: relative;
  overflow: hidden;
  z-index: 1;
  background-image: none;
  padding-top: 0px;
  margin-top: 0px;
  padding-bottom: 0px;
  margin-bottom: 0px;
}
.count {
  pointer-events: none;
  width: 100%;
  height: 100%;
  position: absolute;
  z-index: -1;
  top: 0px;
  left: 0px;
  opacity: 1;
  background-position: center center;
  background-repeat: no-repeat;
  background-size: cover;
  background-image: url("https://avada.theme-fusion.com/construction/wp-content/uploads/sites/55/2015/12/home-244125289.jpg");
  min-height: 150px;
  background-attachment: fixed;
}
.count-inner .count-sperator {
  width: 100wv;
}
.count-content {
  margin-top: 100px;
  margin-bottom: 55px;
  padding: 30px;
}
.count-item  {
  margin-bottom: 40px;
}
.count-item svg {
  font-size: 70px;
  color: var(--main-color);
}
.count-item .display-counter {
  display: block;
  font-size: 60px;
  color: var(--main-color);
  font-weight: 600;
}
@include xs {
  .count-item svg {
    font-size: 40px;
  }
  .count-item .display-counter {
    font-size: 40px;
  }
}
.count-item .counter-text {
  display: block;
  font-size: 16px;
  color: #fff;
  font-weight: 600;
}
</style>
