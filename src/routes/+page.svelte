<script>
	import Button from '$lib/marketing/Button.svelte';
</script>

<h1>Welcome to your library project</h1>
<p>Create your package using @sveltejs/package and preview/showcase your work with SvelteKit</p>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>

<div class="p-8 flex flex-col items-center gap-4">
	<Button
		class="text-md bg-slate-600 border-slate-600 hover:bg-transparent hover:text-slate-600 active:text-slate-500 simple-base"
	>
		<svelte:fragment slot="content">Download</svelte:fragment>
	</Button>

	<Button class="simple-border">
		<svelte:fragment slot="content">Download</svelte:fragment>
	</Button>

	<Button class="icon-base">
		<svelte:fragment slot="content">Download</svelte:fragment>

		<svelte:fragment slot="icon">
			<svg
				class="h-5 w-5"
				xmlns="http://www.w3.org/2000/svg"
				fill="none"
				viewBox="0 0 24 24"
				stroke="currentColor"
			>
				<path
					stroke-linecap="round"
					stroke-linejoin="round"
					stroke-width="2"
					d="M17 8l4 4m0 0l-4 4m4-4H3"
				/>
			</svg>
		</svelte:fragment>
	</Button>

	<Button class="icon-border">
		<svelte:fragment slot="content">Download</svelte:fragment>

		<svelte:fragment slot="icon">
			<svg
				class="h-5 w-5"
				xmlns="http://www.w3.org/2000/svg"
				fill="none"
				viewBox="0 0 24 24"
				stroke="currentColor"
			>
				<path
					stroke-linecap="round"
					stroke-linejoin="round"
					stroke-width="2"
					d="M17 8l4 4m0 0l-4 4m4-4H3"
				/>
			</svg>
		</svelte:fragment>
	</Button>

	<Button class="gradient-base">
		<svelte:fragment slot="content">Download</svelte:fragment>
	</Button>

	<Button class="gradient-pill">
		<svelte:fragment slot="content">Download</svelte:fragment>
	</Button>
</div>
