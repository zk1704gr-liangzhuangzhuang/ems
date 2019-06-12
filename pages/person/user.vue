<template>
	<view>
		<uni-list>
			<uni-list-item note="lhx" title="用户名"></uni-list-item>
			<uni-list-item note="李海星" title="姓名"></uni-list-item>
			<uni-list-item title="修改密码"></uni-list-item>
			<uni-list-item note="13608677462" title="电话"></uni-list-item>
			<uni-list-item note="123@qq.com" title="邮箱"></uni-list-item>
			<uni-list-item note="女" title="性别"></uni-list-item>
			<uni-list-item note="河南 周口" title="地区"></uni-list-item>
			<uni-list-item note="欣赏为主，好看为辅" title="个性签名"></uni-list-item>
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
		mounted() {
			
		},
		methods:{
			
		}
	}
</script>

<style>
	
</style>
