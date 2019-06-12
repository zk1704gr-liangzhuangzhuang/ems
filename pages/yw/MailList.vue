<template>
	<view>
		<mSearch :show="false" border="1px #BEBEBE solid" placeholder='在6位联系人中搜索' @search="search"></mSearch>
		<uni-list>
			<uni-list-item title="张三" note="电话：13608677462" show-extra-icon="true" :extra-icon="{color: '#4cd964',size: '35',type: 'person-filled'}" @click="MailList(1)"></uni-list-item>
			<uni-list-item title="李四" note="电话：13608677463" show-extra-icon="true" :extra-icon="{color: '#4cd964',size: '35',type: 'person-filled'}" @click="MailList(2)"></uni-list-item>
			<uni-list-item title="王五" note="电话：13608677464" show-extra-icon="true" :extra-icon="{color: '#4cd964',size: '35',type: 'person-filled'}" @click="MailList(3)"></uni-list-item>
			<uni-list-item title="赵六" note="电话：13608677465" show-extra-icon="true" :extra-icon="{color: '#4cd964',size: '35',type: 'person-filled'}" @click="MailList(4)"></uni-list-item>
			<uni-list-item title="钱七" note="电话：13608677466" show-extra-icon="true" :extra-icon="{color: '#4cd964',size: '35',type: 'person-filled'}" @click="MailList(5)"></uni-list-item>
			<uni-list-item title="神八" note="电话：13608677467" show-extra-icon="true" :extra-icon="{color: '#4cd964',size: '35',type: 'person-filled'}" @click="MailList(6)"></uni-list-item>
		</uni-list>
	</view>
</template>

<script>
	import uniList from '@dcloudio/uni-ui/lib/uni-list/uni-list.vue'
	import uniListItem from '@dcloudio/uni-ui/lib/uni-list-item/uni-list-item.vue'
	import mSearch from '@/components/mehaotian-search/mehaotian-search.vue'
	export default {
		components: {
			uniList,
			uniListItem,
			mSearch
		},
		data() {
			return {
				
			};
		},
		methods:{
			 search(e) {
				 console.log(e);
			 },
			 MailList(items){
				 if(items==1){
				 	uni.navigateTo({
						url: '../table/tableMailList'
					});
				 }else if(items==2){
				 	console.log(2)
				 }else if(items==3){
				 	console.log(3)
				 }else if(items==4){
				 	console.log(4)
				 }else if(items==5){
				 	console.log(5)
				 }else{
				 	console.log(6)
				 }
			 }
		}
	}
</script>

<style>

</style>
