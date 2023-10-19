<script>
	import Worldclock from './Worldclock.svelte';
	// You will need to pass your parameters to the function
	// You can initialize it with SCP() or SpotifyCurrentlyPlaying()
</script>

<svelte:head>
	<link rel="stylesheet" href="https://unpkg.com/mono-icons@1.0.5/iconfont/icons.css" />
	<link
		rel="stylesheet"
		href="https://cdn.jsdelivr.net/gh/devicons/devicon@v2.15.1/devicon.min.css"
	/>
</svelte:head>

<body>
	<div class="header">
		<h1>Hi, I'm Syed</h1>
		<p class="time">
			<Worldclock timezone="IST" /> in India.
		</p>
	</div>
	<h2>Developer | Student | Founder</h2>
	<hr />
	<section class="hero">
		<div class="content">
			I'm a 15 year old builder who makes cool stuff if I can focus. I've worked for and founded a
			couple of agencies and startups. I also freelance occasioanlly. I'm currently busy creating an
			AI consulting company called <i> firstgenesis </i> . I'm interested in the intersection of the
			arts and humanities with technology and science. I'm a philomath, philosopher and liberal (the
			classical meaning, not the modern one). I'm religous but skeptical. Welcome to my corner of
			the internet. <br />
			<div class="icons">
				<i class="devicon-html5-plain" />
				<i class="devicon-css3-plain" />
				<i class="devicon-tailwindcss-plain" />
				<i class="devicon-javascript-plain" />
				<i class="devicon-nodejs-plain-wordmark" />
				<i class="devicon-sass-original" />
				<i class="devicon-svelte-plain-wordmark" />
				<i class="devicon-bash-plain" />
				<i class="devicon-bootstrap-plain" />
				<i class="devicon-c-plain" />
				<i class="devicon-linux-plain" />
				<i class="devicon-python-plain" />
				<i class="devicon-github-original" />
				<i class="devicon-git-plain" />
				<i class="devicon-postgresql-plain" />
				<i class="devicon-sqlite-plain" />
				<i class="devicon-figma-plain" />
			</div>
		</div>

		<div class="socials">
			I like internet clout. Follow me.
			<ul>
				<li>Instagram</li>
				<li>Twitter/X</li>
				<li>Github</li>
				<li>LinkedIn</li>
				<li>Email</li>
				<li>Calendar</li>
			</ul>
		</div>
	</section>
</body>

<style>
	@import url('https://fonts.googleapis.com/css2?family=Montserrat&family=Raleway:wght@600&display=swap');

	body {
		background: #14191a;
		color: white;
		font-family: 'Montserrat', sans-serif;
		font-family: 'Raleway', sans-serif;
		display: flex;
		flex-direction: column;
		justify-content: center;
		margin: 0;
	}
	h2 {
		font-size: 1.3em;
		color: grey;
		line-height: 1px;
		margin-top: 1px;
		margin-bottom: 2em;
	}

	.time {
		display: flex;
		align-items: flex-end;
		color: grey;
		font-size: 1em;
	}
	.content {
		line-height: 2em;
		align-items: center;
	}

	.icons > i {
		font-size: 2em;
	}

	.socials {
		align-items: center;
	}

	.header {
		display: flex;
		flex-direction: column;
	}

	section {
		height: 100vh;
		display: flex;
	}

	@media screen and (min-width: 779px) {
		body {
			align-items: center;
		}

		h2 {
			margin-top: 0px;
			margin-bottom: 0px;
		}

		.content {
			margin-top: 1em;
			margin-bottom: 1em;
			margin-left: 5em;
			margin-right: 5em;
			font-size: 1.2em;
		}
		section {
			height: 80vh;
		}
	}
</style>
