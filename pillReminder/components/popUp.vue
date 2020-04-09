<template>
	<view class="popUp shadow" v-show="show">
		
	</view>
</template>

<script>
	export default {
		props:{
			show:{
				type:Boolean,
				default:false
			}
		},
		data() {
			return {
				
			};
		}
	}
</script>

<style lang="scss">
	.popUp{
		position: fixed;
		bottom: 0;
		left: 0;
		width: 0;
		top: 0;
		width: 100%;
		height: 100%;
		z-index: 999;
	}
</style>
