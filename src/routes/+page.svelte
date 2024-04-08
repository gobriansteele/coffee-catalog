<script>
	import LinkCard from './components/LinkCard.svelte'
	import { coffeeBeans, coffeeShop } from '$lib'

	export let links = [
		{
			text: 'Coffees',
			href: '/coffees',
			bkgImageUrl: coffeeBeans
		},
		{
			text: 'Roasters',
			href: '/roasters',
			bkgImageUrl: coffeeBeans
		},
		{
			text: 'Shops',
			href: '/shops',
			bkgImageUrl: coffeeShop
		}
	]
</script>

<div class="flex-col md:flex-row flex justify-center items-center h-[100vh]">
	{#each links as link}
		<LinkCard {link} />
	{/each}
</div>
