<script setup></script>

<template>
  <div class="logo-bg-edge">
    <div class="logo-bg">
      <img src="../../public/ravens.svg" alt="ravens logo" class="logo vue" />
    </div>
  </div>
</template>

<style scoped>
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
  width: 40%;
}
</style>
