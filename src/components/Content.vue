<template>
	<div class="Content">
		<div class="info">
			<span>Showing
				<span class="number">15</span> results by...
			</span>

		</div>
		<div class="tags">
			<el-tag closable>
				高雄
			</el-tag>
			<el-tag closable>
				Entertainment
			</el-tag>
		</div>
		<div class="cards">
			<el-card :body-style="{ padding: '0px',display:'flex' }">
				<div class="image"></div>
				<div class="card_content">
					<div class="title">Kogi Cosby sweater.</div>
					<div class="description">Donec euismod scelerisque ligula. Maecenas eu varius risus, eu aliquet arcu. Curabitur fermentum suscipit est, tincidunt
						mattis lorem luctus id. Donec eget massa a diam condimentum pretium. Aliquam erat volutpat. Integer ut tincidunt orci.
						Etiam tristique, elit ut consectetur iaculis, metus lectus mattis justo, vel mollis eros neque quis augue. Sed lobortis
						ultrices lacus, a placerat metus rutrum sit amet. Aenean ut suscipit justo.</div>
					<div class="third_line">
						<span class="author">Ethan Foster</span>
						<span class="category">Entertainment</span>
					</div>
					<div class="fourth_line">
						<span class="place">
							<i class="fas fa-map-marker-alt"></i>
							高雄市</span>
						<span class="date">
							<i class="far fa-calendar-alt"></i>
							時間</span>
					</div>
				</div>
			</el-card>

			<el-card :body-style="{ padding: '0px',display:'flex' }">
				<div class="image"></div>
				<div class="card_content">
					<div class="title">In the tumultuous business.</div>
					<div class="description">It was a humorously perilous business for both of us. For, before we proceed further, it must be said that the monkey-rope
						was fast at both ends; fast to Queequeg's broad canvas belt, and fast to my narrow leather one. So that for better
						or for worse, we two, for the time, were wedded; and should poor Queequeg sink to rise no more, then both usage and
						honour demanded, that instead of cutting the cord, it should drag me down in his.</div>
					<div class="third_line">
						<span class="author">Herman Cobb</span>
						<span class="category">Entertainment</span>
					</div>
					<div class="fourth_line">
						<span class="place">
							<i class="fas fa-map-marker-alt"></i>
							高雄市</span>
						<span class="date">
							<i class="far fa-calendar-alt"></i>
							時間</span>
					</div>
				</div>
			</el-card>
		</div>
	</div>
</template>

<script>
	export default {

	}
</script>

<style lang="scss">
	.Content {
		background-color: #F2F2F2;
		display: inline-block;
		width: 100%;
		.info {
			font-size: 24px;
			font-weight: 300;
			.number {
				color: #9013FE;
				font-weight: 500;
			}
			margin-bottom: 8px;

		}
		.tags{
			margin-bottom: 24px;
		}

		.el-card {
			height: 220px;
			margin-bottom: 24px;
			&.last-child {
				margin-bottom: 0;
			}

			.title {
				width: 100%;
				height: 36px;
				font-size: 24px;
				color: #9013FE;
				line-height: 36px;
				font-weight: 500;
				display: inline-block;
				overflow: hidden;
			}
			.description {
				font-size: 16px;
				width: 100%;
				height: 50px;
				display: inline-block;
				overflow: hidden;
			}
			.third_line {
				margin-top: 16px;
				display: flex;
				.author {
					font-size: 16px;
					font-weight: 700;
					margin-right: 8px;
				}
				.category {
					background-color: #D7D7D7;
					color: white;
					border-radius: 11px;
					padding: 0 15px;
				}
			}
			.fourth_line {
				margin-top: 16px;
				display: flex;
				.place {}
				.date {}
			}
		}
		.image {
			min-width: 220px;
			height: 220px;
			background: url('http://element.eleme.io/static/hamburger.50e4091.png');
			display: inline-block;
		}
		.card_content {
			padding: 24px 20px;
			width: 560px;

		}
	}
</style>