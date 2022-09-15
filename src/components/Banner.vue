<template>
  <div id="main-banner"></div>
</template>

<script>
  export default {
    name: "Banner"
  }
</script>

<style scoped>

  #main-banner {
    background-image: url('/img/banner.png');
    background-size: cover;
    height: 142px;
    width: 360px;
    top: 16px;
    border-radius: 0px;
    justify-content: center;
    position: absolute;
    left: 50%;
    display: block;
    transform: translate(-50%, 0%);
  }


</style>