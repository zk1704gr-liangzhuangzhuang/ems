<template>
	<view>
		<view class="top">
			<view class="zhuyi">注意：此业务用于企业不同数据库间数据的一个同步作用，点击右侧按钮就可以触发...</view>
			<view class="btn"><button type="warn" class="AcqBtn">数据同步</button></view>
		</view>
		<!-- 同步信息 -->
		<tableAcquisition></tableAcquisition>
	</view>
</template>

<script>
	import tableAcquisition from '../table/tableAcquisition.vue'
	export default {
		components:{tableAcquisition},
		data() {
			return {
				
			}
		},
		mounted() {
			
		},
		methods:{
			
		}
	}
</script>

<style>
	
</style>
