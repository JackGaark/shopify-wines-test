<script>
    import "../styles.css"
    import logo from "$lib/images/logo.svg"
</script>

<nav>
    <a class="logo" href="/"><img class="logo" alt="SvelteFlix" src={logo} /></a>

    <div class="links">
        <a href="/contact">Contact</a>
        <a href="/about">Apropos</a>
        <a href="/search">Recherche</a>
        <a href="/newsletter">Info Lettre</a>
        <a href="/login">Log In</a>
        <a href="/cart">Panier</a>
    </div>
</nav>

<main>
    <slot />
</main>

<footer>
    <p>Data provided by 
        <a href="https://www.themoviedb.org/"></a>
    </p>
</footer>


<style>
    nav {
		display: flex;
		width: 100%;
		height: 3rem;
		align-items: center;
		justify-content: space-between;
		color: var(--accent);
		max-width: var(--column);
	}

    img {
        padding-left: 2rem;
        height: 0.5rem;
    }

    .links {
		display: flex;
		gap: 1em;
	}

	.logo {
		height: 80%;
	}
</style>