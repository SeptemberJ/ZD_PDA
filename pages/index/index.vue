<template>
	<view class="content">
		<view class="module" @click="goList">
			<image class="logo" src="/static/ruku.png"></image>
			<view class="text-area">
				<text class="title">{{title}}</text>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: '入库上架'
			}
		},
		onLoad() {

		},
		methods: {
			goList () {
				uni.navigateTo({
					url: '../order/index'
				})
			}
		}
	}
</script>

<style>
	.content {
		height: 100vh;
		display: flex;
		flex-direction: column;
		align-items: center;
	}
	.module{
		width: 240rpx;
		height: 240rpx;
		padding: 10px 20px 20px 20px;
		background: antiquewhite;
		position: absolute;
		top: 40%;
		transform: translateY(-50%);
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}
	.logo {
		height: 200rpx;
		width: 200rpx;
		margin: 0 auto;
	}

	.text-area {
		display: flex;
		justify-content: center;
	}

	.title {
		font-size: 36rpx;
		color: #333333;
		margin-top: 5px;
	}
</style>
