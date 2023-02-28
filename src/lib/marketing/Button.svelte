<script lang="ts">
</script>

<a class={$$props.class ?? 'simple-base'} href="/download">
	<span class="">
		<slot name="content">(content)</slot>
	</span>
	{#if $$slots.icon}
		<slot name="icon" />
	{/if}
</a>

<style lang="postcss">
	@tailwind base;
	@tailwind components;
	@tailwind utilities;

	@layer components {
		.simple-base {
			@apply inline-block rounded border border-indigo-600 bg-indigo-600 px-12 py-3 text-sm font-medium text-white hover:bg-transparent hover:text-indigo-600 focus:outline-none focus:ring active:text-indigo-500;
		}

		.simple-border {
			@apply inline-block rounded border border-indigo-600 px-12 py-3 text-sm font-medium text-indigo-600 hover:bg-indigo-600 hover:text-white focus:outline-none focus:ring active:bg-indigo-500;
		}

		.icon-base {
			@apply simple-base;
			@apply inline-flex items-center gap-2 rounded px-8;
		}

		.icon-border {
			@apply simple-border;
			@apply inline-flex items-center gap-2 px-8;
		}

		.gradient-base {
			@apply inline-block rounded bg-gradient-to-r from-pink-500 via-red-500 to-yellow-500 p-[2px] hover:text-white focus:outline-none focus:ring active:text-opacity-75;
		}

		.gradient-base > span {
			@apply block rounded-sm bg-white px-8 py-3 text-sm font-medium hover:bg-transparent;
		}

		.gradient-pill {
			@apply inline-block rounded-full bg-gradient-to-r from-pink-500 via-red-500 to-yellow-500 p-[2px] hover:text-white focus:outline-none focus:ring active:text-opacity-75;
		}

		.gradient-pill > span {
			@apply block rounded-full bg-white px-8 py-3 text-sm font-medium hover:bg-transparent;
		}
	}
</style>
