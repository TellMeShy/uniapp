<template>
	<view class="today page_content">
		<view class="today_date base_normal_szie">Mar 28, 2020</view>
		<view class="flex">
			<view class="title lg_normal_szie">Today</view>
			    <image class="ico_normal" mode="scaleToFill" src="../../static/image/ioc_add.png"
			     ></image>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'Hello'
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style lang="scss" scoped>
	.today{
		background-color: $uni-bg-color-grey;
		.today_date{
			padding-top: 29px;
		}
		.flex{
			.title{
				flex: 1;
			}
		}
	}
</style>
