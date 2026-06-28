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

	.hero {
		flex: 1;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		text-align: center;
		padding: 5rem;
		animation: fadeIn 0.5s ease-out;
	}
	
	.accent {
		color: #38bdf8;
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
		animation: fadeIn 0.5s ease-out;
	}

	.buttons {
		display: flex;
		gap: 1rem;
		margin-top: 3.5rem;
		animation: fadeIn 1s ease-out;
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

	/* yoinked straight out of https://spatulari.com */
	@keyframes fadeIn {
        from {
            opacity: 0;
            transform: translateY(12px);
        }
        to {
            opacity: 1;
            transform: translateY(0);
        }
    }
</style>