<script>
    import { onMount } from 'svelte';

    onMount(() => {
        document.title = "PC Hardware Deals";
    });
</script>

<section class="tall-section">
    <h1 class="text-3xl font-bold">Find the best offers on PC hardware</h1>
</section>



<style>
    .tall-section {
        background: #5A3C78;
        min-height: 40rem;
        width: 100%;
        display: flex;
        align-items: center;
        justify-content: left;
    }
</style>