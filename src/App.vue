<template>
  <div id="app">
    <div id="nav">
      <div id="home">
        <router-link to="/">Hieroglyphics</router-link>
      </div>
      <div>
        <router-link to="/follow">Follow</router-link>
      </div>

      <div>
        <router-link to="/write">Write</router-link>
      </div>
      <div>
        <button>sign in</button>
      </div>
      <div>
        <router-link to="/getstarted">
          <button>get started</button>
        </router-link>
      </div>
    </div>
    <router-view />
  </div>
</template>

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
}

#nav {
  // width: 100%;
  height: 8%;
  padding: 10px;
  display: flex;
  align-items: center;
  background: #f3e40f;
  // box-shadow: 0px 5px 15px #cccccc;
  #home {
    // flex: 5;
    width: 60vw;
    min-width: 30vw;
    font-size: 2rem;
    font-family: Georgia, 'Times New Roman', Times, serif;
  }
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
  text-decoration: none;
  padding: 1rem;
}

button {
  outline: none;
  border: 2px solid #2c3e50;
  width: 9.5rem;
  height: 8vh;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
