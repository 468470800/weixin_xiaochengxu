<template>
	<image  @click="handleClick" class="img-border" :src="src"></image>
</template>

<script>
	export default{
		props:{
			src:String
		},
		methods:{
			handleClick(){
				this.$emit('srcChange',this.src)
			}
		}
	}
</script>

<style>
	.img-border{
			width: 300rpx;
			height: 300rpx;
			border-radius: 50%;
		}
</style>
