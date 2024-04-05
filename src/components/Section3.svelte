<script>
	let width, height;

    import water from '$lib/images/water.jpg'

	const margin = {
		top: 20,
		right: 80,
		bottom: 30,
		left: 80
	};
</script>

<section
	class="w-full h-full bg-[#c9b4a1] flex flex-col justify-end pb-4"
	bind:clientHeight={height}
	bind:clientWidth={width}
>
    <img class="absolute top-0 left-0 h-[40%] w-full" src="{water}" alt="water">

	<svg {width} height={height / 2}>
		<text
			class="text-[130px]"
			x={margin.left}
			y={margin.top + 80}
			fill="white"
			textLength={width - margin.left - margin.right}
			lengthAdjust="spacingAndGlyphs"
		>
			26
		</text>
		<text
			class="text-[130px]"
			x={margin.left}
			y={margin.top + 190}
			fill="white"
			textLength={width - margin.left - margin.right}
			lengthAdjust="spacingAndGlyphs"
		>
			04
		</text>
		<text
			class="text-[50px]"
			x={margin.left}
			y={margin.top + 240}
			fill="white"
			textLength={width - margin.left - margin.right}
			lengthAdjust="spacingAndGlyphs"
		>
			19 - 22
		</text>
        <text
        class="text-[30px]"
        x={margin.left}
        y={margin.top + 270}
        fill="white"
        textLength={width - margin.left - margin.right}
        lengthAdjust="spacingAndGlyphs"
    >
      Hochkirchstr.14
    </text>
	</svg>
</section>
