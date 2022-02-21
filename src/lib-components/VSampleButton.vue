<template>
   <v-btn @click="clickMe" color="primary">{{ buttonText }}</v-btn>
</template>

<script lang="ts">
import {Component, Emit, Prop, Vue} from 'vue-property-decorator';
import {VBtn} from "vuetify/lib/components";

@Component({ name: 'VSampleButton',
  components: {VBtn}
})
export default class VSampleButton extends Vue {

  @Prop({default: "Click Me"})
  buttonText!: string;

  @Emit("clickMe")
  clickMe(): string {
    return "clicked";
  }

}
</script>
