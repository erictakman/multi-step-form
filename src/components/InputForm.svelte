<script>
	import TextInput from "./TextInput.svelte";

	let labels=["Name", "Email Adress", "Phone Number"];
	let placeholders=["e.g. Stephen King", "e.g. stephenking@lorem.com", "e.g. +1 234 567 890"];
	
</script>

<form class="flex flex-col gap-4" action="">
	{#each labels as label, i}
		<TextInput 
			label={label} 
			placeholder={placeholders[i]}
		/>
	{/each}
</form>