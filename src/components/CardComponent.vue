<template>
    <span>
    <b-alert show class="w-50 m-auto">{{heading}}</b-alert>
    <b-container class="card my-5">
        <b-row>
        <b-col>
            <div>
            <b-card
                :title="data.name"
                :img-src="data.thumbnails"
                img-alt="Image"
                img-top
                tag="article"
                class="mb-2"
            >
                <!-- <b-card-text class="card--header">من الصفر إلي الاحتراف VueJS 2</b-card-text> -->
                <hr />
                <b-card-text class="card--desc">
                <i class="fab fa-youtube card--desc--icon"></i>
                إحصائيات اليوتيوب
                </b-card-text>
                <hr />
                <ul class="card--list">
                <li>
                    <i class="fas fa-bars"></i> {{data.statistics.lessons}} درس
                </li>
                <li>
                    <i class="far fa-clock"></i> {{data.statistics.duration}}
                </li>
                <li>
                    <i class="far fa-play-circle"></i> {{data.statistics.viewCount}} مشاهدة
                </li>
                <li>
                    <i class="far fa-thumbs-up"></i> {{data.statistics.likeCount}} إعجاب
                </li>
                <li>
                    <i class="far fa-comments"></i> {{data.statistics.commentCount}} تعليق
                </li>
                </ul>
                <b-link class="w-100 btn btn-primary " :href="data.url" active-class target="blank">شاهد الآن</b-link>
            </b-card>
            </div>
        </b-col>
        <b-col>2</b-col>
        <b-col>3</b-col>
        </b-row>
    </b-container>
    </span>
</template>
<script lang="ts">
export default {
  name:"Card",
  data() {
    return {};
  },
  props: {
    heading: {
      required: true,
      type: String,
      default: ''
    },
    data: {
      required: true,
      type: Object,
      default: {}
    }
  },
  //   created(){
  //       fetch("@/data/courses.json")
  //       .then(res=>console.log(res.json()))
  //       .catch(e=>console.log(e))
  //   },
  methods: {},
};
</script>
<style lang="scss" scoped>
.card {
  direction: rtl;
  text-align: rtl;
  border: none;
}
.card--header {
  text-align: start;
}
.card--list {
  list-style-type: none;
  padding: 0;
}
.card--list li {
  text-align: start;
}
.card--desc {
  text-align: start;
}
.card--desc--icon {
  color: red !important;
}
</style>
