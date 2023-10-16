<script>
	import { onMount } from 'svelte';

	export let timezone;

	let now = new Date();

	const pad = (n) => (n < 10 ? `0${n}` : n);

	const offsets = {
		GMT: 0,
		EDT: -300,
		IST: +330,
		HKT: +480
		// ...
	};

	$: offset = offsets[timezone];

	// probably a terrible way to handle
	// timezone offsets, sue me
	$: d = new Date(now.getTime() + now.getTimezoneOffset() * 60000 + offset * 60000);

	onMount(() => {
		const interval = setInterval(() => {
			now = new Date();
		}, 1000);
		return () => clearInterval(interval);
	});
</script>

<svelte:head>
	<link rel="stylesheet" href="https://unpkg.com/mono-icons@1.0.5/iconfont/icons.css" />
</svelte:head>

<i class="mi mi-clock"><span class="u-sr-only" /></i>
<span>{pad(d.getHours())}</span> :
<span>{pad(d.getMinutes())}</span> :
<span class="seconds"
	>{pad(d.getSeconds())} <i class="mi mi-location"><span class="u-sr-only" /></i>
</span>

<style>
	span {
		font-variant: tabular-nums;
		color: grey;
		position: relative;
		padding: 1px;
	}

	.mi-clock {
		color: grey;
	}
</style>
