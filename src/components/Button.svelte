<script>
	export let text, filled, previousPage, nextPage, style;

</script>

{#if filled}
	<a href={nextPage} class={"p-4 px-8 bg-[var(--color-marine-blue)] text-[var(--color-white)] rounded-lg self-end hover:opacity-75" + style}>
		{text}
	</a>
{:else}
	<a href={previousPage} class="p-4 bg-none text-[var(--color-cool-gray)] self-start">
		Go Back
	</a>
{/if}
