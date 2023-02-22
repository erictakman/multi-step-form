<script>
	import Content from "./Content.svelte";

	export let previousPage, heading, subheading;
	
</script>

<section class="min-w-[540px] max-w-[640px] flex flex-col justify-between gap-8 py-8 px-24">
	<div class="w-fill h-full flex flex-col justify-center items-center gap-4">
		<img src="/images/icon-thank-you.svg" alt="Thank you illustration" class="w-20 h-20 mb-4">
		<h2 class="text-3xl font-bold text-[var(--color-marine-blue)]">{heading}</h2>
		<p class="text-center text-[var(--color-cool-gray)]">{subheading}</p>
	</div>
	<Content 
		heading=""
		subheading=""
		previousPage={previousPage}
	/>
</section>