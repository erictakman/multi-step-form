<script>
	import InputForm from "./InputForm.svelte";
	import Plan from "./Plan.svelte";
	import AddOns from "./AddOns.svelte";
	import Summary from "./Summary.svelte";

	export let heading, subheading, currentPage;
	
</script>

<section class="flex flex-col gap-8">
	<div>
		<h1>{heading}</h1>
		<h2>{subheading}</h2>
	</div>
	{#if currentPage === "/"}
		<InputForm />
	{:else if currentPage === "/step-two"}
		<Plan />
	{:else if currentPage === "/step-three"}
		<AddOns />
	{:else if currentPage === "/step-four"}
		<Summary />
	{/if}
	
</section>

<style>
	h1 {
		font-size: 1.8rem;
		font-weight: 700;
		color: var(--color-marine-blue);
	}

	h2 {
		color: var(--color-cool-gray);
	}
</style>