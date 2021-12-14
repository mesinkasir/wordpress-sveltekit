<script context="module">
	import { browser, dev } from '$app/env';

	// we don't need any JS on this page, though we'll load
	// it in dev so that we get hot module replacement...
	export const hydrate = dev;

	// ...but if the client-side router is already loaded
	// (i.e. we came here from elsewhere in the app), use it
	export const router = browser;
	// since there's no dynamic data here, we can prerender
	// it so that it gets served as a static asset in prod
	export const prerender = true;
</script>
<script>
	import { onMount } from 'svelte'
	const apiURL = 'https://axcora.my.id/wordpress/wp-json/wp/v2/posts/';
	let data = [];onMount(async function() {const response = await fetch(apiURL);data = await response.json();});
</script>
<svelte:head>
	<title>Wordpress Svelte Blog</title>
</svelte:head>
<div class="container">
<div class="row">
<div class="col-12 p-3 p-md-5">
<div class="content lead">
{#each data as item}	
<h1>{item.title.rendered}</h1>
{@html item.content.rendered}
{/each}
</div>
</div>
</div>
</div>