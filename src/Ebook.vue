<template>
  <div class="ebook">
      
  </div>
</template>
<script>
import Epub from "epubjs";
const DOWNLOAD_URL = '/static/2018_Book_AgileProcessesInSoftwareEngine.epub';
export default {
  // 电子书的解析和渲染
  methods: {
    showEpub() {
      // 生成Book
      this.book = new Epub(DOWNLOAD_URL);
      console.log(this.book);
      console.log(11)
      //生成Rendtion
      //通过Rendtion.display渲染电子书
    },
  },
  mounted () {
     this.showEpub()
     console.log(111)
   }

};
</script>
<style lang="scss" scoped>
@import "./assets/styles/global.scss";
</style>

