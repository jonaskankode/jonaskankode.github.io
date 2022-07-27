<script>
	let drakter = [ "https://store.liverpoolfc.com/media/catalog/product/cache/042594ffe2aeaa6bf11576291063d119/d/j/dj7647r_1_copy.jpg", "https://pbs.twimg.com/media/E6UpSQ3WQAAyrV6.jpg", "https://i2-prod.football.london/incoming/article23896915.ece/ALTERNATES/s1200c/1_Arsenal-22-23-Home-Kit-3.jpg"]
	let i = 0
	const visBilde = () => {
		drakter[i] = drakter[i++] 
		} 
	if(i = drakter.length - 1){
			i=0}
	
	//Fikk litt drlig tid, dermed klarte ikke å resette i haha
		

</script>

<button on:click={visBilde}> Vis neste drakt </button>


<br>

<div>
	<img src={drakter[i]} alt="drakter" style="width:50%; height:50%;">
</div>




