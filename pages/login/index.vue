<template>
	<view>
		<u-button @click="sumbitByPost" type="primary">发送登陆验证码</u-button>
	</view>
</template>

<script>
	export default {
		methods: {
			// post示例
			sumbitByPost() {
				this.$u.api.sendLoginCode({phone: '17865288896'}).then(res => {
					console.log(res);
				})
			}
			
		}
	}
</script>

<style>
</style>
