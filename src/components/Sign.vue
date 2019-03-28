<template>
	<div>
		<div class="header">
			<router-link to="/"><img src="../assets/logo-1.png" class="logo" /></router-link>
		</div>
		<div class="container"></div>
		<div class="sign-box">
			<router-link to="/sign_up">注册</router-link>
			<router-link to="/sign_in">登录</router-link>
			<router-view />
		</div>
	</div>
</template>

<script>
export default {
	name: 'SignIn',
	data() {
		return {};
	}
};
</script>

<style scoped>
.header {
	width: 100%;
	height: 80px;
	background-color: #fff;
}
.logo {
	width: 200px;
	height: 50px;
	margin-left: 200px;
}
.container {
	width: 100%;
	height: 800px;
	background-image: url(../assets/login-bg.jpg);
	background-size: 100%;
}
.sign-box {
	position: absolute;
	bottom: 120px;
	right: 200px;
	width: 500px;
	height: 400px;
	background-color: #fff;
}
a {
	margin-right: 200px;
	font-size: 16pt;
	color: #aaa;
}
</style>
