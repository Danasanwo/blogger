<template>
  <div class="home">
    <div class="loader">
      <p>Read.</p>
      <p>Write.</p>
      <p>Express.</p>
    </div>
    <div id="start">
      <h1>Expand your horizon.</h1>

      <button>Get started</button>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Home',
  components: {}
}
</script>

<style lang="scss" scoped>
.loader {
  width: 100%;
  background: url('../../public/images/pattern.jpg');
  background-size: cover;
  p {
    font-size: 8rem;
    color: #f3c623;
  }
}

#start {
  width: 100%;
  h1 {
    margin: auto;
    text-align: center;
  }
  button {
    margin: 25px 45%;
  }
}

img {
  width: 100%;
  height: 100vh;
}
</style>
