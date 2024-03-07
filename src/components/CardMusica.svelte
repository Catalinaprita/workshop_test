<script>
	export let disco;
	export let artista;
	export let durata;
	export let anno;
	export let immagine;
</script>

<div class="card">
	<img class="card_immagine" src={immagine} alt="Copertina del disco" />
	u
	<div class="card_musica_centro">
		<p>{artista}</p>
		<p class="card_disco_titolo">{disco}</p>
	</div>

	<div class="card_musica_footer">
		<p>{durata}</p>
		<p>{anno}</p>
	</div>
</div>

<style>
	.card {
		background-color: rgb(210, 70, 189);
		width: 250px;
		border-radius: 20px;
		overflow: hidden;
		padding: 20px;
		color: white;
		font-family: Verdana, Geneva, Tahoma, sans-serif;
	}

	.card_disco_titolo {
		font-size: 25px;
	}

	.card_immagine {
		object-fit: cover;
		width: 100%;
		border-radius: 10px;
		aspect-ratio: 1;
	}

	.card_musica_centro {
		margin-top: 20px;
		margin-bottom: 20px;
	}

	.card_musica_footer {
		display: flex;
		flex-direction: row;
		justify-content: space-between;
	}
</style>
