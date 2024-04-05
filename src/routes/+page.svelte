<script>
	import Section1 from '../components/Section1.svelte';
	import Section2 from '../components/Section2.svelte';
	import Section3 from '../components/Section3.svelte';
	import Section4 from '../components/Section4.svelte';

</script>

<main class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4">
	<div class="h-screen w-full sm:order-1 lg:order-1">
		<Section1 />
	</div>
	<div class="h-screen w-full sm:order-2 lg:order-2 ">
		<Section2 />
	</div>
	<div class="h-screen w-full sm:order-4 lg:order-3">
		<Section3 />
	</div>
	<div class="h-screen w-full sm:order-3 lg:order-4">
		<Section4 />
	</div>
</main>

<style lang="postcss">
	:global(html) {
		background-color: theme(colors.gray.100);
	}
</style>
