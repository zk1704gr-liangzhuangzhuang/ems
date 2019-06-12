<template>
	<view>
		<uni-list>
			<uni-list-item title="李海星" note="用户名：lhx" show-extra-icon="true" :extra-icon="{color: '#C2C2C2',size: '70',type: 'contact-filled'}" @click="person(1)"></uni-list-item>
		</uni-list>
		<view class="hr"></view>
		<uni-list>
			<uni-list-item title="签到" show-extra-icon="true" :extra-icon="{color: '#4cd964',size: '25',type: 'checkmarkempty'}" @click="person(2)"></uni-list-item>
		</uni-list>
		<view class="hr"></view>
		<uni-list>
			<uni-list-item title="检查更新" note="已是最新版本" show-extra-icon="true" :extra-icon="{color: '#EE4000',size: '25',type: 'download'}" @click="person(3)"></uni-list-item>
			<uni-list-item title="客服热线" note="400-898-8855" show-extra-icon="true" :extra-icon="{color: '#4cd964',size: '25',type: 'phone-filled'}" @click="person(4)"></uni-list-item>
			<uni-list-item title="帮助与反馈" show-extra-icon="true" :extra-icon="{color: '#FF00FF',size: '25',type: 'help'}" @click="person(5)"></uni-list-item>
			<uni-list-item title="新功能介绍" show-extra-icon="true" :extra-icon="{color: '#FFD700',size: '25',type: 'star-filled'}" @click="person(6)"></uni-list-item>
		</uni-list>
		<view class="hr"></view>
		<uni-list>
			<uni-list-item title="设置" show-extra-icon="true" :extra-icon="{color: '#7A67EE',size: '25',type: 'gear'}" @click="person(7)"></uni-list-item>
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
			person(items){
				if(items==1){
					uni.navigateTo({
						url: "../person/user"
					});
				}else if(items==2){
					uni.navigateTo({
						url: "../person/SignIn"
					});
				}else if(items==3){
					console.log(3)
				}else if(items==4){
					uni.makePhoneCall({
						phoneNumber: '400-898-8855' //仅为示例
					});
				}else if(items==5){
					console.log(5)
				}else if(items==6){
					console.log(6)
				}else{
					console.log(7)
				}
			}
		}
	}
</script>

<style>
	@import url("../../static/css/person.css");
</style>
