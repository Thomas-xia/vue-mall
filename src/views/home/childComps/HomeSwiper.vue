<template>
  <div class="home_swiper">
    <swiper>
    <swiper-item v-for="(item, index) in banners" :key="index">
      <a :href="item.link">
        <img :src="item.image" alt="">
      </a>
    </swiper-item>
  </swiper>
  </div>
</template>
<script>
import { Swiper, SwiperItem } from 'components/common/swiper'

export default {
  name: 'HomeSwiper',
  components: {
    Swiper,
    SwiperItem
  },
  props: ['banners'],
  // props:{
  //   banners: {
  //     type: Array,
  //     default () {
  //       return []
  //     }
  //   }
  // },
  data () {
    return {
    }
  },
  mounted () {
  },
  methods: {
  }
}
</script>
<style lang='less' scoped>
</style>
