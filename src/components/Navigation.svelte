<script>
	import NavigationButton from "./NavigationButton.svelte";

	export let steps, page;

	let stepGroup = page;
	
</script>

<section class="absolute top-0 flex flex-col w-full h-full p-8 pt-10 gap-8">
	{#each steps as step}
		<NavigationButton 
			bind:stepGroup={stepGroup}
			active={step.page === stepGroup}
			step={step.step} 
			name={step.name}
			page={step.page}
		/>
	{/each}
</section>