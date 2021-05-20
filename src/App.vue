<template>
  <main id="main">
    <div class="main-col"><Ava /></div>
    <div class="main-col">Menu</div>
    <div class="main-col">Menu</div>
    <div class="main-col">Menu</div>
  </main>
</template>

<script>
import Ava from "./components/Ava";
export default {
  name: "App",
  components: {
    Ava,
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
  width: 230px;
  height: calc(100% - 20px);
}

.tile {
  background-color: #282a36;
  border-radius: 10px;
  overflow: hidden;
}
</style>
