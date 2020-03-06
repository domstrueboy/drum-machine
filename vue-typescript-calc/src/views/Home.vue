<template>
  <div class="home">
    <Display msg="100"/>
  </div>
</template>

<script>
import Display from '@/components/Display.vue';

export default {
  name: 'Home',
  components: {
    Display,
  },
};
</script>

<style>
.home {
  max-width: 480px;
  height: 100vh;
  box-sizing: border-box;
  margin: 0 auto;
  background: black;
  padding: 10px;
}
</style>
