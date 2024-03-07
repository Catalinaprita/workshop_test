<script>
	import CardMusica from '$components/CardMusica.svelte';

	let dischi = [
		{
			artista: 'Galeffi',
			disco: 'Tazza di te',
			durata: '3:71',
			anno: '2010',
			immagine: 'https://i.scdn.co/image/ab67616d0000b273d5490bf80ec7c5f97f57d3d5'
		},
		{
			artista: 'Frah Quintale',
			disco: 'Missili',
			durata: '4:15',
			anno: '2018',
			immagine:
				'https://64.media.tumblr.com/fadc3285ed2f0b9479225f3bc9fa6b65/tumblr_p7te6cr0Wa1rt4h09o1_1280.jpg'
		},
		{
			artista: 'Calcutta',
			disco: 'Saliva',
			durata: '2:40',
			anno: '2017',
			immagine: 'https://cdn.skuola.net/w1200h687/news_foto/2018/calcutta-evergreen.jpg'
		}
	];
</script>

<svelte:head>
	<link rel="stylesheet" href="https://unpkg.com/tailwindcss@3.4.1/src/css/preflight.css" />
</svelte:head>
{#each dischi as disco}
	<CardMusica
		disco={disco.disco}
		artista={disco.artista}
		durata={disco.durata}
		anno={disco.anno}
		immagine={disco.immagine}
	/>
{/each}
