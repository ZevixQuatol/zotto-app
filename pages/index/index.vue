<template>
	<view class="index-view">
		<view class="index-card">
			<view class="index-card-head">
				<text class="index-card-title">超级大乐透</text>
				<!-- <wd-switch v-model="dltSwitch" active-color="#3D5A80" inactive-color="#0F1C2E"></wd-switch> -->
				<view class="z-btn">
					<text>选号</text>
					<wd-icon name="arrow-right" size="18px"></wd-icon>
				</view>
			</view>
			<view class="index-card-content" v-if="dltSwitch">
				<view class="draw-num">
					<view class="font-num">01 02 03 04 05</view>
					<view class="back-num">06 07</view>
				</view>
				<view class="draw-date">
					<text>2025140期</text>
					<text>2025-01-01 08:00:00</text>
				</view>
			</view>
		</view>
	</view>
</template>

<script setup>
import { onLoad, onShow } from '@dcloudio/uni-app';
import { ref } from 'vue';

const dltSwitch = ref(true);
</script>

<style></style>