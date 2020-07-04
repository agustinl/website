<script context="module">
	import { isLoading, waitLocale } from 'svelte-i18n';

  	export async function preload(page) {
    	return waitLocale();
  	}
</script>

{#if $isLoading}
  	<div class="loading">Loading...</div>
{:else}
    <main>
    	<slot />
  	</main>
{/if}