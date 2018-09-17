<template>
	<view>
		<view class="fz32  bbm pd da_list" v-if="!isjt&&!rtext">
			{{title}} 
		</view>
		<view class="fz32  bbm pd da_list" v-if="isjt&&rtext">
			{{title}}
			<view class="right_ert">
				<text class="z9 cz jieao_er">{{rtext}}</text>
				<icon class="dx icon-i-right  cz fz30"></icon>
			</view>
			
		</view>
		
		<view class="fz32  bbm pd da_list" v-if="!isjt&&rtext">
			{{title}}
			<view class="right_ert">
				<text class="z9 cz jieao_er ab ">{{rtext}}</text>
				
			</view>
			
		</view>
	</view>
</template>

<script>
	export default {
		props: {
			title: "",
			isjt:"",
			rtext:""
		}
	}
</script>

<style scoped="">

	.da_list {
		position: relative;
		line-height: 80px;
	}

	.right_ert {
		position: absolute;
		right: 10px;
		top: -10px;
	}
	.jieao_er{
		position: relative;
		top: 10px;
	}
	.jieao_er.ab{
		top: 15px;
	}
</style>
