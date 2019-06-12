<template>
	<view>
		<uni-notice-bar show-close="true" speed="50" show-icon="true" scrollable="true" single="true" :text="text"></uni-notice-bar>
		<wuc-tab textFlex :tab-list="tabList" :tabCur.sync="TabCur" @change="tabChange"></wuc-tab>
		<view v-show="TabCur === 0">
			<energy></energy>
		</view>
		<view v-show="TabCur === 1">
			<produce></produce>
		</view>
		<view v-show="TabCur === 2">
			<tableRank></tableRank>
		</view>
	</view>
</template>

<script>
	import uniNoticeBar from "@dcloudio/uni-ui/lib/uni-notice-bar/uni-notice-bar.vue"
	import WucTab from '@/components/wuc-tab/wuc-tab.vue'
	import energy from "../index/energy.vue"
	import produce from "../index/produce.vue"
	import tableRank from "../table/tableRank.vue"
	export default {
		components: {
			uniNoticeBar,
			WucTab,
			energy,
			produce,
			tableRank
		},
		data() {
			return {
				TabCur: 0,
				tabList: [{ name: '能耗信息' }, { name: '产销模型' }, { name: '港口能耗排名' }],
				text:'开发者须知：本系统正在开发中，欢迎大家及时在我的专栏反馈信息页面提供建议，如有疑问请联系管理员，QQ号1967609601，如有建议请及时反馈，感激不尽！！！'
			}
		},
		methods: {
			tabChange(index) {
				this.TabCur = index;
			}
		}
	}
</script>

<style>
	@import url("../../static/css/index.css");
</style>
