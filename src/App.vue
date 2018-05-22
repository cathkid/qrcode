<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  -webkit-overflow-scrolling: touch;
}
li {
	list-style-type:none;
}
body {
  font-size: 14px;
  background: #f3f3f3;
  color:#181818;
	font-family: -apple-system,BlinkMacSystemFont,Helvetica Neue,PingFang SC,Microsoft YaHei,Source Han Sans SC,Noto Sans CJK SC,WenQuanYi Micro Hei,sans-serif;
}
img {
  position: relative;
  z-index: 1;
}
textarea{
	font-family: -apple-system,BlinkMacSystemFont,Helvetica Neue,PingFang SC,Microsoft YaHei,Source Han Sans SC,Noto Sans CJK SC,WenQuanYi Micro Hei,sans-serif;
}
a{ 
	text-decoration:none; 
} 
</style>
