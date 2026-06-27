<nav class="navbar">
	<a href="/" class="logo">
		<span class="accent">A</span>zin
	</a>

	<div class="links">
		<a href="https://docs.azin-lang.org">Documentation</a>
		<a href="/blog">Blog</a>
		<a href="/download">Downloads</a>
		<a href="/links">Links</a>
	</div>
</nav>

<style>
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
</style>