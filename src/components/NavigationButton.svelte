<script>
	export let step, name, active, stepGroup, page;

</script>

<button on:click={() => stepGroup = page} class="flex items-center gap-4">
	{#if active}
		<div class="step bg-[var(--color-light-blue)]">
			<p class="text-[var(--color-marine-blue)]">{step}</p>
		</div>
	{:else}
		<div class="step bg-none border border-[var(--color-alabaster)]">
			<p class="text-[var(--color-alabaster)]">{step}</p>
		</div>
	{/if}
	<div class="flex flex-col items-start">
		<p class="text-sm text-[var(--color-pastel-blue)]">Step {step}</p>
		<p class="font-bold text-[var(--color-alabaster)]">{name}</p>
	</div>
</button>

<style>
	.step {
		width: 2.5rem;
		height: 2.5rem;
		display: flex;
		align-items: center;
		justify-content: center;
		border-radius: 50%;
	}
	.step p {
		font-weight: 500;
	}
	p {
		text-transform: uppercase;
	}
</style>