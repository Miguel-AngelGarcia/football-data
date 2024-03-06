<script setup>
import TeamView from "./TeamView.vue";
import TeamChart from "./TeamChart.vue";
</script>

<template>
  <div class="team-hero">
    <TeamView />
    <TeamChart />
  </div>
</template>

<style scoped>
.team-hero {
  width: 100%;
  height: 500px;
  position: relative;
  background-color: red;
  display: flex;
}

.logo {
  height: 200px;
  width: 200px;
  will-change: filter;

  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}

.logo-bg {
  background-color: blanchedalmond;
  height: 100%;
  widows: 100%;
}

.logo-bg-edge {
  border-radius: 10px;
  overflow: hidden;
  display: flex;
  flex-direction: column;
}
</style>
