<template>
  <hello-world />
</template>

<script lang="ts">
import Vue from 'vue';
import HelloWorld from '@/components/HelloWorld.vue';
import { Component } from 'vue-property-decorator';

@Component({
  components: { HelloWorld }
})
export default class App extends Vue {}
</script>

<style>
html {
  width: 400px;
  height: 400px;
}
</style>
