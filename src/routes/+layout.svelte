<script>
	import Footer from '$lib/components/footer.svelte';

	import Header from '$lib/components/header.svelte';
</script>

<Header/>
<main>
	<slot />
</main>
<Footer/>

<style>
	main {
		padding: 1rem;
		min-height: 50vh;
		background-color: #f5f5f5;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-direction: column;
		gap: 1rem;
	}
</style>
