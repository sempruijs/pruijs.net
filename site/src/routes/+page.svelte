<script lang="ts">
	const links = [
		{ label: 'GitHub', href: 'https://github.com/sempruijs' },
		{ label: 'LinkedIn', href: 'https://www.linkedin.com/in/sem-pruijs/' },
		{ label: 'X', href: 'https://x.com/sempruijs' },
		{ label: 'Instagram', href: 'https://instagram.com/sem_pruijs/' },
		{ label: 'TikTok', href: 'https://tiktok.com/@sem.pruijs' },
		{ label: 'Facebook', href: 'https://facebook.com/profile.php?id=61584281690680' }
	];
</script>

<main class="min-h-screen flex flex-col items-center justify-center text-center px-4">
	<h1 class="text-5xl font-bold">Sem Pruijs</h1>
	<img
		src="/sem-pruijs.jpeg"
		alt="Sem Pruijs"
		class="mt-6 w-56 h-56 rounded-full object-cover border border-offblack/15 dark:border-offwhite/20"
	/>

	<nav class="mt-8 flex flex-wrap justify-center gap-3">
		{#each links as link}
			<a
				href={link.href}
				target="_blank"
				rel="noopener noreferrer"
				class="px-4 py-2 rounded-full border border-offblack/15 dark:border-offwhite/20 text-sm text-offblack/80 dark:text-offwhite/80 hover:bg-offblack/5 dark:hover:bg-offwhite/10 hover:text-offblack dark:hover:text-offwhite transition"
			>
				{link.label}
			</a>
		{/each}
	</nav>
</main>
