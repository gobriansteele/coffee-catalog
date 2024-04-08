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
	<div
		class="w-full h-full bg-[url('{link.bkgImageUrl}')] bg-cover bg-center bg-no-repeat opacity-50 hover:opacity-80 absolute"
	></div>
</div>
