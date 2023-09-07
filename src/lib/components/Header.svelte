<script lang="ts">
	import { isOpenSidebar } from '$lib/stores/dashboardStore';
	import Icon from '@iconify/svelte';

	let isOpenNotifications = false;
	let isOpenDropdown = false;
</script>

<header class="z-10 p-4 md:px-6 bg-white shadow-sm border-b">
	<nav class="flex justify-between items-center">
		<button
			type="button"
			on:click|stopPropagation={() => isOpenSidebar.set(true)}
			class="text-2xl block md:hidden text-primary-700 rounded-lg"
		>
			<Icon icon="mingcute:menu-fill" class="text-3xl" />
		</button>
	</nav>
</header>
