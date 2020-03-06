<template>
  <div class="track">
    <slot />
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class Track extends Vue {
  @Prop() private msg!: string;
}
</script>

<style scoped>
.track {
  margin-top: auto;
  width: 100vw;
  height: 200px;
  background: tomato;
}
</style>
