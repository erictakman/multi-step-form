<script>
	export let label, placeholder;
	
</script>

<div class="flex flex-col gap-1">
	<label class="text-[var(--color-marine-blue)] font-[500]" for="input">{label}</label>
	<input 
		class="p-3 border border-[var(--color-light-gray)] rounded-lg"
		id="input" 
		type="text" 
		placeholder={placeholder} 
	/>
</div>

