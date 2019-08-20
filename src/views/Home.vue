<template>
  <div class="home">
    <ym-main />
    <bg-img />
  </div>
</template>

<script>
// @ is an alias to /src
import BgImg from '@/components/BgImg.vue'
import YmMain from '@/components/YmMain.vue'

export default {
  name: 'home',
  components: {
    BgImg,
    YmMain
  }
}
</script>

<style lang="scss">
.home{
  height: 100%;
  background-color: #ccc;
}
</style>
