<script>
</script>

<style>
	h1, p {
		text-align: center;
		margin: 0 auto;
	}

	h1 {
		font-size: 2.8em;
		text-transform: uppercase;
		font-weight: 700;
		margin: 0 0 0.5em 0;
	}

	.min_visual {
		height: 660px;
	}

	@media (min-width: 480px) {
		h1 {
			font-size: 4em;
		}
	}
</style>

<svelte:head>
	<title>메인 페이지</title>
</svelte:head>

<h1>메인 페이지</h1>

<div id="main">
	<div class="main_visual">배너 영역</div>
	<div class="wrap_inner">
		<div class="widget">
			<img src="https://andar.co.kr/web/product/medium/202101/5c49a9dee3f5efe7c4c614576f95cd5d.jpg" />
		</div>
	</div>
</div>
