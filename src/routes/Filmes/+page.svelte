<script>
	const series = [
		{
			title: 'Garota de Fora',
			image: 'https://seriemaniacos.tv/wp-content/uploads/2020/10/gfn1.jpg',
			description: 'Eu adorei como a Nanno quebra todas as regras e expõe as hipocrisias da escola de um jeito tão irreverente.'
		},
		{
			title: 'Alice in Borderland',
			image: 'https://cafecomnerd.com.br/wp-content/uploads/2022/12/Alice-in-Borderland-2-trailer-da-segunda-temporada-da-serie-de-ficcao-cientifica-japonesa-na-Netflix.jpg',
			description: 'A mistura de jogos mortais e um cenário apocalíptico me deixou animado.'
		},
		{
			title: 'The 100',
			image: 'https://m.media-amazon.com/images/S/pv-target-images/d7872d8f250cb8782e69631f0de141559973efdf2b1d3aff751ac0c12543bddc.jpg',
			description: 'The 100 é uma montanha-russa de emoções, com dilemas morais que me fizeram refletir sobre as escolhas difíceis em um mundo pós-apocalíptico.'
		},
		{
			title: 'The Walking Dead',
			image: 'https://prod-ripcut-delivery.disney-plus.net/v1/variant/disney/933E0D6CAF547F41DEB8C66ECE2DC2B7246A6590FF25AEA936859FE934336EB5/scale?width=1200&aspectRatio=1.78&format=webp',
			description: 'Mesmo com um exército de zumbis, o que realmente me fisgou foi o drama humano por trás da sobrevivência e os conflitos internos.'
		},
		{
			title: 'You',
			image: 'https://liderica.com.br/media/25maio19-ARTE-SITE-EME-850px-%C3%97-525px-COMPRESSED-1.jpg',
			description: 'A série mistura charme e perversidade de um jeito perturbador que me deixou desconfiado de cada olhar.'
		}
	];
</script>

<style>
	body {
		background-image: url('https://images.tcdn.com.br/img/img_prod/898929/tecido_tricoline_liso_cor_rosa_chiclete_50cm_x_1_50mt_3043_1_8739a7f846693d56c466c016f369d731.jpg');
	}

  .fundo-rosa {
    background-color: #faa3e0; 
  }
	.anime-card {
		transition: transform 0.3s, box-shadow 0.3s;
		background-color: rgba(255, 255, 255, 0.1);
		backdrop-filter: blur(5px);
		border: 1px solid rgba(255, 255, 255, 0.2);
		border-radius: 10px;
		overflow: hidden;
	}

	.card-text-bg {
		background-color: rgba(0, 0, 0, 0.7);
		padding: 1rem;
		border-radius: 10px;
	}

	.container {
		max-width: 960px;
		margin: 0 auto;
		padding: 2rem;
		min-height: 100vh;
	}

	img {
		width: 100%;
		display: block;
		border-top-left-radius: 10px;
		border-top-right-radius: 10px;
	}

	.card-body {
		padding: 1rem;
		color: white;
	}

	.card-title {
		text-align: center;
		margin-bottom: 1rem;
		font-size: 1.5rem;
	}

	.row {
		display: flex;
		justify-content: center;
		margin-bottom: 20px;
	}

	.col-md-8 {
		flex: 0 0 80%;
	}
</style>
<div class="fundo-rosa">
<h1 style="text-align: center; color: white;">Minhas Séries Favoritas:</h1>

<div class="container">
	{#each series as serie}
		<div class="row">
			<div class="col-md-8">
				<div class="anime-card card shadow-lg">
					<img src={serie.image} alt={serie.title} />
					<div class="card-body">
						<h2 class="card-title">{serie.title}</h2>
						<div class="card-text-bg">
							<p class="lead">{serie.description}</p>
						</div>
					</div>
				</div>
			</div>
		</div>
	{/each}
</div></div>
