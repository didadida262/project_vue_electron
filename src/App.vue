<template>
  <div id="app">
    <div class="left">
      First in DOM, no order applied
    </div>
    <div class="right">
      Second in DOM, with a larger order
    </div>
  </div>
</template>

<script>

export default {
  name: 'App',
  mounted() {
    console.log('mounted!!!')
  }

}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  width: 100vw;
  height: 100vh;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px;
}
.left {
  border: 1px solid gainsboro;
  width: 150px;
  height: 100%;
}
.right {
  width: calc(100% - 160px);
  border: 1px solid gainsboro;
  height: 100%;

}

</style>
