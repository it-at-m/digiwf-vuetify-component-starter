
<template>
  <v-app>
    <VSampleButton color="primary" button-text="Sample Button Test"></VSampleButton>
  </v-app>
</template>

<script lang="ts">
import Vue from 'vue';
import {Component} from "vue-property-decorator";
import {VSampleButton} from "@/entry.esm";
@Component({
  components: {VSampleButton}
})
export default class App extends Vue {
}
</script>

