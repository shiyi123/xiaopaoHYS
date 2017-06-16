<template>
	<div class="mySearch">
		<mt-header fixed title="我要寻药">
	  		 <router-link to="/" slot="left">
			    <mt-button icon="back" v-if="yincang">返回</mt-button>
			  </router-link>
			  <mt-button icon="more" slot="right" @click="xianshi"></mt-button>
	  	</mt-header>
		<div class="Pnumber">
			<input type="text" placeholder="请输入手机号">
		</div>
		<div class="yanzhengma">
			<input type="text" placeholder="请输入手机验证码">
			<button class="btn">获取验证码</button>
		</div>
		<button class="denglu">立即登录</button>
		<router-link to="" class="a1">免费注册</router-link>
		<router-link to="" class="a2">账号登录</router-link>
		<p>您还可以通过以下方式登录：</p>
		<div class="fangshi">
			<dl>
				<dt><img src="http://m.ehaoyao.com/v4/images/xinlang_fa2f7c4.png" alt=""></dt>
				<dd>微博登录</dd>
			</dl>
			<dl>
				<dt><img src="http://m.ehaoyao.com/v4/images/qq1_d6f3c00.png" alt=""></dt>
				<dd>QQ登录</dd>
			</dl>
		</div>
	</div>
</template>
<script>
export default {
  name: 'MySearch',
  data:function(){
		return {
			 yincang:true,
			arr:"",
		}
	}, 	
	methods:{
		xianshi(){
			this.yincang=true
		},
			
	} 
}
</script>
<style scope>
	*{
		margin: 0;
		padding: 0;
	}
	html{
		font-size: 15.625vw;
		/*font-family:"微软雅黑";*/
	}
	.mySearch{
		width:100%;
		height:100vh;
		background: #F2F2F2;
		position: absolute;
		left:0;
		top:1rem;
		z-index:1;
	}
	.mySearch .mint-header{
		background: #0075de;
		height:1rem;
	}
	.mySearch input{
		padding-left:40px;
	}
	.mySearch .Pnumber{
		width:100%;
		height:0.8rem;
	}
	.mySearch .Pnumber input{
		width:100%;
		height:100%;
		border:0;
		outline: none;
		display: block;
	}
	.mySearch .yanzhengma{
		width:100%;
		height:0.8rem;
		border-top: 1px solid #dcdcdc;
		border-bottom: 1px solid #dcdcdc;
		background: #fff;
	}
	.mySearch .yanzhengma input{
		display: block;
		float: left;
		width:50%;
		height: 100%;
		border:0;
		outline: none;
	}
	.mySearch .yanzhengma button{
		display: block;
		width:28%;
		height:80%;
		margin: 1% 3% 0 0;
		border: 0;
		float: right;
		font-size: 0.25rem;
		background: #0075de;
		color:#fff;
		border-radius:2px;
		outline: none;
	}
	.mySearch .denglu{
		width:90%;
		height:0.7rem;
		border:0;
		border-radius: 5px;
		background:#0075de;
		margin-left:5%;
		color:#fff;
		outline: none;
	}
	.mySearch .a1{
		color:#5790bb;
		font-size: 0.25rem;
		float:right;
		border-left: 2px solid #bfbfbf;
		margin-top: 10px;
		padding-left: 10px;
	}
	.mySearch .a2{
		color:#5790bb;
		font-size: 0.25rem;
		float:right;
		margin-top: 10px;
	}
	.mySearch p{
		width:90%;
		height:0.5rem;
		padding-top: 0.25rem;
		margin:40px 0 0 5%;
		border-top:1px solid #dad9d9;
		font-size: 0.25rem;
		color:#666;
	}
	.mySearch .fangshi{
		width:100%;
		height:0.8rem;
		padding-left:10%;
	}
	.mySearch .fangshi dl{
		width:0.9rem;
		height:1.2rem;
		float:left;
		margin-left: 60px;
	}
	.mySearch .fangshi dl dt{
		width:0.7rem;
		height:0.7rem;
		padding: 0.1rem 0 0 0.1rem;
		border-radius: 0.45rem;
		border:1px solid #d2d2d2;
	}
	.mySearch .fangshi dl dt img{
		display: block;
		width:80%;
	}
	.mySearch .fangshi dl dd{
		width:100%;
		height:0.3rem;
		text-align: center;
		line-height: 0.3rem;
		font-size: 0.15rem;
		color:#666;
	}
</style>

