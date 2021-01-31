<script>
	export let segment;
</script>

<style>
	nav {
		border-bottom: 1px solid rgba(255,62,0,0.1);
		font-weight: 300;
		padding: 0 1em;
	}

	ul {
		margin: 0;
		padding: 0;
	}

	/* clearfix */
	ul::after {
		content: '';
		display: block;
		clear: both;
	}

	li {
		display: block;
		float: left;
	}

	[aria-current] {
		position: relative;
		display: inline-block;
	}

	[aria-current]::after {
		position: absolute;
		content: '';
		width: calc(100% - 1em);
		height: 2px;
		background-color: rgb(255,62,0);
		display: block;
		bottom: -1px;
	}

	a {
		text-decoration: none;
		padding: 1em 0.5em;
		display: block;
	}
</style>

<nav>
	<ul>
		<li><a aria-current="{segment === undefined ? 'page' : undefined}" href=".">home</a></li>
		<li><a aria-current="{segment === 'best' ? 'page' : undefined}" href="best">베스트</a></li>

		<!-- for the blog link, we're using rel=prefetch so that Sapper prefetches
		     the blog data when we hover over the link or tap it on a touchscreen -->
		<li><a rel=prefetch aria-current="{segment === 'double' ? 'page' : undefined}" href="double">1&1</a></li>
		<li><a rel=prefetch aria-current="{segment === 'outer' ? 'page' : undefined}" href="outer">아우터</a></li>
		<li><a rel=prefetch aria-current="{segment === 'top' ? 'page' : undefined}" href="top">상의</a></li>
		<li><a rel=prefetch aria-current="{segment === 'bottom' ? 'page' : undefined}" href="bottom">하의</a></li>
		<li><a rel=prefetch aria-current="{segment === 'supplies' ? 'page' : undefined}" href="supplies">홈트용품</a></li>
		<li><a rel=prefetch aria-current="{segment === 'accessory' ? 'page' : undefined}" href="accessory">액세서리</a></li>
		<li><a rel=prefetch aria-current="{segment === 'event' ? 'page' : undefined}" href="event">이벤트</a></li>
	</ul>
</nav>
