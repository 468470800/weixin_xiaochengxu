<template>
	<view>
		<my-form>
			<view>
				<input type="text">
				</view>
		</my-form>
	</view>
	
</template>

<script>
	//引入 组件
import myForm from "@/components/my-form.vue"
export default{
	components:{
		myForm
	},
	onLoad(){
		console.log("onLoad 页面加载完毕")
	},
	onShow(){
		console.log("页面被看到")
	},
	mouted(){
		console.log("myfrom mouted 组件挂载完毕")
	}
}
</script>

<style>

</style>
