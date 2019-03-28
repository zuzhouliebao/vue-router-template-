<template>
	<div>
		<h2>库管理</h2>
		<div class="side-bar">
			<router-link to="/question_bank">题库</router-link>
			<router-link to="/resource_library">资源库</router-link>
			<router-link to="/active_library">活动库</router-link>
		</div>
		<div class="content"><router-view /></div>
	</div>
</template>

<script>
export default {
	name: 'Lib',
	data() {
		return {
			
		};
	}
};
</script>

<style>
	
</style>
