<script>
	import { page } from '$app/stores';
	import Footer from '../components/Footer.svelte';
	import TopNav from '../components/TopNav.svelte';
	import '../app.css';
</script>

{#if $page.url.pathname === '/testingplayground'}
	<slot />
{:else}
	<div class="overflow-x-hidden">
		<div class="sticky top-0 left-0 right-0 z-50">
			<!-- <div class="top-0 sticky"> -->
			<TopNav />
		</div>
		<slot />
		<Footer />
	</div>
{/if}

<style></style>
