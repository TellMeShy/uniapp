<template>
	<view class="today page_content">
		<view class="today_date base_normal_szie">Mar 28, 2020</view>
		<view class="flex today_flex">
			<view class="title lg_normal_szie">Today</view>
			<image class="ico_normal" 
			src="/static/image/ioc_add.png"
			mode="scaleToFill" ></image>
		</view>
		<itemCard></itemCard>
		<view class="confrim">
			<view class="confrim_tit base_normal_szie">Confrim</view>
			<itemCard></itemCard>
		</view>
	</view>
</template>

<script>
	import itemCard from '../../components/itemCard.vue'
	export default {
		data() {
			return {
				title: 'Hello'
			}
		},
		components:{itemCard},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style lang="scss" scoped>
	.today{
		// background-color: $uni-bg-color-grey;
		.today_date{
			padding-top: 58rpx;
		}
		.today_flex{
			margin-top: -6rpx;
			height: 112rpx;
			margin-bottom: 32rpx;
			.title{
				flex: 1;
			}
		}
		.confrim{
			.confrim_tit{
				margin: 16rpx 0;
			}
			
		}
	}
</style>
