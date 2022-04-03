<template>
  <b-container class="card">
    <b-row>
      <b-col>
        <div>
          <b-card
            title
            img-src="https://i.ytimg.com/vi/wTWY0n97vuE/hqdefault.jpg?sqp=-oaymwEbCKgBEF5IVfKriqkDDggBFQAAiEIYAXABwAEG&rs=AOn4CLAhM5y5G2EPQFmJLzBw1SB1hsBVhg"
            img-alt="Image"
            img-top
            tag="article"
            class="mb-2"
          >
            <b-card-text class="card--header">من الصفر إلي الاحتراف VueJS 2</b-card-text>
            <hr />
            <b-card-text class="card--desc">
              <i class="fab fa-youtube card--desc--icon"></i>
              إحصائيات اليوتيوب
            </b-card-text>
            <hr />
            <ul class="card--list">
              <li>
                <i class="fas fa-bars"></i> 66 درس
              </li>
              <li>
                <i class="far fa-clock"></i> 03:00:00
              </li>
              <li>
                <i class="far fa-play-circle"></i> 16,000 مشاهدة
              </li>
              <li>
                <i class="far fa-thumbs-up"></i> 650 إعجاب
              </li>
              <li>
                <i class="far fa-comments"></i> 96 تعليق
              </li>
            </ul>
            <b-button>Button</b-button>
          </b-card>
        </div>
      </b-col>
      <b-col>2</b-col>
      <b-col>3</b-col>
    </b-row>
  </b-container>
</template>

<script lang="ts">
export default {
  data() {
    return {};
  },
  methods: {}
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
