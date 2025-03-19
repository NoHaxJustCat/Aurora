<script lang="ts">
</script>

{#snippet link({ path, name }: { path: string; name: string })}
	<a href={path}>
		<div class="font-medium text-neutral-900 hover:text-neutral-500">
			{name}
		</div>
	</a>
{/snippet}

<nav
	class="bg-opacity-50 fixed top-0 right-0 left-0 z-10 bg-neutral-50 backdrop-blur-2xl backdrop-filter"
>
	<div class="container mx-auto flex items-center justify-between px-4 py-1 sm:px-6">
		<!-- Left -->
		<div>
			<a href="/">
				<img src="logo.svg" alt="logo" class="h-10 w-10" />
			</a>
		</div>
		<!-- Center -->
		<div class="flex items-center space-x-8">
			{@render link({ path: './team', name: 'Team' })}
			{@render link({ path: './projects', name: 'Projects' })}
			{@render link({ path: './sponsors', name: 'Sponsors' })}
			{@render link({ path: './contacts', name: 'Contacts' })}
		</div>
		<!-- Right -->
		<div></div>
	</div>

	<div
		class="absolute right-0 bottom-0 left-0 h-px bg-gradient-to-r from-neutral-50 via-neutral-200 to-neutral-50"
	></div>
</nav>
