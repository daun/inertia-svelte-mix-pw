<script context="module">
    import { writable } from 'svelte/store';
    export const title = writable(null);
</script>

<svelte:head>
    <title>{$title ? `${$title} - ProcessWire` : 'ProcessWire Inertia'}</title>
</svelte:head>

<!-- Slot is needed to render each child -->
<slot/>