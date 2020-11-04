<template>
	<view class="content">
		<view >{{msg}}</view>
		<view>${{money}}</view>
		<view>{{isRich}}</view>
		<view >{{person.name}}</view>
		<view>{{person.pikli}}</view>
		<view :data-color="color">
			color
		</view>
		<view v-for="(item,i) in list" key="item.id">{{item.id}}{{item.text}}{{i}}</view>
		<view v-if="true">v-if</view>
		<view v-show="false">v-show</view>
		<view>{{cnMoeny}}</view>
		<view><view v-for="item in filterList" :key="item.id" v-if="item.id<=0">{{item.text}}</view></view>
	</view>
</template>

<script>
	export default {
		data(){
			return{
				msg:"黑马程序员-北京",
				money:1000,
				isRich:false,
				person:{
					name:"孙悟空",
					pikli:"筋斗云"
				},
				color:"aquer",
				list:[
					{
						id:1,
						text:'鬼彻'						
					},
					{
						id:2,
						text:'斩光'						
					},
					{
						id:1,
						text:'战魂'						
					}
				]
			}
	},
	computed:{
		cnMoeny(){
			return "¥" + 1000;
		},
		filterList(){//只要 id> 0都不要
			return this.list.filter(v => v.id<1)
		}
	},
	
	}
</script>

<style>
	.content{
		width: 100rpx;
		height: 100rpx;
		background: #007AFF;
	}
</style>
