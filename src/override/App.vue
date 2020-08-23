<template>
  <div>
    <p>The game of life biiitch!</p>
    <game-of-life />
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import HelloWorld from '@/components/HelloWorld.vue';
import GameOfLife from '@/components/game-of-life/GameOfLife.vue';
import { Component } from 'vue-property-decorator';

@Component({
  components: { HelloWorld, GameOfLife }
})
export default class App extends Vue {}
</script>
