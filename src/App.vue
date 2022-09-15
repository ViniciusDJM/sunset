<template>
  <div id="background">
    <Navbar :logo="logo_src" :alt="app_name" />
    <div>
      <router-view></router-view>
    </div>
    <section> 
      <div id="video"> 
        <iframe width="560" height="315" src="https://www.youtube.com/embed/IQw-4JABPCM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
      </div>
    </section>
    <Footer />
  </div>
</template>
<script>

import Footer from './components/Footer'


export default {
  data: function() {
    return {
      logo_src: "/img/logo.png",
      app_name: "Sunset"
    }
  },
  components: {
    Footer,
  }
}
</script>

<style>
  * {
    font-family: Helvetica;
    padding: 0;
    margin: 0;
    box-sizing: border-box;
    background-image: url('/img/background.png');
    background-attachment: fixed;
    background-position: center;
  }

  #video{
    left: 32%;
    top: 30%;
    justify-content: center;
    position: absolute;
  }
  

  .main-container {
    margin: 50px;
    min-height: 250px;
  }

  h1 {
    text-align: center;
    font-size: 42px;
    margin-bottom: 30px;
    color: #222;
  }
</style>
