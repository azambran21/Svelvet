<script>
	import DocsSideNav from '../../components/DocsSideNav.svelte';
</script>

<svelte:head>
	<title>Svelvet Documentation</title>
</svelte:head>

<div class="flex justify-start text-gray-800 overflow-x-hidden">
	<nav class="hidden md:block border-r min-w-fit px-8 overflow-y-auto pb-24">
		<DocsSideNav />
	</nav>
	<main class="md:max-w-6xl w-auto overflow-y-auto overflow-x-hidden h-fit p-8 pb-24">
		<slot />
	</main>
</div>
