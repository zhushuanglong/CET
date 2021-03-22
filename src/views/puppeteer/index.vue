<template>
  <div class="puppeteer-container"></div>
</template>

<script>
// impor
export default {
  name: 'puppeteer',
  data() {
    return {}
  },
  watch: {},
  created() {},
  mounted() {
    this.init()
  },
  methods: {
    init() {
      // const puppeteer = require('puppeteer')
      // (async() => {
      //   const browser = await puppeteer.launch({headless: false})
      //   const page = await browser.newPage()
      //   await page.goto('https://www.dianxiaomi.com/dxmCommodityProduct/index.htm', {waitUntil: 'networkidle'})
      //   //

        
      //   // console.log($('.pull-right .btn-dropdown .button')[1], 1111)
      //   //await page.screenshot({path: './data/zhentaoo/zhentaoo.png', type: 'png'});

      //   // browser.close();
      // })()
    }
  },
  destroyed() {}
}
</script>

<style lang="scss" scoped>
.puppeteer-container {
  
}
</style>
