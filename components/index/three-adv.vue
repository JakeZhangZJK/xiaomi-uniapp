<template>
	<!-- 左边w:373 h530 -->
	<!-- 右边w:375 h264  边h2-->
	<view class="d-flex">
		<image class="img-l" :src="resdata[0].src" lazy-load style="width: 373rpx;height: 530rpx;border-right-width: 2rpx;border-right-style: solid;border-right-color: #F5F5F5;" @tap="event(resdata[0])"></image>
		<view class="d-flex flex-column">
			<image class="img-r1" :src="resdata[1].src" 
			style="width: 375rpx;height: 264rpx;border-bottom: 2rpx solid #F5F5F5;"
			@tap="event(resdata[1])"></image>
			<image class="img-r2" :src="resdata[2].src"
			style="width: 375rpx;height: 264rpx;"
			@tap="event(resdata[2])"></image>
		</view>
	</view>
</template>

<script>
	export default {
		props:{
			resdata:Array
		},
		methods:{
			event(obj){
				console.log(obj)
			}
		}
	}
</script>

<style>
</style>
