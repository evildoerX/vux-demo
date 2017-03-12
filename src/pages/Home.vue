<template>
  <div>
    <panel header="板块名称" :footer="footer" :list="list" :type="type"></panel>
    <panel header="板块名称" :footer="footer" :list="list" :type="type"></panel>
  </div>
</template>

<script>
import { Panel } from 'vux'

export default {
  components: {
    Panel
  },
  data () {
    return {
      type: '1',
      list: [{
        src: 'http://placeholder.qiniudn.com/60x60/3cc51f/ffffff',
        title: '圈子名称1',
        desc: '圈子简介......',
        url: '/component/cell'
      }, {
        src: 'http://placeholder.qiniudn.com/60x60/3cc51f/ffffff',
        title: '圈子名称2',
        desc: '圈子简介......',
        url: {
          path: '/component/radio',
          replace: false
        }
      }]
    }
  }
}
</script>