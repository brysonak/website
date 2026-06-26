<svelte:head>
	<title>Azin</title>
	<meta
		name="description"
		content="A modern systems programming language. (In Development)"
	/>
</svelte:head>

<script lang="ts">
	const year = new Date().getFullYear();
</script>

<div class="page">
    <!-- gotta find a way to have one navbar -->
	<nav class="navbar">
		<a href="/" class="logo">
			<span class="accent">A</span>zin
		</a>

		<div class="links">
			<a href="https://docs.azin-lang.org">Documentation</a>
			<a href="/blog">Blog</a>
			<a href="/download">Downloads</a>
			<a href="https://github.com/azin-lang/azin">GitHub</a>
		</div>
	</nav>

	<main class="hero">

		<h1>
			<span class="accent">A</span>zin
		</h1>

		<p class="description">
			A modern systems programming language currently in development.
		</p>

		<div class="buttons">
			<a href="https://docs.azin-lang.org" class="primary">
				Documentation
			</a>

			<a href="https://github.com/azin-lang/azin" class="secondary">
				GitHub
			</a>
		</div>
	</main>

	<footer>
		© {year} Azin Language Project
	</footer>
</div>

<style>
	:global(body) {
		margin: 0;
		background: #09090b;
		font-family:
			Inter,
			system-ui,
			sans-serif;
	}

	.page {
		min-height: 100vh;
		display: flex;
		flex-direction: column;
		background: #09090b;
		color: white;
	}

	.navbar {
		width: min(1200px, calc(100% - 3rem));
		margin: 0 auto;
		padding: 2rem 0;
		display: flex;
		align-items: center;
		justify-content: space-between;
	}

	.logo {
		font-size: 1.7rem;
		font-weight: 800;
		color: white;
		text-decoration: none;
		letter-spacing: -0.03em;
	}

	.accent {
		color: #38bdf8;
	}

	.links {
		display: flex;
		gap: 2.5rem;
	}

	.links a {
		color: #a1a1aa;
		text-decoration: none;
		font-size: 0.95rem;
		transition: color .2s;
	}

	.links a:hover {
		color: #38bdf8;
	}

	.hero {
		flex: 1;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		text-align: center;
		padding: 5rem;
	}

	h1 {
		margin: 0;
		font-size: clamp(5rem, 11vw, 8rem);
		font-weight: 900;
		letter-spacing: -.05em;
		line-height: 0.95;
	}

	.description {
		max-width: 720px;
		margin-top: 2rem;
		font-size: 1.35rem;
		line-height: 1.7;
		color: #a1a1aa;
	}

	.buttons {
		display: flex;
		gap: 1rem;
		margin-top: 3.5rem;
	}

	.primary,
	.secondary {
		padding: 1rem 2rem;
		border-radius: 10px;
		font-weight: 600;
		text-decoration: none;
		transition: .2s;
	}

	.primary {
		background: #0ea5e9;
		color: white;
	}

	.primary:hover {
		background: #38bdf8;
	}

	.secondary {
		border: 1px solid #27272a;
		color: #d4d4d8;
	}

	.secondary:hover {
		border-color: #38bdf8;
		color: white;
	}

	footer {
		padding: 2rem;
		text-align: center;
		font-size: .9rem;
		color: #71717a;
	}
</style>