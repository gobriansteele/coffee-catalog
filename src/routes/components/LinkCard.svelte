<script lang="ts">
	type Link = {
		href: string
		text: string
		bkgImageUrl?: string
	}

	export let link: Link
</script>

<div class="h-1/3 w-full md:w-1/3 md:h-full flex justify-center items-center relative">
	<a href={link.href} class="underline text-white text-2xl z-10">{link.text}</a>
	<img
		class="object-cover w-full h-full opacity-50 hover:opacity-80 absolute"
		src={link.bkgImageUrl}
		alt=""
	/>
</div>
