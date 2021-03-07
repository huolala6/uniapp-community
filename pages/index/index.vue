<template>
	<view class="content">
		<!-- 列表样式 -->
		<block v-for="(item,index) in list" :key="index">
			<commonList :item="item" :index="index"></commonList>
		</block>
		
		
		
	</view>
</template>

<script>
	import commonList from '@/components/common/common-list.vue';
	export default {
		comments:{
			commonList
		},
		data() {
			return {
				title: 'Hello',
				list:[{
					username:"昵称",
					userpic:"/static/default.jpg",
					newstime:"2019-01-23",
					isFollow:false,
					title:"",
					titlepic:"/static/demo/datapic/11.jpg",
					support:{
						type:"support",
						support_count:1,
						unsupport_count:2
					},
					comment_count:2,
					share_num:2
				},{
					username:"昵称",
					userpic:"/static/default.jpg",
					newstime:"2019-01-23",
					isFollow:false,
					title:"",
					titlepic:"/static/demo/datapic/11.jpg",
					support:{
						type:"support",
						support_count:1,
						unsupport_count:2
					},
					comment_count:2,
					share_num:2
				}]
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style>

</style>
