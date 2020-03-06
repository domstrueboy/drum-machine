<template>
  <div class="kick" @click="play">
    <audio data-key="65" src="sounds/clap.wav" ref="sound"></audio>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class Kick extends Vue {
  @Prop() private msg!: string;

  play(): void {
    const sound = this.$refs.sound as HTMLAudioElement;
    sound.play();
  }
}
</script>

<style scoped>
.kick {
  width: 25px;
  height: 25px;
  background: rgb(54, 54, 54);
}
</style>
