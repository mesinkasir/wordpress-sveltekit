<script context="module">
	export const prerender = true;
</script>

<script>
	import Counter from '$lib/Counter.svelte';
</script>

<svelte:head>
	<title>Home</title>
</svelte:head>





<section>
	<h1>
		<div class="welcome">
			<picture>
				<source srcset="svelte-welcome.webp" type="image/webp" />
				<img src="svelte-welcome.png" alt="Welcome" />
			</picture>
		</div>

		Wordpress - SvelteKit app
	</h1>
<h3 class="text-center">
A svelte kit with wordpress integration , free download source code for learn svelte kit. present by <a href="https://axcora.com">axcora technology</a>.
</h3>
	

	<Counter />
	<div class="container lead">
	<div class="row">
	<div class="col-12 p-3 p-md-5">
	<h3>Installation</h3>
	<p>
	For first you can download wordpress SEO template themes on our github repo.
	</p>
	<p><a href="https://github.com/mesinkasir/wordpress-themes" class="button">Donwload Now</a></p>
	<p>or you can using shell terminal </p>
	<p><code class="bg-dark rounded p-1 text-light">git clone https://github.com/mesinkasir/wordpress-themes.git</code></p>
	<p>If you need template SEO wordpress source code you can visit on <a href="https://axcora.my.id/wordpress">https://axcora.my.id/wordpress</a></p>
	<p>Write content article blog and create a new page and finished your wordpress website blog project. then you can integrate with svelte kit.</p>
	<p>Download svelte kit wordpress project</p>
	<p><a href="https://github.com/mesinkasir/wordpress-sveltekit" class="button">Donwload Now</a></p>
	<p>Or clone from our github repo</p>
	<p><code class="bg-dark rounded p-1 text-light">git clone https://github.com/mesinkasir/wordpress-sveltekit.git</code></p>
	<p>Now we need to install this sveltekit-wordpress project with node npm or git, next you can open shell terminal and run this command</p>
	<p><code class="bg-dark rounded p-1 text-light">npm install</code></p>
	<p>Oke now we need to change API url , so you can visit on src/routes/ open and edit blog.svelte and page.svelte with your text editor, change url api https://axcora.my.id with your domain name website and save it.</p>
	<p>Now we need to test so open shell terminal command prompt and run this command </p>
	<p><code class="bg-dark rounded p-1 text-light">npm run dev</code></p>
	<p>Then open your web browser and visit localhost:3000</p>
	<p>Congratulations now you have finished integrate wordpress website with svelte kit</p>
	<p>A source code present by <a href="https://axcora.com/sourcecode">axcora technology</a> and the developer <a href="https://creativebydre.vercel.app">creativebydre</a></p>
	</div>
	</div>
	</div>
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 1;
	}

	h1 {
		width: 100%;
	}

	.welcome {
		position: relative;
		width: 100%;
		height: 0;
		padding: 0 0 calc(100% * 495 / 2048) 0;
	}

	.welcome img {
		position: absolute;
		width: 100%;
		height: 100%;
		top: 0;
		display: block;
	}
</style>
