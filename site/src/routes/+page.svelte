<script lang="ts">
	import { siInstagram, siFacebook, siTiktok, siX, siGithub } from 'simple-icons';
	import { faLinkedin } from '@fortawesome/free-brands-svg-icons';

	const links = [
		{
			label: 'Instagram',
			href: 'https://instagram.com/sem_pruijs/',
			viewBox: '0 0 24 24',
			path: siInstagram.path
		},
		{
			label: 'Facebook',
			href: 'https://facebook.com/profile.php?id=61584281690680',
			viewBox: '0 0 24 24',
			path: siFacebook.path
		},
		{
			label: 'TikTok',
			href: 'https://tiktok.com/@sem.pruijs',
			viewBox: '0 0 24 24',
			path: siTiktok.path
		},
		{ label: 'X', href: 'https://x.com/sempruijs', viewBox: '0 0 24 24', path: siX.path },
		{
			label: 'LinkedIn',
			href: 'https://www.linkedin.com/in/sem-pruijs-a153a62ab/',
			viewBox: `0 0 ${faLinkedin.icon[0]} ${faLinkedin.icon[1]}`,
			path: faLinkedin.icon[4]
		},
		{
			label: 'GitHub',
			href: 'https://github.com/sempruijs',
			viewBox: '0 0 24 24',
			path: siGithub.path
		}
	];
</script>

<main class="min-h-screen flex flex-col items-center justify-center text-center px-4">
	<h1 class="text-5xl font-bold">Sem Pruijs</h1>
	<img
		src="/sem-pruijs.jpeg"
		alt="Sem Pruijs"
		class="mt-10 w-56 h-56 rounded-full object-cover border border-offblack/15 dark:border-offwhite/20"
	/>

	<nav class="mt-8 flex flex-wrap justify-center gap-3">
		{#each links as link}
			<a
				href={link.href}
				aria-label={link.label}
				class="flex items-center justify-center w-11 h-11 rounded-full border border-offblack/30 dark:border-offwhite/30 text-offblack dark:text-offwhite bg-offblack/5 dark:bg-offwhite/5 hover:bg-offblack/10 dark:hover:bg-offwhite/15 transition"
			>
				<svg viewBox={link.viewBox} class="w-5 h-5 fill-current" aria-hidden="true">
					<path d={link.path} />
				</svg>
				<span class="sr-only">{link.label}</span>
			</a>
		{/each}
	</nav>
</main>
