<template>
  <div class="container is_fullhd">
    <main-navbar />
    <nuxt />
    <main-footer />
  </div>
</template>

<script>
import MainNavbar from '~/components/MainNavbar'
import MainFooter from '~/components/MainFooter'

export default {
  components: {
    MainNavbar,
    MainFooter
  }
}
</script>

<style>
html {
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

@media(max-width: 500px) {
  .reverse-columns {
    flex-direction: column-reverse;
    display: flex;
  }
}

.rtl {
  direction: rtl !important;
}

.inner-container {
  margin: 0 auto;
  min-height: 100vh;
  min-width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #2c3e50;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}

</style>
