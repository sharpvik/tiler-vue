<template>
  <button @click="close">
    <p><span class="material-icons"> close </span></p>
  </button>
</template>

<script>
import "../../node_modules/material-design-icons/iconfont/material-icons.css";

export default {
  name: "Corner",
  methods: {
    close() {
      console.log(window.electron);
      window.electron.ipcRenderer.send("quit");
    },
  },
};
</script>

<style scoped>
button {
  border: none;
  background-color: rgb(255, 66, 66);
  width: 60px;
  height: 60px;
  border-radius: 10px;
  cursor: pointer;
}

p {
  text-align: center;
  color: white;
}

span {
  font-size: 28px;
  line-height: 60px;
}
</style>
