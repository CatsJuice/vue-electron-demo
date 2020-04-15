<template>
  <div id="app">
    <div class="drag-handler"></div>
    <router-view/>
  </div>
</template>

<style lang="less">

html,
body {
  width: 100%;
  height: 100%;
  overflow: hidden;
  // background-color: #fff;
  margin: 0;
  padding: 0;
  background-color: transparent;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-color: transparent;

  width: 100%;
  height: 100%;

  .drag-handler {
    width: 100%;
    height: 30px;
    background-color: rgba(255,0,0,0);
    z-index: 0;
    position: absolute;
    cursor: pointer;
    -webkit-app-region: drag;
    webkit-user-select: none;

  }
}


#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
