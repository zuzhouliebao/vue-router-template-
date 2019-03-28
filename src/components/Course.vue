<template>
	<el-row>
		<el-button>默认按钮</el-button>
		<el-button type="primary">主要按钮</el-button>
		<el-button type="success">成功按钮</el-button>
		<el-button type="info">信息按钮</el-button>
		<el-button type="warning">警告按钮</el-button>
		<el-button type="danger">危险按钮</el-button>
		<el-button type="text" @click="open">点击打开 Message Box</el-button>
	</el-row>
</template>

<script>
export default {
	name: 'Course',
	data() {
		return {};
	},
	methods: {
		open() {
			this.$alert('这是一段内容', '标题名称', {
				confirmButtonText: '确定',
				callback: action => {
					this.$message({
						type: 'info',
						message: `action: ${action}`
					});
				}
			});
		}
	}
};
</script>

<style></style>
