<script>
	import Button from "./Button.svelte";
	import Content from "./Content.svelte";

	export let currentPage, previousPage, nextPage, heading, subheading;
	
</script>

<section class="min-w-[540px] flex flex-col justify-between gap-8 py-8 px-24">
	<Content 
		heading={heading}
		subheading={subheading}
		currentPage={currentPage}
	/>
	{#if currentPage === "/"}
		<Button text="Next Page" filled={true} nextPage={nextPage} />
	{:else if currentPage === "/step-four"}
		<div class="flex justify-between">
			<Button filled={false} previousPage={previousPage} />
			<Button style=" bg-[var(--color-purplish-blue)]" text="Confirm" filled={true} nextPage={nextPage} />
		</div>
	{:else}
		<div class="flex justify-between">
			<Button filled={false} previousPage={previousPage} />
			<Button text="Next Page" filled={true} nextPage={nextPage} />
		</div>
	{/if}
</section>