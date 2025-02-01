<script>
    let { children } = $props();
</script>

<nav class="navbar navbar-expand-sm" style="background-color: #ff69b4;">
    <div class="container-fluid">
        <a class="navbar-brand" href="/#"><h1>
            Oiee :) </h1>
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
                    <a class="nav-link" href="/Filmes">Fdddilmes</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="/Animes">Animes</a>
                </li>
            </ul>
        </div>
    </div>
</nav>

{@render children()}