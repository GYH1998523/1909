<template>
	<view style="width: 100vw;height: 100vh;background-color: white;">
		<view class="cu-bar search blue_bj">
			<view class="search-form  round">
				<text class="cuIcon-search"></text>
				<input @focus="InputFocus" @blur="InputBlur" :adjust-position="false" type="text" placeholder="快来搜索你想要的"
				 confirm-type="search"></input>
			</view>
			<view class="action">
			</view>
		</view>
		<!-- sort头 -->
		<view class="list_sort">
			<view class="list">默认</view>

			<view class="list">
				销量
				<view class="sort">
					<view> <text class=" up   cuIcon-triangleupfill"></text></view>
					<view> <text class="  down  cuIcon-triangledownfill"></text></view>
				</view>
			</view>
			<view class="list">价格</view>
		</view>
		<!-- 搜索列表 -->
		<view class="goods_list">
			<view class="list_img">
				<image src="https://ossweb-img.qq.com/images/lol/web201310/skin/big37006.jpg"></image>
			</view>
			<view class="list_info">
				<view class="info_conn"> 稳捷倍优血糖测试仪家用血糖仪精准
					测血糖的仪器稳豪试纸50片</view>
				<view class="info_params">大屏彩显 5秒测糖 600组记忆储存 </view>
				<view class="info_price">
					<text class="info_price_now">￥ 688</text>
					<text class="info_price_old">￥895</text>
					<text class="info_price_sale">销量：120</text>
				</view>
			</view>
		</view>

	<view class="goods_list">
			<view class="list_img">
				<image src="https://ossweb-img.qq.com/images/lol/web201310/skin/big37006.jpg"></image>
			</view>
			<view class="list_info">
				<view class="info_conn"> 稳捷倍优血糖测试仪家用血糖仪精准
					测血糖的仪器稳豪试纸50片</view>
				<view class="info_params">大屏彩显 5秒测糖 600组记忆储存 </view>
				<view class="info_price">
					<text class="info_price_now">￥ 688</text>
					<text class="info_price_old">￥895</text>
					<text class="info_price_sale">销量：120</text>
				</view>
			</view>
		</view>
		
	<view class="goods_list">
			<view class="list_img">
				<image src="https://ossweb-img.qq.com/images/lol/web201310/skin/big37006.jpg"></image>
			</view>
			<view class="list_info">
				<view class="info_conn"> 稳捷倍优血糖测试仪家用血糖仪精准
					测血糖的仪器稳豪试纸50片</view>
				<view class="info_params">大屏彩显 5秒测糖 600组记忆储存 </view>
				<view class="info_price">
					<text class="info_price_now">￥ 688</text>
					<text class="info_price_old">￥895</text>
					<text class="info_price_sale">销量：120</text>
				</view>
			</view>
		</view>		

	</view>
</template>

<script>
	export default {
		data() {
			return {

			};
		}
	}
</script>

<style lang="scss">
	@import "./goods_search.scss"
</style>
