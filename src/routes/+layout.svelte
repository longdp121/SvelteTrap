<script>
    /** @type {import('./$types').LayoutData} */
    import { onMount } from 'svelte';
    import '$lib/app.scss';
    onMount(async () => {
		await import('bootstrap');
	});
    import Nav from '$lib/components/Nav.svelte';
    export let data;
</script>

<div class="container">
    <Nav />
    <slot></slot>
</div>

