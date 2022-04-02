//
<template>
  //
  <div class="hello">
    //
    <h1>Card Component</h1>
    //
  </div>
  //
</template>
//
<script lang="ts">
// import { Component, Prop, Vue } from 'vue-property-decorator';

// @Component
// export default class CardComponent extends Vue {
// //   @Prop() private msg!: string;
// }
//
</script>
<template>
  <b-container class="card">
    <b-row>
      <b-col>
        <div>
          <b-card
            title=""
            img-src="https://i.ytimg.com/vi/wTWY0n97vuE/hqdefault.jpg?sqp=-oaymwEbCKgBEF5IVfKriqkDDggBFQAAiEIYAXABwAEG&rs=AOn4CLAhM5y5G2EPQFmJLzBw1SB1hsBVhg"
            img-alt="Image"
            img-top
            tag="article"
            class="mb-2"
          >
            <b-card-text class="card--header"> من الصفر إلي الاحتراف VueJS 2 </b-card-text>
            <hr />
            <b-card-text> إحصائيات اليوتيوب <i class="fi fi-brands-youtube"></i></b-card-text>
           <hr />
           <ul>
             <li>1</li>
             <li>1</li>
             <li>1</li>
             <li>1</li>
             <li>1</li>
           </ul>
             <b-button>Button</b-button>
          </b-card>
        </div>
      </b-col>
      <b-col>
        2
      </b-col>
      <b-col>
       3
      </b-col>
    </b-row>
  </b-container>
</template>

<script lang="ts">

export default {
  data() {
    return {};
  },
  methods: {},
};
</script>
<style lang="scss" scoped>
.card {
  direction: rtl;
  text-align: rtl;
  border:none;
}
 .card--header{
    text-align:start;
 }
</style>
