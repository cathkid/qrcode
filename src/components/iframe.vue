<template>
  <div class="hello">
  	<!-- 头部 -->
	  <div class="title-box">
	  <div class="center">
	      <a href="/"><h1 class="title-logo">qr-batch <span> 二维码批量生成器 </span></h1></a>
	
	        <ul class="title-menu">
	          <a href="/"><li>首　页</li></a>
	          <a href="/bbs.php"><li>留　言</li></a>
	          <a href="/article_list.php"><li>文　章</li></a>
	        </ul>
	
	
	      <div class="guest-login">
	      	<a href="/login.php" >登陆</a>  /  <a href="/register.php" >免费注册</a>
	      	<!--<p id="my-center">Hi '.$_SESSION['guest'].'  <i class="icon iconfont icon-arrow"></i></p>-->
	      </div>
	
	      <ul class="user-center">
	          <a  href="/center.php"><li>个人中心</li></a>
	          <a href="/binduser.php"><li>修改资料</li></a>
	          <li id="unguest">注销登陆</li>
	      </ul>
	  </div>
	</div>
  
   <div class="son-nav-box">
	  <div class="son-nav">
	      <div class="son-nav-item ">
	          <i class="icon iconfont icon-erweima"></i> 二维码 
	      </div>
	      <div class="son-nav-item ">
	        <i class="icon iconfont icon-iconset0256"></i> 条形码 
	      </div>
	      <div class="son-nav-item">
	        <i class="icon iconfont icon-file"></i> 文本码 
	      </div>
	      <div class="son-nav-item">
	        <i class="icon iconfont icon-erweima1"></i> 微信名片 
	      </div>
	  </div>
	</div> 
  
  
  <router-view/>
  
  
  </div>
</template>

<script>
import '../assets/font/iconfont.css';	
export default {
  name: 'iframe',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.son-nav{
	width: 1000px;
	max-width: 1000px;
	display: block;
	margin: auto;
	height: 35px;
	position: relative;
	margin-top: 50px;
}
.son-nav-item{
	text-align: left;
	font-size: 13px;
	height: 35px;
	line-height: 35px;
	float: left;
	color: #666;
	margin: 0 10px;
	display: inline-block;
	box-sizing: border-box;
	cursor: pointer;
}
.son-nav-item a{
	color: #666;
}
.son-nav .active{
	border-bottom: 2px solid #00a1d6;
}

.son-nav-item:hover{
	border-bottom: 2px solid #00a1d6;
}
.son-nav-box{
	background: #f0f0f0;
	width:100%;
	height:35px;
}
.user-center{
	width: 140px;
	height: 124px;
	position: absolute;
	top: 50px;
	right: 0;
	-webkit-border-radius: 2px;
	-moz-border-radius: 2px;
	border-radius: 2px;
	background-color: #fff;
	display: none;
	border: 1px solid #ddd;
	box-shadow: 2px 2px 4px #eee;
	box-sizing: border-box;
}
.user-center li{
	margin-top: 10px;
	width: 100%;
	height: 40px;
	margin: auto;
	border-bottom: 1px solid #eee;
	text-align: center;
	line-height: 40px;
	font-size: 12px;
	color: #666;
	cursor: pointer;
}
.user-center li:hover{
	color: #20a0ff;
}

.user-center li:hover +.guest-login{
	background-color: #20a0ff;
	color: #fff;
}

.guest-login{
	width: 140px;
	float: right;
	height: 50px;
	line-height: 50px;
	cursor: pointer;
	color: #20a0ff;
	text-align: center;
}
.guest-login p{
	text-align: center;
	width: 140px;
	overflow: hidden;
	height: 50px;
	font-size: 12px;
}
 .title-box{
	position: fixed;
	width: 100%;
	background: #fff;
	top: 0;
	z-index: 11;
	border-radius: 2px;
	-webkit-box-shadow: 0 1px 3px rgba(0,0,0,.1);
	box-shadow: 0 1px 3px rgba(0,0,0,.1);
	-webkit-box-sizing: border-box;
	box-sizing: border-box;
}
.title-box .center{
	width: 1000px;
	max-width: 1000px;
	display: block;
	margin: auto;
	height: 50px;
	position: relative;
}
.title-box .title-logo {
    color: #20a0ff;
    line-height: 30px;
    width: 250px;
    float: left;
    margin-top: 10px;
}
.title-box .title-logo span{
	font-size:12px;
	color: #8590a6;
}
.title-menu{
	width:600px;
	float: left;
	height:50px;
}
.title-menu li{
	padding: 0 15px;
	font-size: 15px;
	line-height: 30px;
	color: #8590a6;
	float: left;
	margin-top: 15px;
}
.title-menu li:hover{
	color: #444;
}
</style>
