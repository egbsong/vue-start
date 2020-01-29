<template>
  <v-app id="app">
    <!-- Header -->
    <Header />

    <!-- Main -->
    <div id="main" role="main">
      <router-view />
    </div>

    <!-- Footer -->
    <Footer />
  </v-app>
</template>

<script>
import Header from '@/components/Header'
import Footer from '@/components/Footer'

export default {
  components: {
    Header,
    Footer
  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css?family=Ubuntu:400,500,700&display=swap');
$bg-white: #ffffff;
$font-white: #ffffff;

#app {
  background-color: $bg-white;
  font-family: 'Ubuntu', sans-serif;
  text-align: center;
  // width: 100%;
  // overflow: hidden;

  * {
    box-sizing: border-box;
    padding: 0;
    margin: 0;
  }

  #main {
    margin-top: 80px;
  }

  section {
    width: 100%;
  }

  .content {
    width: 1200px;
    margin: 0 auto;
  }

  h1 {
    font-size: 56px;
  }

  h2 {
    font-size: 48px;
  }

  h3 {
    font-size: 32px;
  }

  h4 {
    font-size: 24px;
  }

  h5 {
    font-size: 20px;
  }

  h6 {
    font-size: 18px;
  }

  p {
    font-size: 16px;
  }

  a {
    text-decoration: none;
    color: $font-white;
  }

  strong {
    font-size: 12px;
    font-weight: normal;
  }

  em {
    font-size: 12px;
    font-style: normal;
  }

  li {
    list-style: none;
  }
}
</style>
