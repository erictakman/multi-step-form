<script>
	import Navigation from "./Navigation.svelte";

	export let page;

</script>

<aside class="h-auto relative">
	<img src="../images/bg-sidebar-desktop.svg" alt="background" class="w-full h-full">
	<Navigation
		page={page}
		steps={[
			{
				"page": "/",
				"step": 1,
				"name": "Your info",
			},
			{
				"page": "/step-two",
				"step": 2,
				"name": "Select plan",
			},
			{
				"page": "/step-three",
				"step": 3,
				"name": "Add-ons",
			},
			{
				"page": "/step-four",
				"step": 4,
				"name": "Summary",
			}
		]} 
	/>
</aside>
