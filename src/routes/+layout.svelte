<script>
	import '../app.css';
	import Nav from '../components/nav.svelte';
</script>

<div
	class="font-poppins bg-gradient-to-br from-amber-300/50 to-emerald-300/50 dark:from-slate-900 dark:to-stone-900 text-slate-950 transition-colors duration-500 dark:text-zinc-50 w-full min-h-screen"
>
	<main class="max-w-[90%] w-full md:w-3/4 mx-auto py-8 min-h-screen flex flex-col pb-32">
		<Nav />
		<slot />
	</main>
</div>
