<template>
  <div class="tasks">
    <div class="container">
      <div id="app">
        <div class="player-container">
          <vue-core-video-player src="./l.mp4"></vue-core-video-player>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  }
};
</script>

<style scoped>
.container {
  width: 33.3vw;
  border: 1px solid white;
  height: 100vh;
  border-top: none;
  border-left: none;
  border-right: none;
}
</style>