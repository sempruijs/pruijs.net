<script lang="ts">
	import '../app.css';
	let { children } = $props();
</script>

<div class="min-h-screen bg-offwhite text-offblack dark:bg-offblack dark:text-offwhite transition-colors">
{@render children()}
</div>
