<template>
	<view class="page">
		<page-head :title="title"></page-head>
		<view class="uni-card">
			<view class="uni-card-content">
				<view class="uni-card-content-inner">
					这是一个最简单的卡片视图控件；卡片视图常用来显示完整独立的一段信息，比如一篇文章的预览图、作者信息、点赞数量等
				</view>
			</view>
		</view>
		<view class="uni-card">
			<view class="uni-card-header">页眉</view>
			<view class="uni-card-content">
				<view class="uni-card-content-inner">
					包含页眉页脚的卡片，页眉常用来显示面板标题，页脚用来显示额外信息或支持的操作（比如点赞、评论等）
				</view>
			</view>
			<view class="uni-card-footer">页脚</view>
		</view>
		<view class="uni-card">
			<view class="uni-card-header uni-card-media">
				<image class="uni-card-media-logo" src="https://img-cdn-qiniu.dcloud.net.cn/uniapp/images/uni@2x.png"></image>
				<view class="uni-card-media-body">
					<text class="uni-card-media-text-top">小U</text>
					<text class="uni-card-media-text-bottom">发表于 2018-01-30 15:30</text>
				</view>
			</view>
			<view class="uni-card-content image-view">
				<image src="https://img-cdn-qiniu.dcloud.net.cn/uniapp/images/shuijiao.jpg" class="image"></image>
			</view>
			<view class="uni-card-footer">
				<view class="uni-card-link">Like</view>
				<view class="uni-card-link">Comment</view>
				<view class="uni-card-link">Read more</view>
			</view>
		</view>
	</view>
</template>

<script>
	import pageHead from '../../../components/page-head.vue'

	export default {
		data: {
			title: 'cardview'
		},
		components: {
			pageHead
		}
	}
</script>

<style>
	@import "../../../common/uni.css";

	.page {
		padding-top: 60px;
	}

	page {
		background: #efeff4;
	}

	.image-view {
		height: 480px;
		overflow: hidden;
	}

	.image {
		width: 100%;
	}
</style>
