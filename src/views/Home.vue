<template>
  <div id="home" align="center">
    <nav-top />
    <div class="center">
      <menu-card v-show="true"/>
      <demand-list v-show="false"/>
      <info v-show="false"/>
    </div>
  </div>
</template>

<script>
import navTop from "../components/navTop";
import menuCard from "../components/menuCard";
import demandList from "../components/demandList";
import info from "../components/info"
export default {
  components: {
    navTop,menuCard,demandList,info
  },
};
</script>

<style scoped>
#home {
  background-color: white;
  background-position: center;
  height: 100%;
  width: 100%;
  background-size: cover;
  position: fixed;
}
.center {
  /* background-color: aqua; */
  height: 100%;
  width: 1600px;
}
</style>