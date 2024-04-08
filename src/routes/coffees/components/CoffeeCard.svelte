<script lang="ts">
	type Roaster = {
		name: string
	}
	export let name: string
	export let imageUrl: string
	export let roaster: Roaster
	export let roastDate: string = ''
	export let roastType: 'light' | 'medium' | 'dark'

	function capitalizeFirstLetter(string: string) {
		return string.charAt(0).toUpperCase() + string.slice(1)
	}
</script>

<div class="flex flex-col w-[180px] h-[280px] rounded-lg shadow">
	<img class="w-full h-[180px] object-cover rounded-t-lg" src={imageUrl} alt={name} />
	<div class="flex flex-col p-2">
		<h3 class="text-lg font-bold">{name}</h3>
		<p class="text-sm text-gray-500">{roaster.name}</p>
		<p class="text-sm text-gray-500">{roastDate}</p>
		<p class="text-sm text-gray-500">{capitalizeFirstLetter(roastType)}</p>
	</div>
</div>
