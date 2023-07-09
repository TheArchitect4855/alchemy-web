<script>
	import Footer from "./Footer.svelte";
	import HeroIcon from "./HeroIcon.svelte";
</script>

<div class="scroll-container">
	<div class="mobile" style="height: 20vh; height: 20lvh; scroll-snap-align: start;"></div>
	<main>
		<div class="content">
			<HeroIcon />
			<h1>Welcome</h1>
			<h4>
				Alchemy is the new dating app, made specifically for neurodiverse people.
			</h4>

			<p>
				Neurodiverse people <i>date differently.</i> In most cases, this makes
				finding "the one" much more difficult simply because of our different
				approach. <br /> Alchemy aims to fix this: It creates a safe and accepting
				environment for neurodiverse individuals to date like-minded people
				who understand the things that make them different.
			</p>

			<p>
				You don't have to be neurodiverse to use Alchemy - You just have
				to be understanding and supportive of the struggles neurodiverse
				people face in dating.
			</p>

			<h3>Interested?</h3>
			<span>Coming soon to Android and iOS.</span>
		</div>
	</main>
	<Footer />
</div>

<style>
	@media screen and (max-width: 500px) {
		.scroll-container {
			overflow-y: auto;
			scroll-snap-type: y mandatory;

			position: fixed;
			left: 0;
			right: 0;
			top: 0;
			bottom: 0;
		}

		main {
			/* fallbacks */
			min-height: calc(100vh - 24px);

			/* actual values */
			border-top-left-radius: 16px;
			border-top-right-radius: 16px;
			min-height: calc(100lvh - 24px);
			scroll-snap-align: start;
		}
	}

	@media screen and (min-width: 500px) {
		.mobile {
			display: none;
		}

		main {
			aspect-ratio: 1.618;
			border-radius: 16px;
			height: 80vh;
			margin: 10vh auto;
		}
	}

	@media (prefers-color-scheme: dark) {
		:global(body) {
			background-color: black;
			background-image: url("/plants-bg-dark.png");
		}
	}

	@media (prefers-color-scheme: light) {
		:global(body) {
			background-color: var(--primary-color);
			background-image: url("/plants-bg-light.png");
		}
	}

	:global(body) {
		background-attachment: fixed;
		background-position: center;
		background-repeat: repeat;
	}

	.content {
		margin: 0 auto;
		max-width: 50ch;
	}

	main {
		background-color: var(--background-color);
		padding: 16px;
		text-align: center;
	}

	main p {
		text-align: left;
	}
</style>
