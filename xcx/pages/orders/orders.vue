<template>
	<view>
		<view class="cu-bar search bg-white">
			<view class="search-form round">
				<text class="cuIcon-search"></text>
				<input @focus="InputFocus" @blur="InputBlur" :adjust-position="false" type="text" placeholder="搜索图片、文章、视频"
				 confirm-type="search"></input>
			</view>
		</view>
		<scroll-view scroll-x class="bg-white nav">
			<view class="flex text-center">
				<view class="cu-item flex-sub" :class="index==TabCur?'text-orange cur':''" v-for="(item,index) in 4" :key="index"
				 @tap="tabSelect" :data-id="index">
					Tab{{index}}
				</view>
			</view>
		</scroll-view>

		<view class="orderList">
			<view style="padding: 30upx;">
				<view class="order_time">2018/2/3 12:00</view>
				<view class="order_status">待付款</view>
			</view>
			<view class="order_body">
				<view style="height: 160upx;">
					<view class="order_img">
						<image src="https://ossweb-img.qq.com/images/lol/web201310/skin/big10006.jpg"></image>
					</view>
					<view class="order_text">
						<view class="text_js">电动护理床家用多功能老人瘫痪病人全自动</view>
						<view class="text_format">规格：基础款</view>
					</view>
					<view class="order_jgsl">
						<view class="order_price">￥99</view>
						<view class="order_num">x1</view>
					</view>
				</view>
				<view class="order_count">
					<view class="count_total">￥99</view>
					<view class="count_text">合计：</view>
					<view class="count_num">数量:1</view>
				</view>
				<view class="order_submit">
					<button class="cu-btn block  lg ys_white">取消订单</button>
					<button class="cu-btn block  lg  ys_blue">立即付款</button>
				</view>
			</view>

		</view>

		<view class="orderList">
			<view style="padding: 30upx;">
				<view class="order_time">2018/2/3 12:00</view>
				<view class="order_status">待付款</view>
			</view>
			<view class="order_body">
				<view style="height: 160upx;">
					<view class="order_img">
						<image src="https://ossweb-img.qq.com/images/lol/web201310/skin/big10006.jpg"></image>
					</view>
					<view class="order_text">
						<view class="text_js">电动护理床家用多功能老人瘫痪病人全自动</view>
						<view class="text_format">规格：基础款</view>
					</view>
					<view class="order_jgsl">
						<view class="order_price">￥99</view>
						<view class="order_num">x1</view>
					</view>
				</view>
				<view class="order_count">
					<view class="count_total">￥99</view>
					<view class="count_text">合计：</view>
					<view class="count_num">数量:1</view>
				</view>
				<view class="order_submit">
					<button class="cu-btn block  lg ys_white">取消订单</button>
					<button class="cu-btn block  lg  ys_blue">立即付款</button>
				</view>
			</view>

		</view>
		<view class="orderList">
			<view style="padding: 30upx;">
				<view class="order_time">2018/2/3 12:00</view>
				<view class="order_status">待付款</view>
			</view>
			<view class="order_body">
				<view style="height: 160upx;">
					<view class="order_img">
						<image src="https://ossweb-img.qq.com/images/lol/web201310/skin/big10006.jpg"></image>
					</view>
					<view class="order_text">
						<view class="text_js">电动护理床家用多功能老人瘫痪病人全自动</view>
						<view class="text_format">规格：基础款</view>
					</view>
					<view class="order_jgsl">
						<view class="order_price">￥99</view>
						<view class="order_num">x1</view>
					</view>
				</view>
				<view class="order_count">
					<view class="count_total">￥99</view>
					<view class="count_text">合计：</view>
					<view class="count_num">数量:1</view>
				</view>
				<view class="order_submit">
					<button class="cu-btn block  lg ys_white">取消订单</button>
					<button class="cu-btn block  lg  ys_blue">立即付款</button>
				</view>
			</view>

		</view>
		<view class="orderList">
			<view style="padding: 30upx;">
				<view class="order_time">2018/2/3 12:00</view>
				<view class="order_status">待付款</view>
			</view>
			<view class="order_body">
				<view style="height: 160upx;">
					<view class="order_img">
						<image src="https://ossweb-img.qq.com/images/lol/web201310/skin/big10006.jpg"></image>
					</view>
					<view class="order_text">
						<view class="text_js">电动护理床家用多功能老人瘫痪病人全自动</view>
						<view class="text_format">规格：基础款</view>
					</view>
					<view class="order_jgsl">
						<view class="order_price">￥99</view>
						<view class="order_num">x1</view>
					</view>
				</view>
				<view class="order_count">
					<view class="count_total">￥99</view>
					<view class="count_text">合计：</view>
					<view class="count_num">数量:1</view>
				</view>
				<view class="order_submit">
					<button class="cu-btn block  lg ys_white">取消订单</button>
					<button class="cu-btn block  lg  ys_blue">立即付款</button>
				</view>
			</view>

		</view>

	</view>
</template>

<script>
	export default {
		data() {
			return {
				TabCur: 0,

			};
		},
		methods: {
			tabSelect(e) {
				this.TabCur = e.currentTarget.dataset.id;
				this.scrollLeft = (e.currentTarget.dataset.id - 1) * 60
			}
		}
	}
</script>

<style lang="scss">
	@import "./orders.scss"
</style>
