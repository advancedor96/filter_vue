<template>
	<div id="app">
		<!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
		<el-container>
			<el-header height="92px">
				<Title />
			</el-header>

			<el-container class="toggleRowAndCol">

				<el-aside  style="">
					<Aside />
				</el-aside>
				<el-main style="">
					<Content />
				</el-main>
			</el-container>
			<el-footer style="">
				
			</el-footer>

		</el-container>
	</div>
</template>

<script>
	// import HelloWorld from './components/HelloWorld.vue'
	import Title from './components/Title.vue'
	import Aside from './components/Aside.vue'
	import Content from './components/Content.vue'
	import Test from './components/Test.vue';

	export default {
		name: 'app',
		components: {
			Title,
			Aside,
			Content,
			Test
		}
	}
</script>

<style lang="scss">
	@import url('https://fonts.googleapis.com/css?family=Roboto:100,300,400,500,700,900');


	html,
	body {
		margin: 0;
		padding: 0;
		width: 100%;
		height: 100%;
		font-family: 'Roboto', serif;
		min-width: 360px;

	}

	* {
		box-sizing: border-box;
		position: relative; // border: 1px solid black;
	}

	#app {
		width: 100%;
		height: 100%;
		background-color: #F2F2F2;
	}

	.el-header {
		padding: 0;

	}

	.el-aside {
		max-width: 300px;
		margin-left: 38px;
	} 
	// Pad
	@media only screen and (max-width:900px) and (min-width:414px) {
		.el-aside {
			max-width: 300px !important;
			margin-left: 0 !important;
		}
	}
	// Mobile
	@media only screen and (max-width:414px) {
		.toggleRowAndCol{
			flex-direction: column;
		}
		.el-aside {
			width: 100% !important;
			max-width: none;
			margin: 0;
		}
		.el-main{
			min-width: 250px !important;
		}
	}

	.el-main {
		padding: 0;
		max-width: 820px;
		min-width: 468px;

		padding-right: 40px;
		padding-top: 24px;
		padding-left: 42px;
	}

	.second {
		display: flex;
	}
</style>