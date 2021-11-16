<script lang="ts">
	import { page } from '$app/stores';
	import NavBar from '$lib/components/NavBar.svelte';
	import NavItem from '$lib/components/NavItem.svelte';
</script>

<header>
	<div class="corner">
		<a href="/"><span class="h3">Michael Edelman</span></a>
	</div>
	<nav>
		<NavBar>
			<NavItem label="Home" path="/" />
			<NavItem label="Blog" path="/blog" />
			<NavItem label="About" path="/about" />
			<NavItem label="Contact" path="/contact" />
		</NavBar>
	</nav>
</header>

<style lang="postcss">
	header {
		display: flex;
		justify-content: space-between;
	}
	nav {
		display: flex;
		justify-content: flex-end;
		flex: 1;
	}
	.corner {
		height: 3rem;
		flex: 1;
	}
	.corner a {
		display: flex;
		align-items: center;
		justify-content: flex-start;
		width: 100%;
		height: 100%;
	}

	.corner a span {
		color: var(--color-red);
		font-weight: 700;
		margin-top: 0;
		padding-bottom: 0;
	}
</style>
