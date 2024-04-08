<script>
	import { elCairoBean } from '$lib'
	import CoffeeCard from './components/CoffeeCard.svelte'
</script>

<div>
	<CoffeeCard
		name="El Cairo"
		roaster={{ name: 'Prodigal Coffee' }}
		roastType="medium"
		imageUrl={elCairoBean}
	/>
</div>
