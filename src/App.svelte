<script>
	let a, b, c;
	$:x1 = (-b+Math.sqrt(b*b - 4*a*c))/(2*a)
	$:x2 = (-b-Math.sqrt(b*b - 4*a*c))/(2*a)
</script>
	<div>
		<div class="number_inputs">
			<h1>Quadratic Equation Solver</h1>
			<div class="number_input">a = <input type="number" bind:value={a} /></div>
			<div class="number_input">b = <input type="number" bind:value={b} /></div>
			<div class="number_input">c = <input type="number" bind:value={c} /></div>
		</div>
		<div class="roots_container">
			<p>x1 = {x1}</p>
			<p>x2= {x2}</p>
		</div>
	</div>
<style>
	*{
		margin:0;
		padding:0;
   }
   :global(body){
		display: flex;
		justify-content: center;
		align-items: center;
		height: 100vh;
		background-color: #222;
	}
	.number_inputs{
		background-color:#eee;
	 	text-align:center;
		padding:20px
	}
	.number_inputs h1{
		font-size: 25px;
		margin-bottom: 20px;
		padding-bottom: 10px;
		border-bottom: 1px solid #ddd;
	}
	.number_input{
		margin: 10px;
	}
	.number_input input{
		max-width: 40vw;
	}
	.roots_container{
		display: flex;
		flex-wrap: wrap;
		justify-content:space-around;
		align-items:center;
	}
	.roots_container p{
		background-color:#333;
		color:white;
		padding:16px 40px;
		flex: 1;
		text-align:center;
	}
	.roots_container p:nth-child(2) {
		border-left:1px solid #2b2b2b;
	}
	
</style>