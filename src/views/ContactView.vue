<template>
  <div class="about">
    <CardComponent heading="دورات ال Vue Js framework" :data="course"/>
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
export default class ContactView extends Vue {
  data() {
    return {
      course: {
        id: "PL1FWK-sgJ9ek59ylOuaS8Ggjz9oBVM8Hb",
        name: "VueJS \u0625\u0633\u0623\u0644\u0646\u064a \u0639\u0646",
        url:
          "https://www.youtube.com/watch?v=TQQVt3CbSCw&list=PL1FWK-sgJ9ek59ylOuaS8Ggjz9oBVM8Hb",
        description: "",
        thumbnails: "https://i.ytimg.com/vi/TQQVt3CbSCw/sddefault.jpg",
        statistics: {
          viewCount: 111,
          likeCount: 11,
          commentCount: 7,
          duration: "00:04:18",
          lessons: 2
        }
      }
    };
  }
}
</script>
<style lang="scss" scoped>
.about {
  direction: rtl;
  text-align: rtl;
}
</style>
