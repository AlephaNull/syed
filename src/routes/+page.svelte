<script>
	import Worldclock from './Worldclock.svelte';
</script>

<body>
	<div class="header">
		<h1>Hi, I'm Syed</h1>
		<h3>
			<Worldclock timezone="IST" />
		</h3>
	</div>
	<h2>Developer | Student | Founder</h2>
	<div class="content">
		I'm a 15 year old builder who makes cool stuff if I can focus. I've worked for and founded a
		couple of agencies and startups. I'm a freelance developer, designer, marketer and writer. <br
		/>
		I'm currently busy creating an AI consulting company called <i> firstgenesis </i> . <br />
		I'm interested in the intersection of the arts and humanities with technology and science, particularly
		buidling user-friendly but extremely effecient products and systems. I'm a philomath, philosopher
		and liberal (the classical meaning, not the modern one). I'm religous but skeptical. Welcome to my
		corner of the internet.
	</div>
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
	}
	h2 {
		font-size: 1em;
		color: grey;
		line-height: 1px;
		margin-top: 1px;
		margin-bottom: 2em;
	}

	h3 {
		display: flex;
		positon: relative;
		align-items: center;
	}
	.content {
		line-height: 2em;
	}

	.header {
		display: flex;
		flex-direction: row;
	}
</style>
