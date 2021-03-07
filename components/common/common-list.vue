<template>
		<view class="m-2">
			<view class="flex align-center justify-between">
				<view class="flex align-center justify-start">
					<image class="rounded-circle mr-2" style="width: 65rpx;height: 65rpx;" :src="item.userpic" mode="" lazy-load="true"></image>
					<view class="">
						<view class="font">{{item.username}}</view>
						<text class="font-sm text-light-muted">{{item.newstime}}</text>
					</view>
				</view>
				<view v-if="!item.isFollow" class=" rounded" style="height: 50rpx;width: 90rpx;">关注</view>
			</view>
			<view class="font mt-2 mb-2">
				{{item.title}}
			</view>
			<image class=" rounded list-image" :src="item.titlepic" mode=""></image>
			<view class="flex align-center">
				<view class="flex align-center justify-center flex-1">
					<text class="icon icon-dianzan2"></text>
					<text class="ml-2">{{item.support.support_count}}</text>
				</view>
				<view class="flex align-center justify-center flex-1">
					<text class="icon  icon-cai"></text>
					<text class="ml-2">{{item.support.unsupport_count}}</text>
				</view>
				<view class="flex align-center justify-center flex-1">
					<text class="icon  icon-pinglun2"></text>
					<text class="ml-2">{{item.comment_count}}</text>
				</view>
				<view class="flex align-center justify-center flex-1">
					<text class="icon  icon-fenxiang"></text>
					<text class="ml-2">{{item.share_num}}</text>
				</view>
			</view>
		</view>
		
		
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		props:{
			item:Object,
			index:Number
		},
		methods: {
			
		}
	}
</script>

<style>

	.list-image{
		width: 100%;
		height: 350rpx;
	}

</style>
