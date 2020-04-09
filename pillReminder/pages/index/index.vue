<template>
	<view class="today page_content">
		<view class="today_date base_normal_szie">Mar 28, 2020</view>
		<view class="flex today_flex">
			<view class="title lg_normal_szie">Today</view>
			<image class="ico_normal" 
			src="/static/image/ioc_add.png"
			mode="scaleToFill" ></image>
		</view>
		<itemCard @showPop="showPop"></itemCard>
		<view class="confrim">
			<view class="confrim_tit base_normal_szie">Confrim</view>
			<itemCard></itemCard>
		</view>
		<popUp :show="show"></popUp>
	</view>
</template>

<script>
	import itemCard from '../../components/itemCard.vue'
	import popUp from '../../components/popUp.vue'
	export default {
		data() {
			return {
				show: false,
				
			}
		},
		components:{itemCard,popUp},
		onLoad() {

		},
		methods: {
			showPop(){
				this.show = true
			}
		}
	}
</script>

<style lang="scss" scoped>
	page {
	    background-color: $uni-bg-color-grey;
	}

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
