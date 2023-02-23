<script>
	let monthly = false;
	
</script>

<section>
	<div class="flex justify-between">
		<div class="flex flex-col p-4 border rounded-lg border-[var(--color-purplish-blue)] ">
			<img src="/images/icon-arcade.svg" alt="Arcade gaming icon">
			<div >
				<h3></h3>
				<p></p>
			</div>
		</div>
		<div></div>
		<div></div>
	</div>
	<aside class="flex items-center justify-center p-4 rounded-lg gap-8 bg-[var(--color-magnolia)]">
		<p>Monthly</p>
		<button on:click={() => monthly = !monthly} class={"flex items-center p-1 w-12 h-6 rounded-full bg-[var(--color-marine-blue)]" + (monthly ? " justify-start" : " justify-end")}>
			<input bind:checked={monthly} type="checkbox" role="switch" class="rounded-full bg-[var(--color-white)] w-4 h-4 appearance-none">
		</button>
		<p>Yearly</p>
	</aside>
</section>