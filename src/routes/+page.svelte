<script lang="ts">
	export let data;
</script>

<main>
	<h1>Liste d'épicerie de {data.props.user.email}</h1>

	{#each data.props.grocery.items as item}
		<p>{item.name} x{item.quantity}</p>
	{/each}
</main>

<!-- <style>
	main {
		display: flex;
		justify-content: center;
		align-items: center;
		height: 100vh;
		flex-direction: column;
	}
</style> -->
