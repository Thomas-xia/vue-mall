<template>
  <div class="home_recommends">
    <div class="home_recommends_item" v-for="(item, index) in recommends" :key="index">
      <a :href="item.link">
        <img :src="item.image" alt />
        <div>{{item.title}}</div>
      </a>
    </div>
  </div>
</template>
<script>
export default {
  props: ['recommends'],
  data () {
    return {}
  },
  mounted () {},
  methods: {}
}
</script>
<style scoped>
.home_recommends {
  display: flex;
  text-align: center;
  padding: 10px 0 20px;
  font-size: 12px;
  border-bottom: 10px solid #eee;
}

.home_recommends_item {
  flex: 1;
}

.home_recommends_item img {
  width: 70px;
  height: 70px;
  margin-bottom: 10px;
}
</style>
