<script>
	let spillere = [{navn:"Mohamed Salah", fornavn:"Mohamed", etternavn:"Salah", alder:"30", nasjonalitet:"Egypt", h�yde:"175 cm", vekt:"71 kg", assister: "13" ,m�l: "23", kamper: "35", bilde:"https://media.api-sports.io/football/players/306.png"}, {navn:"Cristiano Ronaldo", fornavn:"Cristiano", etternavn:"Ronaldo", alder:"37", nasjonalitet:"Portugal", h�yde: "187 cm", vekt: "85 kg", m�l: "18", kamper: "31", assister: "3", bilde: "https://media.api-sports.io/football/players/874.png"}]
	
	let i = 0
	const finnSpiller = () =>{
		i++
		spillere.navn = spillere.navn[i]
	}

</script>

<tag>S�k p� en fotballspiller: </tag><input bind:value={spillere.navn}> <br>




{#if spillere.navn === spillere[0].navn}
<h2>{spillere[0].navn}</h2>
<img src={spillere[0].bilde} alt="spillerbilde"> <br>
		Alder: {spillere[0].alder} <br>
		Nasjonalitet: {spillere[0].nasjonalitet} <br>
		H�yde: {spillere[0].h�yde} <br>
		Kamper: {spillere[0].kamper} <br>
		M�l: {spillere[0].m�l} <br>
		Assister: {spillere[0].assister}

{:else if spillere.navn === spillere[1].navn}
		<img src={spillere[1].bilde} alt="spillerbilde"> <br>
		Alder: {spillere[1].alder} <br>
		Nasjonalitet: {spillere[1].nasjonalitet} <br>
		H�yde: {spillere[1].h�yde} <br>
		Kamper: {spillere[1].kamper} <br>
		M�l: {spillere[1].m�l} <br>
		Assister: {spillere[1].assister}
{:else}
	
{/if}






