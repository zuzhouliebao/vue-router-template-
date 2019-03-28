<template>
	<div>
		<div class="header">
			<div class="nav">
				<router-link to="/index" class="logo">我的班课</router-link>
				<router-link to="/task">任务中心</router-link>
				<router-link to="/lib">库管理</router-link>
				<router-link to="/ucenter">个人中心</router-link>
				<router-link to="/sign">退出</router-link>
			</div>
		</div>
		<div class="content"><router-view /></div>
	</div>
</template>

<script>
export default {
	name: 'Index',
	data() {
		return {};
	}
};
</script>

<style>
.header {
	width: 100%;
	height: 80px;
	background-color: #fff;
	display: flex;
	align-items: center;
}
.nav{
	width: 80%;
	margin: 0 auto;
}
a{
	color: darkslategrey;
	font-size: 18pt;
	text-decoration: none;
	margin-right: 50px;
}
a:hover{
	color: rgb(0, 187, 221);
}
.logo{
	margin-right: 50%;
}
.content {
	width: 80%;
	margin: 0 auto;
	margin-top: 20px;
	height: 600px;
}
</style>
