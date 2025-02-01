<script>
    let { children } = $props();
</script>

<nav class="navbar navbar-expand-sm navbar-dark bg-danger">
    <div class="container-fluid">
        <a class="navbar-brand" href="/#">
            Oiee :)
        </a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav">
                <li class="nav-item">
                    <a class="nav-link" href="/Maquiagem">Maquiagem</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="/Filmes">Filmes</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="/Animes">Animes</a>
                </li>
            </ul>
        </div>
    </div>
</nav>

<style>
    .navbar {
        background-color: #ff69b4 !important;
    }
</style>

{@render children()}