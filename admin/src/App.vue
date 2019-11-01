<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";

import Vue from "vue";
import {
  MdButton,
  MdCard,
  MdContent,
  //  MdTabs,
  MdDatepicker,
  MdDivider,
  MdField,
  //  MdIcon,
  MdImage,
  MdProgress,
  MdSubheader
  //  MdList,
} from "vue-material/dist/components";
import "vue-material/dist/vue-material.min.css";
import "vue-material/dist/theme/default.css";

Vue.use(MdButton);
Vue.use(MdCard);
Vue.use(MdContent);
Vue.use(MdDatepicker);
Vue.use(MdDivider);
Vue.use(MdField);
Vue.use(MdImage);
Vue.use(MdProgress);
Vue.use(MdSubheader);

export default {
  name: "app",
  components: {
    HelloWorld
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
