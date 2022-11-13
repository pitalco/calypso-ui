<script>
	import '../app.css';
	// @ts-ignore
	import NavBar from '../components/NavBar.svelte';
	import Menu from '../components/Menu.svelte';
</script>

<header>
	<div class="nav-div">
		<NavBar />
	</div>
</header>

<main>
	<div class="main-section">
		<slot />
	</div>
</main>

<footer />

<style>
	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		max-width: 1024px;
		margin: 0 auto;
		box-sizing: border-box;
	}

	footer {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		padding: 40px;
	}

	@media (min-width: 480px) {
		footer {
			padding: 40px 0;
		}
	}
	.nav-div {
		padding: 10px;
	}
	.columns {
		display: grid;
		grid-template-columns: 0.18fr 0.82fr;
	}
	.main-section {
		padding: 20px;
	}
</style>
