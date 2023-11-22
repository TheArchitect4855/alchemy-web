<script>
	import Footer from "./Footer.svelte";
	import HeroIcon from "./HeroIcon.svelte";
</script>

<div class="container">
	<main>
		<article>
			<HeroIcon />
			<h1>Welcome</h1>
			<h4>
				Alchemy is the new dating app, made specifically for neurodiverse
				people.
			</h4>

			<p>
				Neurodiverse people <i>date differently.</i> In most cases, this makes
				finding "the one" much more difficult simply because of our different
				approach. <br /> Alchemy aims to fix this: It creates a safe and accepting
				environment for neurodiverse individuals to date like-minded people who
				understand the things that make them different.
			</p>

			<p>
				You don't have to be neurodiverse to use Alchemy - You just have to be
				understanding and supportive of the struggles neurodiverse people face
				in dating.
			</p>

			<h3>Interested?</h3>
			<div class="badges">
				<a href="https://web.usealchemy.app" target="_blank">
					<img
					alt="iOS Link"
					src="/ios-badge.svg"
					style="height: 3.3em;"
					/>
				</a>
				<a href='https://play.google.com/store/apps/details?id=app.usealchemy.alchemy&pcampaignid=pcampaignidMKT-Other-global-all-co-prtnr-py-PartBadge-Mar2515-1' target='_blank'>
					<img
					alt='Get it on Google Play'
					src='https://play.google.com/intl/en_us/badges/static/images/badges/en_badge_web_generic.png'
					style="height: 5em;"
					/>
				</a>
			</div>
		</article>
		<Footer />
	</main>
</div>

<style>
	@media screen and (min-width: 60ch) {
		main {
			border-radius: 16px;
			margin: 1em auto;
		}
	}

	@media screen and (max-width: 60ch) {
		.container {
			background-attachment: fixed;
		}

		main {
			border-radius: 16px;
			border-bottom-left-radius: 0;
			border-bottom-right-radius: 0;
			margin: 0 auto;
			margin-top: 15vh;
			margin-top: 15lvh;
		}
	}

	.badges {
		display: flex;
		align-items: center;
		justify-content: center;
	}

	.container {
		background-image: url("/plants-bg.png");
		min-height: 100vh;
		min-height: 100lvh;

		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	article {
		margin: 0;
		padding: 1em;
		text-align: center;
	}

	main {
		background-color: var(--background-color);
		box-shadow: 0 0 8px 0 #0005;
		overflow: auto;
		width: min(60ch, 100vw);
	}
</style>
