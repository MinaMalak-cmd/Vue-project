<template>
  <div class="about">
    <h1>دورات ال Vue Js framework</h1>
    <CardComponent />
  </div>
</template>
<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import CardComponent from "@/components/CardComponent.vue";

@Component({
  components: {
    CardComponent
  }
})
export default class ContactView extends Vue {}
</script>
<style lang="scss" scoped>
.about {
  direction: rtl;
  text-align: rtl;
}
</style>
