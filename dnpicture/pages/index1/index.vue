<template>
	<view  class="content" >
		<view data-index="11" @click="handleCllick(1,$event)">
		惦记我 1
	    </view>
		<view data-index="22" @click="handleCllick(2,$event)">
		惦记我 2
		</view>
	</view>
	
</template>

<script>
	export default {
		methods:{
			handleCllick(index,event){
				console.log(index,event)
				console.log(event.currentTarget.dataset.index)
			}
		}
	}
		
</script>

<style>

</style>
