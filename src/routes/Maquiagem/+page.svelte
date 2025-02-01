<script>
	const produtos = [
		{
			title: 'Blush Rare Beauty',
			image: 'https://encrypted-tbn2.gstatic.com/shopping?q=tbn:ANd9GcS_egj6CdPYxrOPKuMDVZEJgTcOjyJfHP1pvrS-MoN9BExUXBNFic5HRXLDikpnqBf-bmCV-k-4CL_BhRCuuX62wNj6RPKQS1-ya-rFt1QoiQnPihPwe-o4&usqp=CAE',
			description: 'Este blush líquido tem um acabamento natural e radiante.'
		},
		{
			title: 'Corretivo Ruby Kisses',
			image: 'https://kissnewyork.vtexassets.com/arquivos/ids/169044/731509990379_UC10B_ABERTO.jpg?v=638542323366870000',
			description: 'Meu favorito pra usar pra olheiras'
		},
		{
			title: 'Gloss Kiko Milano',
			image: 'https://encrypted-tbn3.gstatic.com/shopping?q=tbn:ANd9GcQzGIBpX51F6D2AtooV3Fb6N0A7nZmUYxY79ugQIQGstbZiC5CvpUq9BXzOPyRgS5Xc4wlzMGIga6a10Ld1g8yt8kuZw4T5lTmc12yvLCENjD05Ehsaunzy4Vw&usqp=CAE',
			description: 'Tem ótimo brilho e efeito volumizador, deixando os lábios brilhando.'
		},
		{
			title: 'Contorno Océane',
			image: 'https://oceane.vtexassets.com/arquivos/ids/205722/AP2001175CO016F_contorno_em_bastao_medium_marrom_medio_oceane_edition_1.jpg?v=638429130933870000',
			description: 'Muito bom pra esculpir o formato do rosto.'
		},
		{
			title: 'Rímel Melu',
			image: 'https://encrypted-tbn2.gstatic.com/shopping?q=tbn:ANd9GcQn6RdVsCZw3SKuy3DhDh-PurphIJpDlF7gosMvwWwmA4rE9QTwn0PQtADa-npBP9xC2kGViwYYMCFJXwZPYIfgWrt3fZBuL4lTtBsMXJ7URFvJgyHTeCMVLg&usqp=CAE',
			description: 'A máscara dá volume e alongamento, deixando o olhar com intensidade e definição.'
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
	<h1 style="text-align: center; color: white;">Meus Produtos de Maquiagem Favoritos:</h1>

	<div class="container">
		{#each produtos as produto}
			<div class="row">
				<div class="col-md-8">
					<div class="anime-card card shadow-lg">
						<img src={produto.image} alt={produto.title} />
						<div class="card-body">
							<h2 class="card-title">{produto.title}</h2>
							<div class="card-text-bg">
								<p class="lead">{produto.description}</p>
							</div>
						</div>
					</div>
				</div>
			</div>
		{/each}
	</div>
</div>
