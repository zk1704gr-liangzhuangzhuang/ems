<template>
	<view>
		<uni-list>
			<uni-list-item title="港口能耗对比" show-extra-icon="true" :extra-icon="{color:'#1296db',size:'30',type:'navigate'}" @click="report(1)"></uni-list-item>
			<uni-list-item title="港口作业量对比" show-extra-icon="true" :extra-icon="{color:'#4cd964',size:'30',type:'navigate'}" @click="report(2)"></uni-list-item>
			<uni-list-item title="流程作业量对比" show-extra-icon="true" :extra-icon="{color:'#1296db',size:'30',type:'navigate'}" @click="report(3)"></uni-list-item>
			<uni-list-item title="设备类比作业量对比" show-extra-icon="true" :extra-icon="{color:'#4cd964',size:'30',type:'navigate'}" @click="report(4)"></uni-list-item>
			<uni-list-item title="流程能耗对比" show-extra-icon="true" :extra-icon="{color:'#1296db',size:'30',type:'navigate'}" @click="report(5)"></uni-list-item>
			<uni-list-item title="设备类比能耗对比" show-extra-icon="true" :extra-icon="{color:'#4cd964',size:'30',type:'navigate'}" @click="report(6)"></uni-list-item>
			<uni-list-item title="港口间设备利用率对比" show-extra-icon="true" :extra-icon="{color:'#1296db',size:'30',type:'navigate'}" @click="report(7)"></uni-list-item>
			<uni-list-item title="成本核算信息" show-extra-icon="true" :extra-icon="{color:'#4cd964',size:'30',type:'navigate'}" @click="report(8)"></uni-list-item>
		</uni-list>
	</view>
</template>

<script>
	import uniList from '@dcloudio/uni-ui/lib/uni-list/uni-list.vue'
	import uniListItem from '@dcloudio/uni-ui/lib/uni-list-item/uni-list-item.vue'
	export default {
		components: {
			uniList,
			uniListItem
		},
		data() {
			return {
				
			}
		},
		onLoad() {

		},
		methods: {
			report(items){
				if(items==1){
					console.log(1)
				}else if(items==2){
					console.log(2)
				}else if(items==3){
					console.log(3)
				}else if(items==4){
					console.log(4)
				}else if(items==5){
					console.log(5)
				}else if(items==6){
					console.log(6)
				}else if(items==7){
					console.log(7)
				}else{
					console.log(8)
				}
			}
		}
	}
</script>

<style>
	
</style>
