<svelte:head>
	<title>bundumpling</title>
</svelte:head>

<header>
	<a href="/"
		><img
			src="logo.png"
			alt="Brush style text displaying 'bundumpling' between mirrored illustrations of a scallion."
		/></a
	>
</header>

<article>
	<section class="socials">
		<ul>
			<li data-site="twitch">
				<a href="https://www.twitch.tv/bundumpling">
					<img src="icons/MdiTwitch.svg" alt="Twitch.TV Icon" />
					<span>Twitch.TV Channel</span>
				</a>
			</li>

			<li data-site="youtube">
				<a href="https://www.youtube.com/@bundumpling">
					<img src="icons/MdiYoutube.svg" alt="YouTube Icon" />
					<span>YouTube Channel</span>
				</a>
			</li>

			<li data-site="speedrun">
				<a href="https://www.speedrun.com/users/bundumpling">
					<img src="icons/MdiRunFast.svg" alt="Icon of a runner" />
					<span>Speedrun Profile</span>
				</a>
			</li>

			<li data-site="github">
				<a href="https://github.com/bundumpling">
					<img src="icons/MdiGithub.svg" alt="Github Icon" />
					<span>Github Repositories</span>
				</a>
			</li>

			<li data-site="bluesky">
				<a href="https://bsky.app/profile/bundumpling.bsky.social">
					<img src="icons/MdiThoughtBubbleOutline.svg" alt="Icon of thought bubbles" />
					<span>Bluesky Profile</span>
				</a>
			</li>
		</ul>
	</section>
</article>

<style>
	:global(body) {
		background-color: #ab540e;
	}

	header {
		display: flex;
		justify-content: center;
	}

	.socials {
		margin-block-start: 3rem;
		display: grid;
		place-items: center;
	}

	.socials > ul {
		display: flex;
		flex-direction: column;
		align-items: stretch;
		gap: 0.5rem;
		list-style: none;
		font-size: 2rem;
		font-weight: 700;
	}

	.socials > ul > li {
		border-width: 3px;
		border-style: solid;
		border-color: #111;
		display: flex;
		gap: 0.5em;
		box-shadow:
			1.2px 0.8px 2.2px rgba(0, 0, 0, 0.02),
			3px 2px 5.3px rgba(0, 0, 0, 0.028),
			5.6px 3.8px 10px rgba(0, 0, 0, 0.035),
			10.1px 6.7px 17.9px rgba(0, 0, 0, 0.042),
			18.8px 12.5px 33.4px rgba(0, 0, 0, 0.05),
			45px 30px 80px rgba(0, 0, 0, 0.07);
	}

	.socials > ul > li:hover {
		border-color: #ffc77f;
	}

	.socials > ul > li > a {
		padding: 0.25em 0.5em;
		text-decoration: none;
		color: #111;
		display: inline-flex;
		align-items: center;
		gap: 0.25em;
	}

	.socials > ul > li > a:visited {
		color: #111;
	}

	li[data-site='twitch'] {
		background-color: #ba2ca6;
	}

	li[data-site='youtube'] {
		background-color: #ae3d44;
	}

	li[data-site='speedrun'] {
		background-color: #3cb564;
	}

	li[data-site='github'] {
		background-color: #dfe0df;
	}

	li[data-site='bluesky'] {
		background-color: #c4fcf0;
	}
</style>
