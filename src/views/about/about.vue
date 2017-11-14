<style lang="less">
	@import '../../styles/common.less';
	@import './about.less';
</style>

<template>
	<div class="">
		<Row>
			<Card>
				<div class="text-center">
					<h3>{{aboutDate.title}}</h3>
					<h5>{{aboutDate.describe}}</h5>
					<p class="step-content" v-html="aboutDate.content"></p>
				</div>
			</Card>
		</Row>
	</div>
</template>

<script>
export default {
	data () {
		return {
			aboutDate: {
				title: '',
				describe: '',
				content: ''
			}
		}
	},
	mounted () {
		this.aboutDate = {
			title: '前端资源规整使用描述',
			describe: '李梦晓',
			content: '&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;规整项目前端资源，便于后续使用前端资源查看，更好的遵循前端规范。此版本为第一个版本，后续如果有更新不断更新添加。添加要写明增加和更改内容。<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;以后添加版本更新时间线'
		};
	}
}
</script>
