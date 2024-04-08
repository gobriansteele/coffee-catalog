<script>
	import LinkCard from './components/LinkCard.svelte'

	export let links = [
		{
			text: 'Coffees',
			href: '/coffees',
			bkgImageUrl: '/images/coffee_beans.jpeg'
		},
		{
			text: 'Roasters',
			href: '/roasters',
			bkgImageUrl: '/images/coffee_shop.jpeg'
		},
		{
			text: 'Shops',
			href: '/shops',
			bkgImageUrl: '/images/coffee_shop.jpeg'
		}
	]
</script>

<div class="flex-col md:flex-row flex justify-center items-center h-[100vh]">
	{#each links as link}
		<LinkCard {link} />
	{/each}
</div>
