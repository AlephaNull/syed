<script>
	import Worldclock from './Worldclock.svelte';
	import '@fortawesome/fontawesome-free/css/all.min.css';
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
	<section class="hero">
		<div class="content">
			I'm a 15 year old builder who makes cool stuff if I can focus. I've worked for and founded a
			couple of agencies and startups. I also freelance occasioanlly. I'm currently busy creating an
			AI consulting company called <i> firstgenesis </i> . I'm interested in the intersection of the
			arts and humanities with technology and science. I'm a philomath, philosopher and liberal (the
			classical meaning, not the modern one). I'm religous but skeptical. Welcome to my corner of
			the internet.
			<hr />
			<div class="dev-icons">
				<i class="fa-brands fa-html5" />
				<i class="fa-brands fa-css3-alt" />
				<i class="fa-brands fa-square-js" />
				<i class="fa-brands fa-python" />
				<i class="devicon-typescript-plain" />
				<i class="devicon-sass-original" />
				<i class="devicon-postgresql-plain-wordmark" />
				<i class="devicon-bootstrap-plain-wordmark" />
				<i class="devicon-tailwindcss-plain" />
				<i class="devicon-svelte-plain" />
				<i class="devicon-firebase-plain" />
				<i class="devicon-git-plain" />
				<i class="devicon-github-original" />
				<i class="devicon-sqlite-plain" />
				<i class="devicon-figma-plain" />
				<i class="devicon-linux-plain" />
				<i class="devicon-pandas-original-wordmark" />
				<i class="devicon-numpy-original-wordmark" />
				<i class="devicon-vim-plain" />
			</div>
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
		margin-left: 2em;
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
		margin-left: 0.5em;
		margin-right: 2em;
	}

	.dev-icons > i {
		font-size: 2em;
	}

	.header {
		display: flex;
		flex-direction: column;
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
	}
</style>
