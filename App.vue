<script>
	export default {
		onLaunch: function() {
			console.log('App Launch')
		},
		onShow: function() {
			console.log('App Show')
		},
		onHide: function() {
			console.log('App Hide')
		}
	}
</script>

<style>
	/*每个页面公共css */
	/* 官方css库 */
	@import "./common/uni.css";
	/* 自定义图表库 */
	@import "./common/iconfont.css";
	/* 引入动画库 */
	@import "./common/animate.css";
	/* 自定义公共样式库 */
	@import "./common/free.css";
	/* 本项目自定义全局样式库 */
	@import "./common/common.css";
</style>
