<script>
	let width, height;

	const textParts = ['FOL', 'LOW', 'THE', 'MET', 'TA*'];
	const margin = {
		top: 40,
		right: 20,
		bottom: 20,
		left: 20
	};

	$: textHeight = height / 5.6;
</script>

<section id="section1" class="w-full h-full" bind:clientHeight={height} bind:clientWidth={width}>
	<svg {width} {height}>
		{#each textParts as part, i}
			<text
				class="text-[9rem]"
				x={margin.left}
				y={margin.top + textHeight + i * textHeight}
				fill="{i > 3 ? "#ea92ea" : "white"}"
				textLength={width - margin.left - margin.right}
				lengthAdjust="spacingAndGlyphs"
			>
				{part}
			</text>
		{/each}
	</svg>
</section>

<style>
	#section1 {
		background-image: url($lib/images/bamboo.jpg);;
		background-repeat: no-repeat;
	}
</style>
