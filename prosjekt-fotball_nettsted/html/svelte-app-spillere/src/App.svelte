<script>
	let spillere = [{navn:"Mohamed Salah", fornavn:"Mohamed", etternavn:"Salah", alder:"30", nasjonalitet:"Egypt", høyde:"175 cm", vekt:"71 kg", assister: "13" ,mål: "23", kamper: "35", bilde:"https://media.api-sports.io/football/players/306.png"}, {navn:"Cristiano Ronaldo", fornavn:"Cristiano", etternavn:"Ronaldo", alder:"37", nasjonalitet:"Portugal", høyde: "187 cm", vekt: "85 kg", mål: "18", kamper: "31", assister: "3", bilde: "https://media.api-sports.io/football/players/874.png"}]
	
	let i = 0
	const finnSpiller = () =>{
		i++
		spillere.navn = spillere.navn[i]
	}

</script>

<tag>Søk på en fotballspiller: </tag><input bind:value={spillere.navn}> <br>




{#if spillere.navn === spillere[0].navn}
<h2>{spillere[0].navn}</h2>
<img src={spillere[0].bilde} alt="spillerbilde"> <br>
		Alder: {spillere[0].alder} <br>
		Nasjonalitet: {spillere[0].nasjonalitet} <br>
		Høyde: {spillere[0].høyde} <br>
		Kamper: {spillere[0].kamper} <br>
		Mål: {spillere[0].mål} <br>
		Assister: {spillere[0].assister}

{:else if spillere.navn === spillere[1].navn}
		<img src={spillere[1].bilde} alt="spillerbilde"> <br>
		Alder: {spillere[1].alder} <br>
		Nasjonalitet: {spillere[1].nasjonalitet} <br>
		Høyde: {spillere[1].høyde} <br>
		Kamper: {spillere[1].kamper} <br>
		Mål: {spillere[1].mål} <br>
		Assister: {spillere[1].assister}
{:else}
	
{/if}






