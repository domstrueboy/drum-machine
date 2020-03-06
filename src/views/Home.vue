<template>
  <div class="home">
    <Display msg="100"/>
    <Kick />
    <Track msg="100"/>
  </div>
</template>

<script>
import Display from '@/components/Display.vue';
import Track from '@/components/Track.vue';
import Kick from '@/components/Kick.vue';

export default {
  name: 'Home',
  components: {
    Display,
    Track,
    Kick,
  },
};
</script>

<style>
.home {
  display: flex;
  flex-direction: column;
  width: 100vw;
  height: 100vh;
  box-sizing: border-box;
  background: black;
}
</style>
