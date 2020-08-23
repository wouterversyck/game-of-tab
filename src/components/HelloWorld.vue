<template>
  <div>
    <p>{{ defaultText }}</p>
    <p>yes</p>
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import { Component } from 'vue-property-decorator';

@Component
export default class HelloWorld extends Vue {
  mounted() {
    browser.runtime.sendMessage({});
  }

  get defaultText() {
    return browser.i18n.getMessage('extName');
  }
}
</script>

<style scoped>
p {
  font-size: 20px;
}
</style>
