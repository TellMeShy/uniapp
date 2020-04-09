<template>
	<view class="itemCard flex" :style="{background:cardColorArr[item.type]}">
		<image class="ico_normal"
		 :src="src"
		 mode="scaleToFill" ></image>
		 <view class="itemCard_dl">
		 	<view class="base_normal_szie itemCard_title">
		 		{{item.title}}
		 	</view>
			<view class="sm_normal_szie">
				{{item.subtitle}}
			</view>
		 </view>
	</view>
</template>

<script>
	import {cardColorArr} from './until.js'
	const item = {
			type:0,
			medType:0,
			title:'Amoxicillin at 12:00 PM',
			subtitle:'1 times daily, Before meal'
		}
	export default {
		props:{
			item:{
				type:Object,
				default:()=>item
			}
		},
		data() {
			return {
				cardColorArr,
			};
		},
		computed:{
			src(){
				return `/static/image/med_type/${this.item.medType}.png`
			}
		}
	}
</script>

<style lang="scss" scoped>
	.itemCard{
		width:686rpx;
		height:144rpx;
		margin-bottom: 16rpx;
		background:rgba(255,255,255,1);
		border-radius:16rpx;
		.ico_normal{
			margin: 0 32rpx;
			
		}
		.itemCard_title{
			padding-bottom: 4rpx;
		}
	}
</style>
