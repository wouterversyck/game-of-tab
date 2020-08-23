<template>
  <div id="Game__game-container"></div>
</template>

<script lang="ts">
import Vue from 'vue';
import { Component } from 'vue-property-decorator';
import Game from './Game';

@Component
export default class HelloWorld extends Vue {
  mounted() {
    browser.runtime.sendMessage({});
    new Game();
  }
}
</script>

<style scoped>
p {
  font-size: 20px;
}
</style>
