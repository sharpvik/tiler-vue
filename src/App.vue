<template>
  <main id="main">
    <div class="main-col" width="230px"><Ava /></div>
    <div class="main-col" width="230px">Menu</div>
    <div class="main-col" width="230px">Menu</div>
    <div class="main-col" width="60px"><Corner /></div>
  </main>
</template>

<script>
import Ava from "./components/Ava";
import Corner from "./components/Corner";

export default {
  name: "App",
  components: {
    Ava,
    Corner,
  },
};
</script>

<style>
* {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  padding: 0;
  margin: 0;
  outline: none;
}

#main {
  height: 100vh;
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  align-items: center;
}

.main-col {
  height: calc(100% - 20px);
}

.tile {
  background-color: #282a36;
  border-radius: 10px;
  overflow: hidden;
}
</style>
