<template>
  <div id="editor">
    <button @click="onClick" />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component
export default class HelloWorld extends Vue {
  private onClick() {
    window.alert("clicked");
  }
}
</script>
