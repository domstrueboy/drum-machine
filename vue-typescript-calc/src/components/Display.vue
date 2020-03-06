<template>
  <div class="display">
    {{ msg }}
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class Display extends Vue {
  @Prop() private msg!: string;
}
</script>

<style scoped>
.display {
  background: lightblue;
  border-radius: 5px;
  height: 96px;
  line-height: 96px;
  font-size: 80px;
  font-weight: 100;
}
</style>
