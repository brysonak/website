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

		<div class="construction">
			<h2>Downloads Under Construction</h2>

			<p>
				The downloads page is currently under construction.
				Prebuilt binaries and installation instructions will be available soon.
			</p>
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

	.hero {
		flex: 1;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		text-align: center;
		padding: 2rem;
	}

	h1 {
		margin: 0;
		font-size: clamp(4.5rem, 10vw, 7rem);
		font-weight: 900;
		letter-spacing: -0.05em;
		line-height: 1;
	}

	.accent {
		color: #38bdf8;
	}

	.description {
		margin-top: 2rem;
		max-width: 600px;
		font-size: 1.25rem;
		line-height: 1.7;
		color: #d4d4d8;
	}

	footer {
		padding: 2rem;
		text-align: center;
		font-size: 0.9rem;
		color: #52525b;
	}

    .construction {
        margin-top: 3.5rem;
        max-width: 640px;
        width: 100%;
        padding: 2rem;
        border: 1px solid #27272a;
        border-radius: 14px;
        background: #0d0d10;
    }

    .construction h2 {
        margin: 0;
        font-size: 1.4rem;
        font-weight: 700;
        letter-spacing: -0.02em;
        color: white;
    }

    .construction p {
        margin: 1rem 0 0;
        color: #a1a1aa;
        line-height: 1.7;
        font-size: 1rem;
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

    .links {
        display: flex;
        gap: 2.5rem;
    }

    .links a {
        color: #a1a1aa;
        text-decoration: none;
        font-size: 0.95rem;
        transition: color 0.2s;
    }

    .links a:hover {
        color: #38bdf8;
    }
</style>