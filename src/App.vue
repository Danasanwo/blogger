<template>
  <div id="app">
    <Signup />
    <div id="nav">
      <div id="home">
        <router-link to="/">Hieroglyphics</router-link>
      </div>

      <div id="follow">
        <router-link to="/follow">Follow</router-link>
      </div>

      <div id="write">
        <router-link to="/write">Write</router-link>
      </div>
      <div id="sign-in">
        <button>sign in</button>
      </div>
      <div id="started">
        <router-link to="/getstarted">
          <button>get started</button>
        </router-link>
      </div>
    </div>
    <router-view />
  </div>
</template>

<script>
import Signup from '@/components/Signup.vue'
export default {
  components: {
    Signup
  }
}
</script>
<style lang="scss">
*,
*::before,
*::after {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background-color: #f4f6ff;
}

#nav {
  // width: 100%;
  height: 8%;
  padding: 10px;
  display: flex;
  position: sticky;
  top: 0;
  align-items: center;
  background: #f3c623;
  // box-shadow: 0px 5px 15px #cccccc;
  #home {
    // flex: 5;
    width: 60vw;
    min-width: 30vw;
    font-size: 2rem;
    font-family: Georgia, 'Times New Roman', Times, serif;
  }
  #started {
    button {
      background-color: #10375c;
      color: #f4f6ff;
    }
  }
}

#nav a {
  font-weight: bold;
  color: #10375c;
  text-decoration: none;
  padding: 1rem;
}

button {
  outline: none;
  border: 2px solid #10375c;
  width: 9rem;
  height: 2.5rem;
}

#nav a.router-link-exact-active {
  color: #10375c;
}

@media screen and (max-width: 850px) {
  html,
  body {
    font-size: 13px;
  }
  #follow,
  #sign-in,
  #write {
    display: none;
  }
}

@media screen and (max-width: 850px) {
  html,
  body {
    font-size: 11px;
  }
}
</style>
