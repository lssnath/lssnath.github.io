<script>
	const animes = [
		{
			title: 'Shingeki no Kyojin',
			image: 'https://i.scdn.co/image/ab67616d0000b273b5a7bc528f2f3d9afddd5280',
			description:
				'É uma montanha-russa de plot-twists, com um clima sombrio e os dilemas existenciais que te deixam vidrado na tela.'
		},
		{
			title: 'Naruto',
			image: 'https://m.media-amazon.com/images/S/pv-target-images/37ae6eaf1e35049384801438c20a4dec3aa06593542c9770c83935d6b84a3e59._SX1080_FMjpg_.jpg',
			description:
				'É aquele clássico que, com suas batalhas épicas e a energia contagiante da amizade, continua conquistando gerações.'
		},
		{
			title: 'Demon Slayer',
			image: 'https://static.wixstatic.com/media/d1d730_5eecce26241c4e3590cf29f856473e2d~mv2.jpg/v1/fill/w_1000,h_500,al_c,q_85,usm_0.66_1.00_0.01/d1d730_5eecce26241c4e3590cf29f856473e2d~mv2.jpg',
			description:
				'A animação é tão boa que te prende do início ao fim, cada luta sendo pura emoção.'
		}
	];
</script>

<style>

    .fundo-rosa {
    background-color: #faa3e0; 
  }
	body {
		background-image: url('https://images.tcdn.com.br/img/img_prod/898929/tecido_tricoline_liso_cor_rosa_chiclete_50cm_x_1_50mt_3043_1_8739a7f846693d56c466c016f369d731.jpg');
	}
	.anime-card {
		transition: transform 0.3s, box-shadow 0.3s;
		background-color: rgba(255, 255, 255, 0.1);
		backdrop-filter: blur(5px);
		border: 1px solid rgba(255, 255, 255, 0.2);
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
	}
	img {
		width: 100%;
		display: block;
		border-top-left-radius: 5px;
		border-top-right-radius: 5px;
	}
	.card-body {
		padding: 1rem;
		color: white;
	}
	.card-title {
		text-align: center;
		margin-bottom: 1rem;
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
<h1 style="text-align: center;">Meus Animes Favoritos:</h1>

<div class="container py-5">
	{#each animes as anime}
		<div class="row justify-content-center mb-4">
			<div class="col-md-8">
				<div class="anime-card card border-0 shadow-lg">
					<img src={anime.image} alt={anime.title} />
					<div class="card-body">
						<h1 class="card-title text-center mb-4">{anime.title}</h1>
						<div class="card-text-bg">
							<p class="lead">{anime.description}</p>
						</div>
					</div>
				</div>
			</div>
		</div>
	{/each}
</div>
</div>