<template>
  <v-app>
    <div>
      <v-textarea
        solo
        name="input-7-4"
        label="いまどうしてる？"
        v-model="text"
      ></v-textarea>
    </div>
    <div>
      <v-btn
        class="white--text"
        color="blue"
        rounded
        :absolute="true"
        :right="true"
        @click="onClick"
        >呟く</v-btn
      >
    </div>
  </v-app>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import * as Constants from "@/constant/Constants";

@Component
export default class Editor extends Vue {
  private text = "";
  private onClick() {
    window.alert(this.text);
  }
}
</script>
