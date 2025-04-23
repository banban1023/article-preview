<template>
  <div class="app">
    <div class="card">
      <div class="pic">
        <img src="./assets/drawers.jpg" alt="">
      </div>
      <div class="content">
        <h2>
          Shift the overall look and feel by adding these wonderful
          touches to furniture in your home
        </h2>

        <article>
          Ever been in a room and felt like something was missing? Perhaps
          it felt slightly bare and uninviting. I’ve got some simple tips
          to help you make any room feel complete.
        </article>

        <div class="info">
          <div class="propic">
            <img src="./assets/avatar-michelle.jpg" alt="">
          </div>
          <div class="msg">
            <div class="name">
              Michelle Appleton
            </div>
            <div class="date">
              28 Jun 2020
            </div>
          </div>

          <div class="isShow" @click="isShow">
            <a href="#"></a>
          </div>
        </div>
      </div>
      <div class="share" :class="{ismove: ismove}" v-show="isvisible">
        <p>SHARE</p>
        <div class="btn">
          <div class="icon">
            <img src="./assets/icon-facebook.svg" alt="">
          </div>
          <div class="icon">
            <img src="./assets/icon-twitter.svg" alt="">
          </div>
          <div class="icon">
            <img src="./assets/icon-pinterest.svg" alt="">
          </div>
        </div>
        <div class="noshare" @click="isShow">
          <a href="#"></a>
        </div>
      </div>
    </div>
    <div class="attribution">
      Challenge by <a href="https://www.frontendmentor.io?ref=challenge" target="_blank">Frontend Mentor</a>.
      Coded by <a href="#">banban</a>.
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      isvisible: false,
      ismove: false
    }
  },
  methods: {
    isShow () {
      this.ismove = !this.ismove
      this.isvisible = !this.isvisible
    }
  }
}
</script>

<style lang="less">
@import '@/style/style.less';
</style>
