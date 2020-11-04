<template>
	<view  class="content" >
	<img-border @srcChange="handeSrcChange" :src="src1"></img-border>
	<img-border @srcChange="handeSrcChange" :src="src2"></img-border>
		</view>	
</template>

<script>
	//引入 组件
import imgBorder from"@/components/img-border";
export default {	
		//声明一下接收父组件
		data(){
			return {
				src1:"https://ss1.bdstatic.com/70cFuXSh_Q1YnxGkpoWK1HF6hhy/it/u=1530300490,912486349&fm=26&gp=0.jpg",
				src2:"https://dss2.bdstatic.com/70cFvnSh_Q1YnxGkpoWK1HF6hhy/it/u=3386097826,1140583544&fm=26&gp=0.jpg"
	             }		
	},
	components:{//注册组件
		imgBorder
	}
}
</script>

<style>

</style>
